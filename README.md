# Business On Bot - Backend Task

This project is a backend REST service that provides bank details by using the data provided in the API's query parameters. It has been developed using NodeJS, ExpressJS, and MongoDB Atlas. There are three API endpoints that are available in this service.

I.The first API endpoint is POST api/import-csv. This endpoint allows users to upload the data of a CSV file into MongoDB.

II.The second API endpoint is GET api/search. This endpoint is used to search for bank details by city name, and it allows users to set a limit and offset for the number of results returned. The results are ordered by IFSC code in ascending order.

III.The third API endpoint is GET api/branch. This endpoint also searches for bank details by city name, and it allows users to set a limit and offset for the number of results returned. The results are ordered by IFSC code in descending order based on the branch name.

Overall, this service provides a simple and efficient way to retrieve bank details by using various search parameters.


# Case 1
Search API to return possible matches across all columns and all rows, ordered by IFSC code (ascending order) with limit and offset.


Request URL - /api/search?q=Mumbai&limit=2&offset=1

Image:
![Screenshot 2023-02-28 191407](https://user-images.githubusercontent.com/77921023/221874218-0436caad-341d-4ae1-9ba3-97fa2a78f900.jpg)


# Case 2
Branch API to return possible matches based on the branch name ordered by IFSC code (descending order) with limit and offset

Request URL - /api/branch?q=LONI&limit=1&offset=1

Image:
![Screenshot 2023-02-28 191459](https://user-images.githubusercontent.com/77921023/221874134-5f875a65-01e7-4713-a943-8afb4eecb005.jpg)
