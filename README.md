# Business On Bot - Backend Task
---

- This project is a REST service that can fetch bank details, using the data given in the API’s query parameters.
- It is developed using NodeJS, ExpressJS, MongoDB Atlas
- It has three API endpoints
    1. POST *api/import-csv*
        - Uploads data of CSV file into MongoDB
    2. GET *api/search* (params -> q=*City Name*, limit=*To Limit the number of output*, offset=*To skip offset number of values*)
        - Search API to return possible matches across all columns and all rows, ordered by IFSC code (ascending order) with limit and offset.
        
    3. GET *api/branch* (params -> q=*City Name*, limit=*To Limit the number of output*, offset=*To skip offset number of values*)
        -  Branch API to return possible matches based on the branch name ordered by IFSC code (descending order) with limit and offset


# Output Screenshots
---

## Case 1

Search API to return possible matches across all columns and all rows, ordered by IFSC code (ascending order) with limit and offset.

Request URL  - /api/search?q=Mumbai&limit=2&offset=1 



## Case 2

Branch API to return possible matches based on the branch name ordered by IFSC code (descending order) with limit and offset

Request URL  - /api/branch?q=LONI&limit=1&offset=1 

Request URL - /api/branch?q=LONI&limit=1&offset=0

