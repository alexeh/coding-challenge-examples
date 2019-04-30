# Software engineer - importer challenge

As part of this exercise, you need to build a small REST API. This API should have two endpoints:

- POST: expects a CSV and saves it to a mongo/elasticsearch database
- GET: reads that same mongo/elasticsearch database and serves the content as a JSON

Each endpoint needs to be implemented as its own standalone application. They will share the underlying data storage, but will not be aware of each other.

Both apps, as well as the underlying dependencies must be configured to run using a `docker-compose` file you must provide. You can use either nodejs, python. Extra kudos will be given if you use both, one per app. 

Document on the code/config files any significant decisions you make as you go (be concise). Tests are a plus.

## Requirements:

- Use your favourite ORM/DB abstraction lib to handle database objects.
- Use a framework - it may be overkill for such small apps, but real-world apps are never this small.
- Document how to start your application in a docker + docker-compose environment. 

There is no need to create a web interface

## Things to keep in mind:

- Be pragmatic and mindful of the trade-off between feature-completeness and complexity/performance.
- In a real world scenario, the data file could be a lot larger.
- Assume a "write once, read many" scenario, where users may be willing to wait a few minutes for the file to be uploaded, depending on its size, but the GET endpoint needs to be fast.
- This code challenge should match your CV. If you have experience with python or node, use that language. If you have experience with both, use this as an opportunity to impress us with your multi-language skills.


## Data

[emissions.csv](data/emissions.csv)
