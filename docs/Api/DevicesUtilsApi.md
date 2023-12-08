# Swagger\Client\DevicesUtilsApi

All URIs are relative to *https://gateway.am.wso2.core.drural-sandbox.eu/devicemanagement/6.2.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**checkPolygon**](DevicesUtilsApi.md#checkpolygon) | **POST** /v1/device/is/in/polygon | 
[**checkPolygonPublic**](DevicesUtilsApi.md#checkpolygonpublic) | **POST** /v1/device/is/in/polygon/public | 

# **checkPolygon**
> \Swagger\Client\Model\InlineResponse2003 checkPolygon($body)



Check if a device is inside or outside of a given polygon

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: Direct
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-nick-name', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-nick-name', 'Bearer');// Configure API key authorization: Standard
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-auth-token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-auth-token', 'Bearer');
// Configure OAuth2 access token for authorization: default
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\DevicesUtilsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CheckDeviceInPolygonRequestAPI(); // \Swagger\Client\Model\CheckDeviceInPolygonRequestAPI | 

try {
    $result = $apiInstance->checkPolygon($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesUtilsApi->checkPolygon: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CheckDeviceInPolygonRequestAPI**](../Model/CheckDeviceInPolygonRequestAPI.md)|  |

### Return type

[**\Swagger\Client\Model\InlineResponse2003**](../Model/InlineResponse2003.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **checkPolygonPublic**
> \Swagger\Client\Model\InlineResponse2003 checkPolygonPublic($body)



Check if a device is inside or outside of a given polygon

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: Public
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-data-access', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-data-access', 'Bearer');
// Configure OAuth2 access token for authorization: default
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\DevicesUtilsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CheckDeviceInPolygonRequestAPI(); // \Swagger\Client\Model\CheckDeviceInPolygonRequestAPI | 

try {
    $result = $apiInstance->checkPolygonPublic($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesUtilsApi->checkPolygonPublic: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CheckDeviceInPolygonRequestAPI**](../Model/CheckDeviceInPolygonRequestAPI.md)|  |

### Return type

[**\Swagger\Client\Model\InlineResponse2003**](../Model/InlineResponse2003.md)

### Authorization

[Public](../../README.md#Public), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

