# Swagger\Client\UserApi

All URIs are relative to *https://gateway.am.wso2.core.drural-sandbox.eu/devicemanagement/6.2.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**loginUser**](UserApi.md#loginuser) | **POST** /v1/user/login | 

# **loginUser**
> \Swagger\Client\Model\InlineResponse2014 loginUser($body)



Performs login for a registered user. Supply the user's credentials (email,password) and recieve a unique authorization token.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: default
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\LoginAPI(); // \Swagger\Client\Model\LoginAPI | 

try {
    $result = $apiInstance->loginUser($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->loginUser: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\LoginAPI**](../Model/LoginAPI.md)|  |

### Return type

[**\Swagger\Client\Model\InlineResponse2014**](../Model/InlineResponse2014.md)

### Authorization

[default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

