# CreateDeviceAPI

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | A meaningful name provided by user | 
**description** | **string** | Description about the entity | [optional] 
**organization** | [**AnyOfCreateDeviceAPIOrganization**](AnyOfCreateDeviceAPIOrganization.md) | The Organization id that the device belong to | [optional] 
**dataset** | [**AnyOfCreateDeviceAPIDataset**](AnyOfCreateDeviceAPIDataset.md) | The Dataset id (under some Organization) that the device belong to | [optional] 
**permissions_policy** | [**\Swagger\Client\Model\PolicyAPI**](PolicyAPI.md) |  | 
**fiware** | [**\Swagger\Client\Model\FiwareAPI**](FiwareAPI.md) |  | 
**entity_type** | **string** | The entity type | 
**categories** | [**\Swagger\Client\Model\EntityCategory[]**](EntityCategory.md) | Device&#x27;s Categories | 
**transport** | [**\Swagger\Client\Model\IotTransport**](IotTransport.md) |  | 
**attributes** | [**\Swagger\Client\Model\KeyAttributeAPI[]**](KeyAttributeAPI.md) | Device&#x27;s attributes | 
**lazy_attributes** | [**\Swagger\Client\Model\KeyAttributeAPI[]**](KeyAttributeAPI.md) | Device&#x27;s lazy attributes | 
**command_attributes** | [**\Swagger\Client\Model\CommandAttributeAPI[]**](CommandAttributeAPI.md) | Device&#x27;s command attributes | 
**static_attributes** | [**\Swagger\Client\Model\StaticAttributeAPI[]**](StaticAttributeAPI.md) | Device&#x27;s static attributes | 
**internal_attributes** | [****](.md) | Device&#x27;s internal attributes | 
**protocol** | [**\Swagger\Client\Model\IotProtocol**](IotProtocol.md) |  | 
**template_id** | **string** | The identificator of the template used to create the device | [optional] 
**service_id** | **string** | The identificator of the service that the device belongs to | [optional] 
**device_id** | **string** | The identificator provided by user to identify it when sending data to the platform | 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

