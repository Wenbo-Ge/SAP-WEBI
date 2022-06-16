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
   
## Freehand SQL prompt syntax
    https://answers.sap.com/questions/12672275/implementation-of.html

## #DATASYNC Error
   ![image](https://user-images.githubusercontent.com/36894305/174075656-1f0d3a85-5151-47b5-b3d7-1b8fa1085321.png)
   Just change variable type to measure
   ![image](https://user-images.githubusercontent.com/36894305/174075867-bb649676-30dd-4bc1-aa0d-93ea12248fab.png)

