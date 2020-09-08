# MercantileApi.ApiTokenAuthApi

All URIs are relative to *https://mercantile-api.gurleen.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiTokenAuthCreate**](ApiTokenAuthApi.md#apiTokenAuthCreate) | **POST** /api-token-auth/ | 


<a name="apiTokenAuthCreate"></a>
# **apiTokenAuthCreate**
> apiTokenAuthCreate()





### Example
```javascript
var MercantileApi = require('mercantile_api');
var defaultClient = MercantileApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new MercantileApi.ApiTokenAuthApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.apiTokenAuthCreate(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

