# swagger_client.TokenApi

All URIs are relative to *https://apis.wso2.com/oauth2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**token_post**](TokenApi.md#token_post) | **POST** /token | generate access tokens and authorize them


# **token_post**
> AccessToken token_post(grant_type, username=username, password=password, refresh_token=refresh_token, scope=scope)

generate access tokens and authorize them

generate access tokens and authorize them 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure HTTP basic authorization: basicAuth
swagger_client.configuration.username = 'YOUR_USERNAME'
swagger_client.configuration.password = 'YOUR_PASSWORD'

# create an instance of the API class
api_instance = swagger_client.TokenApi()
grant_type = 'grant_type_example' # str | 
username = 'username_example' # str |  (optional)
password = 'password_example' # str |  (optional)
refresh_token = 'refresh_token_example' # str |  (optional)
scope = 'scope_example' # str |  (optional)

try: 
    # generate access tokens and authorize them
    api_response = api_instance.token_post(grant_type, username=username, password=password, refresh_token=refresh_token, scope=scope)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling TokenApi->token_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **grant_type** | **str**|  | 
 **username** | **str**|  | [optional] 
 **password** | **str**|  | [optional] 
 **refresh_token** | **str**|  | [optional] 
 **scope** | **str**|  | [optional] 

### Return type

[**AccessToken**](AccessToken.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

