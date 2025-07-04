# Database Concepts
## ✅ What is a Database?
- A database is an organized collection of data stored electronically. It allows easy access, management, and updating of data.

## ✅ What is a Table?
- A table is a structure inside a database that stores data in rows and columns, like a spreadsheet.

  
## ✅ What is a Record?
- A record (or row) is a single entry in a table that contains values for each column.

## ✅ What is a Transaction?
- A transaction is a sequence of one or more SQL operations that are executed as a single unit of work.
- It ensures data integrity, even in case of failure.

## 💡 A transaction follows ACID properties:
- Atomicity – All or nothing

- Consistency – Always valid state

- Isolation – Transactions don’t interfere

- Durability – Once done, it stays done

## ✅ What is CRUD?
- CRUD is a set of 4 basic operations used to interact with a database.

| Operation  | SQL Keyword | Description          |
| ---------- | ----------- | -------------------- |
| **C**reate | `INSERT`    | Add new data         |
| **R**ead   | `SELECT`    | Fetch data           |
| **U**pdate | `UPDATE`    | Modify existing data |
| **D**elete | `DELETE`    | Remove data          |


## ✅ What is a Rollback Mechanism?
- Rollback is the process of undoing a transaction when something goes wrong, restoring the database to its previous consistent state.
