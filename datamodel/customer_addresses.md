|column       | description |
--------------|-------------|
|id           | Primary key - Unique identifier of the address. |
|customer_id  | Foreign key - Unique identifier of the customer. |
|geography_id | Foreign key - Unique identifier of the customer's location. |
|address      | Address that the customer used in an order. |
|is_home      | Boolean value wether the address is the customer's home address. [1,0] |
|created_at   | Timestamp when the address was created. |
|updated_at   | Timestamp when the address was modified. |
|deleted_at   | Timestamp when the address was soft deleted. |
