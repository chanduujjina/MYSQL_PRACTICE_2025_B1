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
