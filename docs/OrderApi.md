# MercantileApi.OrderApi

All URIs are relative to *https://mercantile-api.gurleen.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**orderConfirm**](OrderApi.md#orderConfirm) | **POST** /order/{id}/confirm/ | 
[**orderCreate**](OrderApi.md#orderCreate) | **POST** /order/ | 
[**orderList**](OrderApi.md#orderList) | **GET** /order/ | 
[**orderRead**](OrderApi.md#orderRead) | **GET** /order/{id}/ | 


<a name="orderConfirm"></a>
# **orderConfirm**
> Order orderConfirm(id, data)



Create, list, and retrieve orders. Per-order actions available.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.OrderApi();

var id = "id_example"; // String | 

var data = new MercantileApi.Order(); // Order | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.orderConfirm(id, data, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | 
 **data** | [**Order**](Order.md)|  | 

### Return type

[**Order**](Order.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="orderCreate"></a>
# **orderCreate**
> Order orderCreate(data)



Create, list, and retrieve orders. Per-order actions available.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.OrderApi();

var data = new MercantileApi.Order(); // Order | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.orderCreate(data, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Order**](Order.md)|  | 

### Return type

[**Order**](Order.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="orderList"></a>
# **orderList**
> InlineResponse2003 orderList(opts)



Create, list, and retrieve orders. Per-order actions available.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.OrderApi();

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
apiInstance.orderList(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Number**| A page number within the paginated result set. | [optional] 

### Return type

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="orderRead"></a>
# **orderRead**
> Order orderRead(id)



Create, list, and retrieve orders. Per-order actions available.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.OrderApi();

var id = "id_example"; // String | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.orderRead(id, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | 

### Return type

[**Order**](Order.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

