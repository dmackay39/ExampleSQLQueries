# ExampleSQLQueries
Examples of queries I ran while completing the Codecademy Pro Skill Path: Analyse Data with SQL.

1. For a database called 'transactions' with columns: id INTEGER, user_id INTEGER, date DATE, currency TEXT, money_in REAL, money_out REAL. Build a ledger with the date, average money in, and average money out as the columns.

 SELECT date, 
        ROUND(AVG(money_in),2) AS 'avg in', 
        ROUND(AVG(money_out),2) AS 'avg in' 
 FROM transactions GROUP BY date;
