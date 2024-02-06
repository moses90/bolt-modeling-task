| Column             | Description |
|--------------------|-------------|
|id                  | Primary key - Unique identifier of the orders. |
|customer_id         | Foreign key - Unique identifier of a customer who made the order. |
|customer_address_id | Foreign key - Unique identifier of the address of the delivery. |
|restaurant_id       | Foreign key - Unique identifier of a restaurant where the order was made from. |
|description         | Details of the order. |
|status              | Status of the order. [In preparation, At courier, Delivered, Cancalled] |
|payment_method      | Way of the payment. [Cash, Card in app, Card at courier] |
|price               | Total price of the order. |
|delivery_fee        | Total fee of the delivery. |
|tip                 | Tip the customer can give to the courier. (Optional) |
|ordered_at          | Timestamp when the order was made. |
|accepted_at         | Timestamp when the order was accepted by the courier. |
|pickedup_at         | Timestamp when the order was picked up by the courier at the restaurant. |
|delivered_at        | Timestamp when the order was successfully delivered to the customer. |
|canceled_at         | Timestamp when the order was cancelled by the customer. |
