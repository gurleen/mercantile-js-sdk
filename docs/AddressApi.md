# MercantileApi.AddressApi

All URIs are relative to *https://mercantile-api.gurleen.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addressCreate**](AddressApi.md#addressCreate) | **POST** /address/ | 
[**addressDelete**](AddressApi.md#addressDelete) | **DELETE** /address/{id}/ | 
[**addressList**](AddressApi.md#addressList) | **GET** /address/ | 
[**addressPartialUpdate**](AddressApi.md#addressPartialUpdate) | **PATCH** /address/{id}/ | 
[**addressRead**](AddressApi.md#addressRead) | **GET** /address/{id}/ | 
[**addressUpdate**](AddressApi.md#addressUpdate) | **PUT** /address/{id}/ | 


<a name="addressCreate"></a>
# **addressCreate**
> Address addressCreate(data)



CRUD for customer addresses.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.AddressApi();

var data = new MercantileApi.Address(); // Address | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.addressCreate(data, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Address**](Address.md)|  | 

### Return type

[**Address**](Address.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="addressDelete"></a>
# **addressDelete**
> addressDelete(id, )



CRUD for customer addresses.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.AddressApi();

var id = "id_example"; // String | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.addressDelete(id, , callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="addressList"></a>
# **addressList**
> InlineResponse200 addressList(opts)



CRUD for customer addresses.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.AddressApi();

var opts = { 
  'page': 56 // Number | A page number within the paginated result set.
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.addressList(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Number**| A page number within the paginated result set. | [optional] 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="addressPartialUpdate"></a>
# **addressPartialUpdate**
> Address addressPartialUpdate(id, data)



CRUD for customer addresses.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.AddressApi();

var id = "id_example"; // String | 

var data = new MercantileApi.Address(); // Address | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.addressPartialUpdate(id, data, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | 
 **data** | [**Address**](Address.md)|  | 

### Return type

[**Address**](Address.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="addressRead"></a>
# **addressRead**
> Address addressRead(id, )



CRUD for customer addresses.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.AddressApi();

var id = "id_example"; // String | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.addressRead(id, , callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | 

### Return type

[**Address**](Address.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="addressUpdate"></a>
# **addressUpdate**
> Address addressUpdate(id, data)



CRUD for customer addresses.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.AddressApi();

var id = "id_example"; // String | 

var data = new MercantileApi.Address(); // Address | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.addressUpdate(id, data, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | 
 **data** | [**Address**](Address.md)|  | 

### Return type

[**Address**](Address.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

