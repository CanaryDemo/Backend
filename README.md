# Backend
The backend component of the canary demo

## Version Branches
Each branch represents a separate version of the canary demo. The version 1.0 will display a simple website green website, v1.1 will cause a 500 range error and v1.2 will result in  a blue website. This is only used to demonstrate and test canary deployments.

## Endpoints
The API is listening on port ```8000``` by default. The default port can be changed with the ```ROCKET_PORT``` environment variable. 

### Backend
The following endpoints are available:
- GET ```/health/live```: Checks if the application is health
- GET ```/health/startup```: Delays the application ready state

- GET ```/color```: Returns the defined color
- GET ```/load```: Can be used to generate load on the server to observe scaling