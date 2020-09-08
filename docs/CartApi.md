# MercantileApi.CartApi

All URIs are relative to *https://mercantile-api.gurleen.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cartCreate**](CartApi.md#cartCreate) | **POST** /cart/ | 
[**cartDelete**](CartApi.md#cartDelete) | **DELETE** /cart/{id}/ | 
[**cartList**](CartApi.md#cartList) | **GET** /cart/ | 
[**cartPartialUpdate**](CartApi.md#cartPartialUpdate) | **PATCH** /cart/{id}/ | 
[**cartRead**](CartApi.md#cartRead) | **GET** /cart/{id}/ | 
[**cartUpdate**](CartApi.md#cartUpdate) | **PUT** /cart/{id}/ | 


<a name="cartCreate"></a>
# **cartCreate**
> CartItem cartCreate(data)



CRUD for CartItems. Creating a cart item means that item is in your \"cart\".

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.CartApi();

var data = new MercantileApi.CartItem(); // CartItem | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.cartCreate(data, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**CartItem**](CartItem.md)|  | 

### Return type

[**CartItem**](CartItem.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="cartDelete"></a>
# **cartDelete**
> cartDelete(id, )



CRUD for CartItems. Creating a cart item means that item is in your \"cart\".

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.CartApi();

var id = "id_example"; // String | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.cartDelete(id, , callback);
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

<a name="cartList"></a>
# **cartList**
> InlineResponse2001 cartList(opts)



CRUD for CartItems. Creating a cart item means that item is in your \"cart\".

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.CartApi();

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
apiInstance.cartList(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Number**| A page number within the paginated result set. | [optional] 

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="cartPartialUpdate"></a>
# **cartPartialUpdate**
> CartItem cartPartialUpdate(id, data)



CRUD for CartItems. Creating a cart item means that item is in your \"cart\".

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.CartApi();

var id = "id_example"; // String | 

var data = new MercantileApi.CartItem(); // CartItem | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.cartPartialUpdate(id, data, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | 
 **data** | [**CartItem**](CartItem.md)|  | 

### Return type

[**CartItem**](CartItem.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="cartRead"></a>
# **cartRead**
> CartItem cartRead(id, )



CRUD for CartItems. Creating a cart item means that item is in your \"cart\".

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.CartApi();

var id = "id_example"; // String | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.cartRead(id, , callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | 

### Return type

[**CartItem**](CartItem.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="cartUpdate"></a>
# **cartUpdate**
> CartItem cartUpdate(id, data)



CRUD for CartItems. Creating a cart item means that item is in your \"cart\".

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.CartApi();

var id = "id_example"; // String | 

var data = new MercantileApi.CartItem(); // CartItem | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.cartUpdate(id, data, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | 
 **data** | [**CartItem**](CartItem.md)|  | 

### Return type

[**CartItem**](CartItem.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

