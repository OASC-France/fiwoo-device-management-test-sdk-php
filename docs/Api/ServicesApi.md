# Swagger\Client\ServicesApi

All URIs are relative to *https://drural-api-manager.oasc.fr:8243/fiwoo-device-management/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**countServices**](ServicesApi.md#countservices) | **GET** /v1/service/{id}/count/devices | 
[**createService**](ServicesApi.md#createservice) | **POST** /v1/service | 
[**deleteService**](ServicesApi.md#deleteservice) | **DELETE** /v1/service/{id} | 
[**listAllServices**](ServicesApi.md#listallservices) | **GET** /v1/service/list/all | 
[**listMineServices**](ServicesApi.md#listmineservices) | **GET** /v1/service/list/mine | 
[**listPublicServices**](ServicesApi.md#listpublicservices) | **GET** /v1/service/list/public | 
[**readService**](ServicesApi.md#readservice) | **GET** /v1/service/{id} | 
[**updateService**](ServicesApi.md#updateservice) | **PUT** /v1/service/{id} | 

# **countServices**
> \Swagger\Client\Model\CountResponseAPI countServices($id)



Count devices belonging to a service

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

$apiInstance = new Swagger\Client\Api\ServicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->countServices($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ServicesApi->countServices: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\CountResponseAPI**](../Model/CountResponseAPI.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createService**
> \Swagger\Client\Model\InlineResponse2012 createService($body)



Creates services

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

$apiInstance = new Swagger\Client\Api\ServicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CreateServiceAPI(); // \Swagger\Client\Model\CreateServiceAPI | 

try {
    $result = $apiInstance->createService($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ServicesApi->createService: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CreateServiceAPI**](../Model/CreateServiceAPI.md)|  |

### Return type

[**\Swagger\Client\Model\InlineResponse2012**](../Model/InlineResponse2012.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteService**
> deleteService($id)



Deletes a service

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

$apiInstance = new Swagger\Client\Api\ServicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $apiInstance->deleteService($id);
} catch (Exception $e) {
    echo 'Exception when calling ServicesApi->deleteService: ', $e->getMessage(), PHP_EOL;
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

# **listAllServices**
> \Swagger\Client\Model\InlineResponse2004 listAllServices($x_query_page, $x_query_size)



List all services, based on parameters given

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

$apiInstance = new Swagger\Client\Api\ServicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$x_query_page = 1.2; // double | 
$x_query_size = 1.2; // double | 

try {
    $result = $apiInstance->listAllServices($x_query_page, $x_query_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ServicesApi->listAllServices: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_query_page** | **double**|  | [optional]
 **x_query_size** | **double**|  | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2004**](../Model/InlineResponse2004.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listMineServices**
> \Swagger\Client\Model\InlineResponse2004 listMineServices($x_query_page, $x_query_size)



List services owned by authenticated user, based on parameters given

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

$apiInstance = new Swagger\Client\Api\ServicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$x_query_page = 1.2; // double | 
$x_query_size = 1.2; // double | 

try {
    $result = $apiInstance->listMineServices($x_query_page, $x_query_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ServicesApi->listMineServices: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_query_page** | **double**|  | [optional]
 **x_query_size** | **double**|  | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2004**](../Model/InlineResponse2004.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listPublicServices**
> \Swagger\Client\Model\InlineResponse2004 listPublicServices($x_query_page, $x_query_size)



List services with policy set to public, based on parameters given

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

$apiInstance = new Swagger\Client\Api\ServicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$x_query_page = 1.2; // double | 
$x_query_size = 1.2; // double | 

try {
    $result = $apiInstance->listPublicServices($x_query_page, $x_query_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ServicesApi->listPublicServices: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_query_page** | **double**|  | [optional]
 **x_query_size** | **double**|  | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2004**](../Model/InlineResponse2004.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **readService**
> \Swagger\Client\Model\InlineResponse2012 readService($id)



Get service by its id

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

$apiInstance = new Swagger\Client\Api\ServicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->readService($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ServicesApi->readService: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\InlineResponse2012**](../Model/InlineResponse2012.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateService**
> \Swagger\Client\Model\InlineResponse2012 updateService($body, $id)



Updates a service

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

$apiInstance = new Swagger\Client\Api\ServicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\UpdateServiceAPI(); // \Swagger\Client\Model\UpdateServiceAPI | 
$id = "id_example"; // string | 

try {
    $result = $apiInstance->updateService($body, $id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ServicesApi->updateService: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\UpdateServiceAPI**](../Model/UpdateServiceAPI.md)|  |
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\InlineResponse2012**](../Model/InlineResponse2012.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

