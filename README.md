# swagger-java-client

Parking Spot Api REST
- API version: 1.0
  - Build date: 2022-02-25T17:12:46.932Z

API REST for parking spot control.


*Automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen)*


## Requirements

Building the API client library requires:
1. Java 1.7+
2. Maven/Gradle

## Installation

To install the API client library to your local Maven repository, simply execute:

```shell
mvn clean install
```

To deploy it to a remote Maven repository instead, configure the settings of the repository and execute:

```shell
mvn clean deploy
```

Refer to the [OSSRH Guide](http://central.sonatype.org/pages/ossrh-guide.html) for more information.

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
  <groupId>io.swagger</groupId>
  <artifactId>swagger-java-client</artifactId>
  <version>1.0.0</version>
  <scope>compile</scope>
</dependency>
```

### Gradle users

Add this dependency to your project's build file:

```groovy
compile "io.swagger:swagger-java-client:1.0.0"
```

### Others

At first generate the JAR by executing:

```shell
mvn clean package
```

Then manually install the following JARs:

* `target/swagger-java-client-1.0.0.jar`
* `target/lib/*.jar`

## Getting Started

Please follow the [installation](#installation) instruction and execute the following Java code:

```java

import io.swagger.client.*;
import io.swagger.client.auth.*;
import io.swagger.client.model.*;
import io.swagger.client.api.ParkingSpotControllerApi;

import java.io.File;
import java.util.*;

public class ParkingSpotControllerApiExample {

    public static void main(String[] args) {
        
        ParkingSpotControllerApi apiInstance = new ParkingSpotControllerApi();
        UUID id = new UUID(); // UUID | id
        try {
            Object result = apiInstance.deleteParkingSpotByIdUsingDELETE(id);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ParkingSpotControllerApi#deleteParkingSpotByIdUsingDELETE");
            e.printStackTrace();
        }
    }
}

```

## Documentation for API Endpoints

All URIs are relative to *https://localhost:8080*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ParkingSpotControllerApi* | [**deleteParkingSpotByIdUsingDELETE**](docs/ParkingSpotControllerApi.md#deleteParkingSpotByIdUsingDELETE) | **DELETE** /parking-spot/{id} | Delete parking spot by id.
*ParkingSpotControllerApi* | [**getAllParkingSpotUsingGET**](docs/ParkingSpotControllerApi.md#getAllParkingSpotUsingGET) | **GET** /parking-spot | Return all parking spot.
*ParkingSpotControllerApi* | [**getParkingSpotByIdUsingGET**](docs/ParkingSpotControllerApi.md#getParkingSpotByIdUsingGET) | **GET** /parking-spot/{id} | Return a parking spot by id.
*ParkingSpotControllerApi* | [**saveParkingSpotUsingPOST**](docs/ParkingSpotControllerApi.md#saveParkingSpotUsingPOST) | **POST** /parking-spot | Save a parking spot.
*ParkingSpotControllerApi* | [**updateParkingSpotByIdUsingPUT**](docs/ParkingSpotControllerApi.md#updateParkingSpotByIdUsingPUT) | **PUT** /parking-spot/{id} | Update parking spot by id.


## Documentation for Models

 - [ParkingSpotDto](docs/ParkingSpotDto.md)
 - [ParkingSpotModel](docs/ParkingSpotModel.md)


## Documentation for Authorization

All endpoints do not require authorization.
Authentication schemes defined for the API:

## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Author

marcus.quintela@gmail.com
