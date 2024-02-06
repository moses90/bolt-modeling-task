|column           |description |
|-----------------|------------|
|id               | Primary key - Unique identifier of the order response. |
|order_id         | Foreign key - Unique identifier of the order. |
|activity_id      | Foreign key - Unique identifier of the courier activity. |
|status           | Status of the response. [accepted, declined] |
|responsed_at     | Timestamp when the courier has responded to the dispatched order. |
