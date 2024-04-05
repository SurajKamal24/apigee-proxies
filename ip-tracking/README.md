# IP-Tracking Apigee Proxy

The ip-tracking proxy is used to track the details of the IP addresses. It helps in understanding how the proxy request flows through the Apigee environment.

Apigee architecture consists of three layers:

1. Load Balancer: It is the first layer that handles incoming requests and distributes them to maintain a balance.

2. VM Instance Groups (Customer GCP Project): It is the second layer where the requests are sent by the load balancer.

3. Apigee Runtime (Google GCP Project): It is the final layer where the actual processing of requests takes place.

## Implementation on Apigee

The target API for retrieving IP addresses is: https://httpbin.org/ip. This API, configured in this proxy, will return all IP addresses from origin to end.

## Example Requests
![postman](ip-tracking/docs/postman.png)
