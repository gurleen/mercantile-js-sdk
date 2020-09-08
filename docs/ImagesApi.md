# MercantileApi.ImagesApi

All URIs are relative to *https://mercantile-api.gurleen.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**imagesList**](ImagesApi.md#imagesList) | **GET** /images/ | 
[**imagesRead**](ImagesApi.md#imagesRead) | **GET** /images/{id}/ | 


<a name="imagesList"></a>
# **imagesList**
> InlineResponse2002 imagesList(opts)



List and filter all available product images.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.ImagesApi();

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
apiInstance.imagesList(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Number**| A page number within the paginated result set. | [optional] 

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="imagesRead"></a>
# **imagesRead**
> ProductImage imagesRead(id)



List and filter all available product images.

### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.ImagesApi();

var id = 56; // Number | A unique integer value identifying this product image.


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.imagesRead(id, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Number**| A unique integer value identifying this product image. | 

### Return type

[**ProductImage**](ProductImage.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

