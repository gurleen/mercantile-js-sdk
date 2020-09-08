# MercantileApi.ProductApi

All URIs are relative to *https://mercantile-api.gurleen.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**productList**](ProductApi.md#productList) | **GET** /product/ | 
[**productRead**](ProductApi.md#productRead) | **GET** /product/{id}/ | 


<a name="productList"></a>
# **productList**
> InlineResponse2004 productList(opts)



List and filter all available products.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.ProductApi();

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
apiInstance.productList(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Number**| A page number within the paginated result set. | [optional] 

### Return type

[**InlineResponse2004**](InlineResponse2004.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="productRead"></a>
# **productRead**
> Product productRead(id)



List and filter all available products.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.ProductApi();

var id = 56; // Number | A unique integer value identifying this product.


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.productRead(id, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Number**| A unique integer value identifying this product. | 

### Return type

[**Product**](Product.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

