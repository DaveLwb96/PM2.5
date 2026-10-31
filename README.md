# PM2.5 Dashboard

- Dashboard that displays latest PM2.5 data.
- URL: https://personal-zqhxbmd9.outsystemscloud.com/PM25/Admindashboard?_ts=639289567927532407
<img width="2528" height="1244" alt="image" src="https://github.com/user-attachments/assets/3f75eb30-2295-4a46-9a10-42fc821f22d1" />


## Technology stack

- OutSystems 11
- data.gov.sg REST API
- Git

## Architecture

PM25 (UI)
- Contains dashboard with basic functionalities (search, clear) for data display
- Has dependency on PM25_CS for reusable logic that fetch data via API

PM25_CS (Core services)
- Consume rest API to retrieve PM25 data (https://api-open.data.gov.sg/v2/real-time/api/pm25?date={date})
- Contains reusable logic that calls the API
