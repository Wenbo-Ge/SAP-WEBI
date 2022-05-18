# SAP-WEBI

## Merge Queries
   Select same object from different queries, and merge them at report level
   
## Put Objects From Different Queries In Same Report
   1. First need to merge these queries.
   2. Create the new variable for these objects from different queries (type is measurement)
   3. Then put them in same report
   4. Check Avoid duplicate row aggregation

## Query Script Editor "No column name was specified for column 1" error when puting union table in the FROM Clause
   Solution: give the alias name to that column in every union.
   Then follow the MS SQL Syntax:
   SELECT A
   FROM
   (
       SELECT A, B FROM TableA
       UNION
       SELECT A, B FROM TableB
   ) AS tbl
