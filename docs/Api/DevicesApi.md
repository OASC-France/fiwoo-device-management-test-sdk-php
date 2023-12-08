# Swagger\Client\DevicesApi

All URIs are relative to *https://gateway.am.wso2.core.drural-sandbox.eu/devicemanagement/6.2.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createDevice**](DevicesApi.md#createdevice) | **POST** /v1/device | 
[**deleteDevice**](DevicesApi.md#deletedevice) | **DELETE** /v1/device/{id} | 
[**listAllDevices**](DevicesApi.md#listalldevices) | **GET** /v1/device/list/all | 
[**listMineDevices**](DevicesApi.md#listminedevices) | **GET** /v1/device/list/mine | 
[**listPublicDevices**](DevicesApi.md#listpublicdevices) | **GET** /v1/device/list/public | 
[**readDevice**](DevicesApi.md#readdevice) | **GET** /v1/device/{id} | 
[**readPublicDevice**](DevicesApi.md#readpublicdevice) | **GET** /v1/device/{id}/public | 
[**sendCommand**](DevicesApi.md#sendcommand) | **POST** /v1/device/{id}/sendCommand | 
[**sendMultipleCommands**](DevicesApi.md#sendmultiplecommands) | **POST** /v1/device/sendMultipleCommands | 
[**status**](DevicesApi.md#status) | **GET** /v1/device/{id}/status | 
[**updateDevice**](DevicesApi.md#updatedevice) | **PUT** /v1/device/{id} | 

# **createDevice**
> \Swagger\Client\Model\InlineResponse201 createDevice($body, $x_auth_token)



Creates devices

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

$apiInstance = new Swagger\Client\Api\DevicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CreateDeviceAPI(); // \Swagger\Client\Model\CreateDeviceAPI | 
$x_auth_token = "x_auth_token_example"; // string | 

try {
    $result = $apiInstance->createDevice($body, $x_auth_token);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesApi->createDevice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CreateDeviceAPI**](../Model/CreateDeviceAPI.md)|  |
 **x_auth_token** | **string**|  |

### Return type

[**\Swagger\Client\Model\InlineResponse201**](../Model/InlineResponse201.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteDevice**
> deleteDevice($id)



Deletes a Device

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

$apiInstance = new Swagger\Client\Api\DevicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $apiInstance->deleteDevice($id);
} catch (Exception $e) {
    echo 'Exception when calling DevicesApi->deleteDevice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

void (empty response body)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listAllDevices**
> object listAllDevices($x_auth_token, $x_query_page, $x_query_size)



List all devices, based on parameters given

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

$apiInstance = new Swagger\Client\Api\DevicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$x_auth_token = "x_auth_token_example"; // string | 
$x_query_page = 1.2; // double | 
$x_query_size = 1.2; // double | 

try {
    $result = $apiInstance->listAllDevices($x_auth_token, $x_query_page, $x_query_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesApi->listAllDevices: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_auth_token** | **string**|  |
 **x_query_page** | **double**|  | [optional]
 **x_query_size** | **double**|  | [optional]

### Return type

**object**

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listMineDevices**
> \Swagger\Client\Model\InlineResponse200 listMineDevices($x_query_page, $x_query_size)



List devices owned by authenticated user, based on parameters given

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

$apiInstance = new Swagger\Client\Api\DevicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$x_query_page = 1.2; // double | 
$x_query_size = 1.2; // double | 

try {
    $result = $apiInstance->listMineDevices($x_query_page, $x_query_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesApi->listMineDevices: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_query_page** | **double**|  | [optional]
 **x_query_size** | **double**|  | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse200**](../Model/InlineResponse200.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listPublicDevices**
> \Swagger\Client\Model\InlineResponse200 listPublicDevices($x_query_page, $x_query_size)



List devices with policy set to public, based on parameters given

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

$apiInstance = new Swagger\Client\Api\DevicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$x_query_page = 1.2; // double | 
$x_query_size = 1.2; // double | 

try {
    $result = $apiInstance->listPublicDevices($x_query_page, $x_query_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesApi->listPublicDevices: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_query_page** | **double**|  | [optional]
 **x_query_size** | **double**|  | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse200**](../Model/InlineResponse200.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **readDevice**
> object readDevice($id, $x_auth_token)



Get device by its id

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

$apiInstance = new Swagger\Client\Api\DevicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 
$x_auth_token = "x_auth_token_example"; // string | 

try {
    $result = $apiInstance->readDevice($id, $x_auth_token);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesApi->readDevice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |
 **x_auth_token** | **string**|  |

### Return type

**object**

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **readPublicDevice**
> \Swagger\Client\Model\InlineResponse201 readPublicDevice($id)



Get device. Security definition: `Public`

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

$apiInstance = new Swagger\Client\Api\DevicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->readPublicDevice($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesApi->readPublicDevice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\InlineResponse201**](../Model/InlineResponse201.md)

### Authorization

[Public](../../README.md#Public), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sendCommand**
> \Swagger\Client\Model\InlineResponse2001 sendCommand($body, $id)



Send command to device

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

$apiInstance = new Swagger\Client\Api\DevicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\SendCommandDeviceAPI(); // \Swagger\Client\Model\SendCommandDeviceAPI | 
$id = "id_example"; // string | 

try {
    $result = $apiInstance->sendCommand($body, $id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesApi->sendCommand: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\SendCommandDeviceAPI**](../Model/SendCommandDeviceAPI.md)|  |
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\InlineResponse2001**](../Model/InlineResponse2001.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sendMultipleCommands**
> object sendMultipleCommands($body)



Send command to device

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

$apiInstance = new Swagger\Client\Api\DevicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\SendMultipleCommandsToDevicesAPI(); // \Swagger\Client\Model\SendMultipleCommandsToDevicesAPI | 

try {
    $result = $apiInstance->sendMultipleCommands($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesApi->sendMultipleCommands: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\SendMultipleCommandsToDevicesAPI**](../Model/SendMultipleCommandsToDevicesAPI.md)|  |

### Return type

**object**

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **status**
> \Swagger\Client\Model\InlineResponse2001 status($id)



Get device status

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

$apiInstance = new Swagger\Client\Api\DevicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->status($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesApi->status: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\InlineResponse2001**](../Model/InlineResponse2001.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateDevice**
> \Swagger\Client\Model\InlineResponse201 updateDevice($body, $x_auth_token, $id)



Updates a device

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

$apiInstance = new Swagger\Client\Api\DevicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\UpdateDeviceAPI(); // \Swagger\Client\Model\UpdateDeviceAPI | 
$x_auth_token = "x_auth_token_example"; // string | 
$id = "id_example"; // string | 

try {
    $result = $apiInstance->updateDevice($body, $x_auth_token, $id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevicesApi->updateDevice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\UpdateDeviceAPI**](../Model/UpdateDeviceAPI.md)|  |
 **x_auth_token** | **string**|  |
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\InlineResponse201**](../Model/InlineResponse201.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

