# Sample Spring Cloud Gateway with load balancing

This project demonstrates the use of the new [Spring Cloud Gateway](https://spring.io/projects/spring-cloud-gateway).

As a minor step further I enabled the load balancing feature when this service is connected to a service registry such as Eureka or Consul. So instead of the usual http://remote.service.com, it uses the format lb://service-in-registry.

This project assumes you have a configured and running service registry. It can start up but will keep searching for a running registry.

I have included configurations application.properties and application.yml.backup for whatever both use cases. I have enabled the properties file by default because it was tricky for developers using this approach when configuring CORS, which is not so clearly documented in SC Gateway of this writing.