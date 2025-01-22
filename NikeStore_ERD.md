```mermaid
---
title: Nike Store
---
erDiagram

    CUSTOMER {
        string name
        int custID
    }

    PRODUCT {
    }

    SALE {
    }

    INVENTORY {
    }

    CUSTOMER ||--o{ SALE : creates
    CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
    SALE ||--|{ PRODUCT : contains
    INVENTORY ||--o{ PRODUCT : contains
```
