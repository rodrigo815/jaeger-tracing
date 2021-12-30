# jaeger-tracing

1. Install Jaeger client and execute jaeger-all-in-one
2. Install Postman
3. Run fact-service with Spring profile *prod* and variable SPRING_APPLICATION_NAME=fact
4. Run fib-service with Spring profile *prod* and variable SPRING_APPLICATION_NAME=fib
5. Run compute-service with Spring profile *prod* and variable SPRING_APPLICATION_NAME=compute
6. Open Postman and execute GET request localhost:8082/api/compute/fact/10
7. Open Jaeger UI (http://localhost:16686/) and see the request selecting Service "unkown-spring-boot"
