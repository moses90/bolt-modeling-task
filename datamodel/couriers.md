|column            |description |
|------------------|------------|
|id                | Primary key - Unique identifier of the courier. |
|courier_fleet_id  | Foreign key - Unique identifier of the courier fleet. |
|geography_id      | Foreign key - Unique identifier of the courier's current location. |
|bank_account_id   | Foreign key - Unique identifier of the courier's bank account. |
|name              | Name of the courier. |
|delivery_type     | Way of delivery. [car, scooter, bike, other] |
|created_at        | Timestamp when the courier's account was first created. |
|updated_at        | Timestamp when the courier's record was modified. |
|deleted_at        | Timestamp when the courier's account was soft deleted. |
