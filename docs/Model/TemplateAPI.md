# TemplateAPI

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | [**AnyOfTemplateAPIId**](AnyOfTemplateAPIId.md) | The identificator given to the entity entity in the platform | 
**name** | **string** | A meaningful name provided by user | 
**description** | **string** | Description about the entity | [optional] 
**organization** | [**AnyOfTemplateAPIOrganization**](AnyOfTemplateAPIOrganization.md) | The Organization id that the device belong to | [optional] 
**dataset** | [**AnyOfTemplateAPIDataset**](AnyOfTemplateAPIDataset.md) | The Dataset id (under some Organization) that the device belong to | [optional] 
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
**owner** | [**AnyOfTemplateAPIOwner**](AnyOfTemplateAPIOwner.md) | The entity&#x27;s owner | [optional] 
**created_at** | [**\DateTime**](\DateTime.md) | Entity creation date | [optional] 
**updated_at** | [**\DateTime**](\DateTime.md) | Last entity modification date | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

