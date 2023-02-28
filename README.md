This project is a backend REST service that provides bank details by using the data provided in the API's query parameters. It has been developed using NodeJS, ExpressJS, and MongoDB Atlas. There are three API endpoints that are available in this service.

The first API endpoint is POST api/import-csv. This endpoint allows users to upload the data of a CSV file into MongoDB.

The second API endpoint is GET api/search. This endpoint is used to search for bank details by city name, and it allows users to set a limit and offset for the number of results returned. The results are ordered by IFSC code in ascending order.

The third API endpoint is GET api/branch. This endpoint also searches for bank details by city name, and it allows users to set a limit and offset for the number of results returned. The results are ordered by IFSC code in descending order based on the branch name.

Overall, this service provides a simple and efficient way to retrieve bank details by using various search parameters.



