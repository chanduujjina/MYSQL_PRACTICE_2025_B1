# RelationShip
## One to One Realationship
```mermaid
erDiagram
    USERS ||--|| USER_PROFILES : has
    USERS {
        INT id PK
        VARCHAR name
        VARCHAR email
    }
    USER_PROFILES {
        INT user_id PK, FK
        TEXT bio
        DATE dob
    }
```

## DDL Query

```sql
-- Create USERS table
CREATE TABLE users (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100) UNIQUE
);

-- Create USER_PROFILES table
CREATE TABLE user_profiles (
    user_id INT PRIMARY KEY,  -- also acts as FK
    bio TEXT,
    dob DATE,
    FOREIGN KEY (user_id) REFERENCES users(id)
);
```

## Insert Query
```sql
INSERT INTO users (id, name, email)
VALUES 
(1, 'Alice', 'alice@example.com'),
(2, 'Bob', 'bob@example.com'),
(3, 'Charlie', 'charlie@example.com');

```
# 📦 One-to-Many Relationship in SQL (MySQL)
## Example: Customers and Orders

---

## 📘 Concept

- **One Customer** can have **many Orders**
- **Each Order** belongs to **one Customer**

---

## 🗺️ ER Diagram (Mermaid)

```mermaid
erDiagram
    CUSTOMERS ||--o{ ORDERS : places

    CUSTOMERS {
        INT id PK
        VARCHAR name
        VARCHAR email
    }

    ORDERS {
        INT id PK
        INT customer_id FK
        DATE order_date
        DECIMAL total_amount
    }
```
