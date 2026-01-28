# CSC3916 Assignment 2 - Movies API

## Description
A Node.js REST API with authentication (Basic Auth and JWT) for movie operations.

## Deployed URL
https://csc3916-assignment2-y36h.onrender.com

## Postman Collection
[<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://app.getpostman.com/run-collection/41547135-aac3d823-5e1a-49d2-8add-f30bf660df90?action=collection%2Ffork&source=rip_markdown&collection-url=entityId%3D41547135-aac3d823-5e1a-49d2-8add-f30bf660df90%26entityType%3Dcollection%26workspaceId%3D3e7cea0b-9a30-4ea3-82f9-47cf84cc6f0d#?env%5BCho%20-%20HW2%5D=W3sia2V5IjoidXJsIiwidmFsdWUiOiJodHRwczovL2NzYzM5MTYtYXNzaWdubWVudDIteTM2aC5vbnJlbmRlci5jb20iLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6Imh0dHBzOi8vY3NjMzkxNi1hc3NpZ25tZW50Mi15MzZoLm9ucmVuZGVyLmNvbSIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiaHR0cHM6Ly9jc2MzOTE2LWFzc2lnbm1lbnQyLXkzNmgub25yZW5kZXIuY29tIiwic2Vzc2lvbkluZGV4IjowfSx7ImtleSI6InRva2VuIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IkpXVC4uLiIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiSldUIGV5SmhiR2NpT2lKSVV6STFOaUlzSW5SNWNDSTZJa3BYVkNKOS5leUpwWkNJNklqVTBOMll3T0Rrd1ltWXlNRFU1T1dRMk9UTm1PRFU0WkRWbE56UmlOelkxWlRJME1ERmtPR1FpTENKMWMyVnlibUZ0WlNJNkluUmxjM1IxYzJWeUlpd2lhV0YwSWpveE56WTVOak01TURBeGZRLmdIZ3hRVGowc3FnQTdEYUJhaFJjZHdDblRlNHUzTGRYMzM5eUtzTEktVVEiLCJzZXNzaW9uSW5kZXgiOjF9XQ==)

## How to Test
After importing the collection, select the "Cho - HW2" environment and run the requests in this order:

1. **POST signup** - Creates a new user
2. **POST signin** - Logs in and saves the JWT token to the environment
3. **PUT movies (JWT)** - Uses the saved token for authentication
4. Other requests can be run in any order

**Note:** DELETE movies uses Basic Auth with credentials already saved in the request.

## Endpoints
- POST /signup - Create a new user
- POST /signin - Login and receive JWT token
- GET /movies - Get movies (no auth)
- POST /movies - Save a movie (no auth)
- PUT /movies - Update a movie (JWT auth required)
- DELETE /movies - Delete a movie (Basic Auth required)