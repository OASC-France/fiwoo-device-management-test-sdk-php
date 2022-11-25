# Swagger\Client\TemplatesApi

All URIs are relative to *https://drural-api-manager.oasc.fr:8243/fiwoo-device-management/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**countDevicesTemplate**](TemplatesApi.md#countdevicestemplate) | **GET** /v1/template/{id}/count/devices | 
[**createTemplate**](TemplatesApi.md#createtemplate) | **POST** /v1/template | 
[**deleteTemplate**](TemplatesApi.md#deletetemplate) | **DELETE** /v1/template/{id} | 
[**listAllTemplates**](TemplatesApi.md#listalltemplates) | **GET** /v1/template/list/all | 
[**listMineTemplates**](TemplatesApi.md#listminetemplates) | **GET** /v1/template/list/mine | 
[**listPublicTemplates**](TemplatesApi.md#listpublictemplates) | **GET** /v1/template/list/public | 
[**readTemplate**](TemplatesApi.md#readtemplate) | **GET** /v1/template/{id} | 
[**updateTemplate**](TemplatesApi.md#updatetemplate) | **PUT** /v1/template/{id} | 

# **countDevicesTemplate**
> \Swagger\Client\Model\CountResponseAPI countDevicesTemplate($id)



Count devices created from a template

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

$apiInstance = new Swagger\Client\Api\TemplatesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->countDevicesTemplate($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TemplatesApi->countDevicesTemplate: ', $e->getMessage(), PHP_EOL;
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

# **createTemplate**
> \Swagger\Client\Model\InlineResponse2013 createTemplate($body)



Creates templates

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

$apiInstance = new Swagger\Client\Api\TemplatesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CreateTemplateAPI(); // \Swagger\Client\Model\CreateTemplateAPI | 

try {
    $result = $apiInstance->createTemplate($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TemplatesApi->createTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CreateTemplateAPI**](../Model/CreateTemplateAPI.md)|  |

### Return type

[**\Swagger\Client\Model\InlineResponse2013**](../Model/InlineResponse2013.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteTemplate**
> deleteTemplate($id)



Deletes a template

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

$apiInstance = new Swagger\Client\Api\TemplatesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $apiInstance->deleteTemplate($id);
} catch (Exception $e) {
    echo 'Exception when calling TemplatesApi->deleteTemplate: ', $e->getMessage(), PHP_EOL;
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

# **listAllTemplates**
> \Swagger\Client\Model\InlineResponse2005 listAllTemplates($x_query_page, $x_query_size)



List all templates, based on parameters given

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

$apiInstance = new Swagger\Client\Api\TemplatesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$x_query_page = 1.2; // double | 
$x_query_size = 1.2; // double | 

try {
    $result = $apiInstance->listAllTemplates($x_query_page, $x_query_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TemplatesApi->listAllTemplates: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_query_page** | **double**|  | [optional]
 **x_query_size** | **double**|  | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2005**](../Model/InlineResponse2005.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listMineTemplates**
> \Swagger\Client\Model\InlineResponse2005 listMineTemplates($x_query_page, $x_query_size)



List templates owned by authenticated user, based on parameters given

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

$apiInstance = new Swagger\Client\Api\TemplatesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$x_query_page = 1.2; // double | 
$x_query_size = 1.2; // double | 

try {
    $result = $apiInstance->listMineTemplates($x_query_page, $x_query_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TemplatesApi->listMineTemplates: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_query_page** | **double**|  | [optional]
 **x_query_size** | **double**|  | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2005**](../Model/InlineResponse2005.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listPublicTemplates**
> \Swagger\Client\Model\InlineResponse2005 listPublicTemplates($x_query_page, $x_query_size)



List templates with policy set to public, based on parameters given

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

$apiInstance = new Swagger\Client\Api\TemplatesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$x_query_page = 1.2; // double | 
$x_query_size = 1.2; // double | 

try {
    $result = $apiInstance->listPublicTemplates($x_query_page, $x_query_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TemplatesApi->listPublicTemplates: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_query_page** | **double**|  | [optional]
 **x_query_size** | **double**|  | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2005**](../Model/InlineResponse2005.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **readTemplate**
> \Swagger\Client\Model\InlineResponse2013 readTemplate($id)



Get template by its id

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

$apiInstance = new Swagger\Client\Api\TemplatesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->readTemplate($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TemplatesApi->readTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\InlineResponse2013**](../Model/InlineResponse2013.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateTemplate**
> \Swagger\Client\Model\InlineResponse2013 updateTemplate($body, $id)



Updates a template

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

$apiInstance = new Swagger\Client\Api\TemplatesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\UpdateTemplateAPI(); // \Swagger\Client\Model\UpdateTemplateAPI | 
$id = "id_example"; // string | 

try {
    $result = $apiInstance->updateTemplate($body, $id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TemplatesApi->updateTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\UpdateTemplateAPI**](../Model/UpdateTemplateAPI.md)|  |
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\InlineResponse2013**](../Model/InlineResponse2013.md)

### Authorization

[Direct](../../README.md#Direct), [Standard](../../README.md#Standard), [default](../../README.md#default)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

