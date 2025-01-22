```mermaid

---
title: Nike Store
---

erDiagram
    PRODUCT {
        int productID PK
        string modelName
        string color
        string size
    }

    CUSTOMER {
        int custID PK
        string name
    }

    SALE {
        int txID PK

    }

    INVENTORY {
        int productID PK
        int quantity
        float pricePerUnit
    }

    CUSTOMER ||--o{ SALE : creates
    SALE ||--|{ PRODUCT : contains
    INVENTORY ||--o{ PRODUCT : contains

```
