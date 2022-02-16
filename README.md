# mongodb2xshipper
Ships data from mongodb to any database.

## Pre-conditions
1. Each tenant might have its own user credentials

## CLI methods
1. Test Connection to MongoDB and target database
    1. Read from MongoDB.
    2. Create, Update and Delete record in Target Database.
2. Prefetch data. 
    1. Drop Target Database’s tables.
    2. Pull data from source as a batch/stream.
    3. Push data into target database as a batch/stream.
    4. Allow query to be specified on MongoDB.
    5. Schemas will work similar to cube schema in cube.js
3. Sync Data.
    1. Do not know how to do it yet.
4. Start Shipper.
    1. Get a list of all databases and tables
    2. Configuration will include seed shippers.
    3. An API will have the ability to turn a shipper seed mode on/off
    4. Provide configuration to a shipper that will contact seed node and learn which shipper node will be connecting to which CDC.
    5. Read cube-like schema
    6. Create tables and metadata in target database
    7. Read as batch/stream
    8. Transform data into what needs to be stored in the target database.


