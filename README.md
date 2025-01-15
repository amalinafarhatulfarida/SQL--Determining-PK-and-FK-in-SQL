## Foreign Key Relationship Query

This SQL query is designed to explore the foreign key relationships between the `SalesOrderHeader` and `Address` tables in the AdventureWorks database. Specifically, it identifies the columns in the `SalesOrderHeader` table (`ShipToAddressID` and `BillToAddressID`) that reference the `AddressID` column in the `Address` table.

### **Query Explanation**
- Retrieves the name of the foreign key constraint.
- Identifies the parent table (`SalesOrderHeader`) and the column that acts as the foreign key.
- Identifies the referenced table (`Address`) and the corresponding primary key column (`AddressID`).

### **How to Use**
Run the query in SQL Server Management Studio (SSMS) to explore relationships in the AdventureWorks database.

### **Sample Output**
| ForeignKeyName     | ParentTable        | ParentColumn       | ReferencedTable | ReferencedColumn |
|--------------------|--------------------|--------------------|------------------|------------------|
| FK_SalesOrderHeader_ShipToAddress | SalesOrderHeader | ShipToAddressID | Address          | AddressID        |
| FK_SalesOrderHeader_BillToAddress | SalesOrderHeader | BillToAddressID | Address          | AddressID        |
