# SwaggerClient-php
No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 0.0.0-development
- Build package: io.swagger.codegen.v3.generators.php.PhpClientCodegen

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/GIT_USER_ID/GIT_REPO_ID.git"
    }
  ],
  "require": {
    "GIT_USER_ID/GIT_REPO_ID": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/SwaggerClient-php/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Direct
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-nick-name', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-nick-name', 'Bearer');
// Configure API key authorization: Standard
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

// Configure API key authorization: Direct
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-nick-name', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-nick-name', 'Bearer');
// Configure API key authorization: Standard
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

// Configure API key authorization: Direct
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-nick-name', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-nick-name', 'Bearer');
// Configure API key authorization: Standard
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

// Configure API key authorization: Direct
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-nick-name', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-nick-name', 'Bearer');
// Configure API key authorization: Standard
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

// Configure API key authorization: Direct
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-nick-name', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-nick-name', 'Bearer');
// Configure API key authorization: Standard
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

// Configure API key authorization: Direct
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-nick-name', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-nick-name', 'Bearer');
// Configure API key authorization: Standard
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

// Configure API key authorization: Direct
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-nick-name', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-nick-name', 'Bearer');
// Configure API key authorization: Standard
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

// Configure API key authorization: Direct
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-nick-name', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-nick-name', 'Bearer');
// Configure API key authorization: Standard
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

// Configure API key authorization: Direct
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-nick-name', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-nick-name', 'Bearer');
// Configure API key authorization: Standard
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

// Configure API key authorization: Direct
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-nick-name', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-nick-name', 'Bearer');
// Configure API key authorization: Standard
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

## Documentation for API Endpoints

All URIs are relative to *https://gateway.am.wso2.core.drural-sandbox.eu/devicemanagement/6.2.1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DevicesApi* | [**createDevice**](docs/Api/DevicesApi.md#createdevice) | **POST** /v1/device | 
*DevicesApi* | [**deleteDevice**](docs/Api/DevicesApi.md#deletedevice) | **DELETE** /v1/device/{id} | 
*DevicesApi* | [**listAllDevices**](docs/Api/DevicesApi.md#listalldevices) | **GET** /v1/device/list/all | 
*DevicesApi* | [**listMineDevices**](docs/Api/DevicesApi.md#listminedevices) | **GET** /v1/device/list/mine | 
*DevicesApi* | [**listPublicDevices**](docs/Api/DevicesApi.md#listpublicdevices) | **GET** /v1/device/list/public | 
*DevicesApi* | [**readDevice**](docs/Api/DevicesApi.md#readdevice) | **GET** /v1/device/{id} | 
*DevicesApi* | [**readPublicDevice**](docs/Api/DevicesApi.md#readpublicdevice) | **GET** /v1/device/{id}/public | 
*DevicesApi* | [**sendCommand**](docs/Api/DevicesApi.md#sendcommand) | **POST** /v1/device/{id}/sendCommand | 
*DevicesApi* | [**sendMultipleCommands**](docs/Api/DevicesApi.md#sendmultiplecommands) | **POST** /v1/device/sendMultipleCommands | 
*DevicesApi* | [**status**](docs/Api/DevicesApi.md#status) | **GET** /v1/device/{id}/status | 
*DevicesApi* | [**updateDevice**](docs/Api/DevicesApi.md#updatedevice) | **PUT** /v1/device/{id} | 
*DevicesAuthApi* | [**createAuthDevice**](docs/Api/DevicesAuthApi.md#createauthdevice) | **POST** /v1/device/{id}/auth | 
*DevicesAuthApi* | [**deleteAllAuthDevices**](docs/Api/DevicesAuthApi.md#deleteallauthdevices) | **DELETE** /v1/device/{id}/auth | 
*DevicesAuthApi* | [**deleteAuthDevice**](docs/Api/DevicesAuthApi.md#deleteauthdevice) | **DELETE** /v1/device/{id}/auth/{authId} | 
*DevicesAuthApi* | [**readAuthDevice**](docs/Api/DevicesAuthApi.md#readauthdevice) | **GET** /v1/device/{id}/auth | 
*DevicesAuthApi* | [**renewDeviceToken**](docs/Api/DevicesAuthApi.md#renewdevicetoken) | **PUT** /v1/device/{id}/auth/{authId}/renew | 
*DevicesUtilsApi* | [**checkPolygon**](docs/Api/DevicesUtilsApi.md#checkpolygon) | **POST** /v1/device/is/in/polygon | 
*DevicesUtilsApi* | [**checkPolygonPublic**](docs/Api/DevicesUtilsApi.md#checkpolygonpublic) | **POST** /v1/device/is/in/polygon/public | 
*ServicesApi* | [**countServices**](docs/Api/ServicesApi.md#countservices) | **GET** /v1/service/{id}/count/devices | 
*ServicesApi* | [**createService**](docs/Api/ServicesApi.md#createservice) | **POST** /v1/service | 
*ServicesApi* | [**deleteService**](docs/Api/ServicesApi.md#deleteservice) | **DELETE** /v1/service/{id} | 
*ServicesApi* | [**listAllServices**](docs/Api/ServicesApi.md#listallservices) | **GET** /v1/service/list/all | 
*ServicesApi* | [**listMineServices**](docs/Api/ServicesApi.md#listmineservices) | **GET** /v1/service/list/mine | 
*ServicesApi* | [**listPublicServices**](docs/Api/ServicesApi.md#listpublicservices) | **GET** /v1/service/list/public | 
*ServicesApi* | [**readService**](docs/Api/ServicesApi.md#readservice) | **GET** /v1/service/{id} | 
*ServicesApi* | [**updateService**](docs/Api/ServicesApi.md#updateservice) | **PUT** /v1/service/{id} | 
*ServicesAuthApi* | [**createAuthService**](docs/Api/ServicesAuthApi.md#createauthservice) | **POST** /v1/service/{id}/auth | 
*ServicesAuthApi* | [**deleteAllAuthServices**](docs/Api/ServicesAuthApi.md#deleteallauthservices) | **DELETE** /v1/service/{id}/auth | 
*ServicesAuthApi* | [**deleteAuthService**](docs/Api/ServicesAuthApi.md#deleteauthservice) | **DELETE** /v1/service/{id}/auth/{authId} | 
*ServicesAuthApi* | [**readAuthService**](docs/Api/ServicesAuthApi.md#readauthservice) | **GET** /v1/service/{id}/auth | 
*ServicesAuthApi* | [**renewServiceToken**](docs/Api/ServicesAuthApi.md#renewservicetoken) | **PUT** /v1/service/{id}/auth/{authId}/renew | 
*TemplatesApi* | [**countDevicesTemplate**](docs/Api/TemplatesApi.md#countdevicestemplate) | **GET** /v1/template/{id}/count/devices | 
*TemplatesApi* | [**createTemplate**](docs/Api/TemplatesApi.md#createtemplate) | **POST** /v1/template | 
*TemplatesApi* | [**deleteTemplate**](docs/Api/TemplatesApi.md#deletetemplate) | **DELETE** /v1/template/{id} | 
*TemplatesApi* | [**listAllTemplates**](docs/Api/TemplatesApi.md#listalltemplates) | **GET** /v1/template/list/all | 
*TemplatesApi* | [**listMineTemplates**](docs/Api/TemplatesApi.md#listminetemplates) | **GET** /v1/template/list/mine | 
*TemplatesApi* | [**listPublicTemplates**](docs/Api/TemplatesApi.md#listpublictemplates) | **GET** /v1/template/list/public | 
*TemplatesApi* | [**readTemplate**](docs/Api/TemplatesApi.md#readtemplate) | **GET** /v1/template/{id} | 
*TemplatesApi* | [**updateTemplate**](docs/Api/TemplatesApi.md#updatetemplate) | **PUT** /v1/template/{id} | 
*UserApi* | [**loginUser**](docs/Api/UserApi.md#loginuser) | **POST** /v1/user/login | 

## Documentation For Models

 - [AnyOfCreateDeviceAPIDataset](docs/Model/AnyOfCreateDeviceAPIDataset.md)
 - [AnyOfCreateDeviceAPIOrganization](docs/Model/AnyOfCreateDeviceAPIOrganization.md)
 - [AnyOfCreateServiceAPIDataset](docs/Model/AnyOfCreateServiceAPIDataset.md)
 - [AnyOfCreateServiceAPIOrganization](docs/Model/AnyOfCreateServiceAPIOrganization.md)
 - [AnyOfCreateTemplateAPIDataset](docs/Model/AnyOfCreateTemplateAPIDataset.md)
 - [AnyOfCreateTemplateAPIOrganization](docs/Model/AnyOfCreateTemplateAPIOrganization.md)
 - [AnyOfDeviceAPIDataset](docs/Model/AnyOfDeviceAPIDataset.md)
 - [AnyOfDeviceAPIId](docs/Model/AnyOfDeviceAPIId.md)
 - [AnyOfDeviceAPIOrganization](docs/Model/AnyOfDeviceAPIOrganization.md)
 - [AnyOfDeviceAPIOwner](docs/Model/AnyOfDeviceAPIOwner.md)
 - [AnyOfDomainIdValue](docs/Model/AnyOfDomainIdValue.md)
 - [AnyOfServiceAPIDataset](docs/Model/AnyOfServiceAPIDataset.md)
 - [AnyOfServiceAPIId](docs/Model/AnyOfServiceAPIId.md)
 - [AnyOfServiceAPIOrganization](docs/Model/AnyOfServiceAPIOrganization.md)
 - [AnyOfServiceAPIOwner](docs/Model/AnyOfServiceAPIOwner.md)
 - [AnyOfTemplateAPIDataset](docs/Model/AnyOfTemplateAPIDataset.md)
 - [AnyOfTemplateAPIId](docs/Model/AnyOfTemplateAPIId.md)
 - [AnyOfTemplateAPIOrganization](docs/Model/AnyOfTemplateAPIOrganization.md)
 - [AnyOfTemplateAPIOwner](docs/Model/AnyOfTemplateAPIOwner.md)
 - [AnyOfUpdateDeviceAPIDataset](docs/Model/AnyOfUpdateDeviceAPIDataset.md)
 - [AnyOfUpdateDeviceAPIOrganization](docs/Model/AnyOfUpdateDeviceAPIOrganization.md)
 - [AnyOfUpdateServiceAPIDataset](docs/Model/AnyOfUpdateServiceAPIDataset.md)
 - [AnyOfUpdateServiceAPIOrganization](docs/Model/AnyOfUpdateServiceAPIOrganization.md)
 - [AnyOfUpdateTemplateAPIDataset](docs/Model/AnyOfUpdateTemplateAPIDataset.md)
 - [AnyOfUpdateTemplateAPIOrganization](docs/Model/AnyOfUpdateTemplateAPIOrganization.md)
 - [AuthenticationAPI](docs/Model/AuthenticationAPI.md)
 - [AvailableCommand](docs/Model/AvailableCommand.md)
 - [CheckDeviceInPolygonRequestAPI](docs/Model/CheckDeviceInPolygonRequestAPI.md)
 - [CheckDeviceInPolygonResponseAPI](docs/Model/CheckDeviceInPolygonResponseAPI.md)
 - [CommandAPI](docs/Model/CommandAPI.md)
 - [CommandAttributeAPI](docs/Model/CommandAttributeAPI.md)
 - [CountResponseAPI](docs/Model/CountResponseAPI.md)
 - [CreateDeviceAPI](docs/Model/CreateDeviceAPI.md)
 - [CreateServiceAPI](docs/Model/CreateServiceAPI.md)
 - [CreateTemplateAPI](docs/Model/CreateTemplateAPI.md)
 - [DeviceAPI](docs/Model/DeviceAPI.md)
 - [DeviceResponseInternalAPI](docs/Model/DeviceResponseInternalAPI.md)
 - [DomainId](docs/Model/DomainId.md)
 - [EntityCategory](docs/Model/EntityCategory.md)
 - [FiwareAPI](docs/Model/FiwareAPI.md)
 - [InlineResponse200](docs/Model/InlineResponse200.md)
 - [InlineResponse2001](docs/Model/InlineResponse2001.md)
 - [InlineResponse2002](docs/Model/InlineResponse2002.md)
 - [InlineResponse2003](docs/Model/InlineResponse2003.md)
 - [InlineResponse2004](docs/Model/InlineResponse2004.md)
 - [InlineResponse2005](docs/Model/InlineResponse2005.md)
 - [InlineResponse201](docs/Model/InlineResponse201.md)
 - [InlineResponse2011](docs/Model/InlineResponse2011.md)
 - [InlineResponse2012](docs/Model/InlineResponse2012.md)
 - [InlineResponse2013](docs/Model/InlineResponse2013.md)
 - [InlineResponse2014](docs/Model/InlineResponse2014.md)
 - [IotProtocol](docs/Model/IotProtocol.md)
 - [IotTransport](docs/Model/IotTransport.md)
 - [KeyAttributeAPI](docs/Model/KeyAttributeAPI.md)
 - [LoginAPI](docs/Model/LoginAPI.md)
 - [MessageError](docs/Model/MessageError.md)
 - [PermissionAPI](docs/Model/PermissionAPI.md)
 - [PolicyAPI](docs/Model/PolicyAPI.md)
 - [SendCommandDeviceAPI](docs/Model/SendCommandDeviceAPI.md)
 - [SendMultipleCommandsToDevicesAPI](docs/Model/SendMultipleCommandsToDevicesAPI.md)
 - [ServiceAPI](docs/Model/ServiceAPI.md)
 - [ServiceResponseInternalAPI](docs/Model/ServiceResponseInternalAPI.md)
 - [StaticAttributeAPI](docs/Model/StaticAttributeAPI.md)
 - [SubscribeAPI](docs/Model/SubscribeAPI.md)
 - [TargetAPI](docs/Model/TargetAPI.md)
 - [TemplateAPI](docs/Model/TemplateAPI.md)
 - [TokenAPI](docs/Model/TokenAPI.md)
 - [UpdateDeviceAPI](docs/Model/UpdateDeviceAPI.md)
 - [UpdateServiceAPI](docs/Model/UpdateServiceAPI.md)
 - [UpdateTemplateAPI](docs/Model/UpdateTemplateAPI.md)
 - [UserTokenResponseAPI](docs/Model/UserTokenResponseAPI.md)
 - [WorldwideAPI](docs/Model/WorldwideAPI.md)

## Documentation For Authorization


## Direct

- **Type**: API key
- **API key parameter name**: x-nick-name
- **Location**: HTTP header

## Public

- **Type**: API key
- **API key parameter name**: x-data-access
- **Location**: HTTP header

## Standard

- **Type**: API key
- **API key parameter name**: x-auth-token
- **Location**: HTTP header

## default

- **Type**: OAuth
- **Flow**: implicit
- **Authorization URL**: https://drural-api-manager.oasc.fr:8243/authorize
- **Scopes**: 


## Author

info@fiwoo.eu

