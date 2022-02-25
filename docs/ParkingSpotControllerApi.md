# ParkingSpotControllerApi

All URIs are relative to *https://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteParkingSpotByIdUsingDELETE**](ParkingSpotControllerApi.md#deleteParkingSpotByIdUsingDELETE) | **DELETE** /parking-spot/{id} | Delete parking spot by id.
[**getAllParkingSpotUsingGET**](ParkingSpotControllerApi.md#getAllParkingSpotUsingGET) | **GET** /parking-spot | Return all parking spot.
[**getParkingSpotByIdUsingGET**](ParkingSpotControllerApi.md#getParkingSpotByIdUsingGET) | **GET** /parking-spot/{id} | Return a parking spot by id.
[**saveParkingSpotUsingPOST**](ParkingSpotControllerApi.md#saveParkingSpotUsingPOST) | **POST** /parking-spot | Save a parking spot.
[**updateParkingSpotByIdUsingPUT**](ParkingSpotControllerApi.md#updateParkingSpotByIdUsingPUT) | **PUT** /parking-spot/{id} | Update parking spot by id.


<a name="deleteParkingSpotByIdUsingDELETE"></a>
# **deleteParkingSpotByIdUsingDELETE**
> Object deleteParkingSpotByIdUsingDELETE(id)

Delete parking spot by id.

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.ParkingSpotControllerApi;


ParkingSpotControllerApi apiInstance = new ParkingSpotControllerApi();
UUID id = new UUID(); // UUID | id
try {
    Object result = apiInstance.deleteParkingSpotByIdUsingDELETE(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ParkingSpotControllerApi#deleteParkingSpotByIdUsingDELETE");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)| id |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a name="getAllParkingSpotUsingGET"></a>
# **getAllParkingSpotUsingGET**
> List&lt;ParkingSpotModel&gt; getAllParkingSpotUsingGET()

Return all parking spot.

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.ParkingSpotControllerApi;


ParkingSpotControllerApi apiInstance = new ParkingSpotControllerApi();
try {
    List<ParkingSpotModel> result = apiInstance.getAllParkingSpotUsingGET();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ParkingSpotControllerApi#getAllParkingSpotUsingGET");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List&lt;ParkingSpotModel&gt;**](ParkingSpotModel.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a name="getParkingSpotByIdUsingGET"></a>
# **getParkingSpotByIdUsingGET**
> Object getParkingSpotByIdUsingGET(id)

Return a parking spot by id.

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.ParkingSpotControllerApi;


ParkingSpotControllerApi apiInstance = new ParkingSpotControllerApi();
UUID id = new UUID(); // UUID | id
try {
    Object result = apiInstance.getParkingSpotByIdUsingGET(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ParkingSpotControllerApi#getParkingSpotByIdUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)| id |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a name="saveParkingSpotUsingPOST"></a>
# **saveParkingSpotUsingPOST**
> Object saveParkingSpotUsingPOST(parkingSpotDto)

Save a parking spot.

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.ParkingSpotControllerApi;


ParkingSpotControllerApi apiInstance = new ParkingSpotControllerApi();
ParkingSpotDto parkingSpotDto = new ParkingSpotDto(); // ParkingSpotDto | parkingSpotDto
try {
    Object result = apiInstance.saveParkingSpotUsingPOST(parkingSpotDto);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ParkingSpotControllerApi#saveParkingSpotUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **parkingSpotDto** | [**ParkingSpotDto**](ParkingSpotDto.md)| parkingSpotDto |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="updateParkingSpotByIdUsingPUT"></a>
# **updateParkingSpotByIdUsingPUT**
> Object updateParkingSpotByIdUsingPUT(id, parkingSpotDto)

Update parking spot by id.

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.ParkingSpotControllerApi;


ParkingSpotControllerApi apiInstance = new ParkingSpotControllerApi();
UUID id = new UUID(); // UUID | id
ParkingSpotDto parkingSpotDto = new ParkingSpotDto(); // ParkingSpotDto | parkingSpotDto
try {
    Object result = apiInstance.updateParkingSpotByIdUsingPUT(id, parkingSpotDto);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ParkingSpotControllerApi#updateParkingSpotByIdUsingPUT");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)| id |
 **parkingSpotDto** | [**ParkingSpotDto**](ParkingSpotDto.md)| parkingSpotDto |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

