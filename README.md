## Courier Datamodel

### The Datamodel
You can find the ER diagram and the description of each model in the [datamodel] folder.

### Infrastructure
A diagram image is also provided in root folder called *infrastructure_diagram.svg*. 
In this recommendation/assumption: 
- The main data source is a PostgreSQL database, this acts as the backend transactional database of the application.
- The extraction and loading job is written in Python.
- Our data warehouse is Bigquery.
- Within Bigquery we perform the data modeling and transformations using dbt.
- The presentation layer is connected to Looker, other ML applications/notebooks and our reverse ETL process is loading the analytics back to the source database. (So it is available to the couriers within the app.)
- Python scripts and dbt is orchestrated with Mage.

### Data Marts
Complexities and obstacles:
- translating business needs and defining the metrics to be as relevant as possible for the company would require extra care (e.g. what is an active user?)
- data storage and transformation performance is crucial. aggregations on millions of rows would need proper indexing and other performance optimization techniques 
- how much latency is okay with the metrics? which metrics should be real-time (or near real-time) and which shouldn't?
- in case of some of personal and sensitive informations, security measures need to be considered to be complient with GDPR and other regulations
