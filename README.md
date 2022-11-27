
# Availability Zone based Redirecting

The current project contains 2 Availability zones and each Availability zone has api-gateway, service discovery server and application servers. Each API gateway serves using it's zone elements and if element not available then from another zone.

## API Reference

#### From Availability Zone-1

```http
  GET localhost:8090/simple-service/zone :- returns string with Availability zone name
```

#### From Availability Zone-2

```http
  GET localhost:8091/simple-service/zone :- returns string with Availability zone name
```


## System Design

![App Screenshot](https://i.ibb.co/Pz1kHsf/availabilty-zone-system-design.jpg)
