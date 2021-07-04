# CryoFallStatisticsApiClient\ServerApi

All URIs are relative to *https://virtserver.swaggerhub.com/Hanisch-IT/CryoFall_Statistics/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getOnlineAction**](ServerApi.md#getonlineaction) | **GET** /server/{guid}/player_online | 

# **getOnlineAction**
> \CryoFallStatisticsApiClient\Model\PlayerOnlineResponse[] getOnlineAction($guid)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: Bearer
    $config = CryoFallStatisticsApiClient\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new CryoFallStatisticsApiClient\Api\ServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$guid = "guid_example"; // string | The Server GUID

try {
    $result = $apiInstance->getOnlineAction($guid);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ServerApi->getOnlineAction: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **guid** | **string**| The Server GUID |

### Return type

[**\CryoFallStatisticsApiClient\Model\PlayerOnlineResponse[]**](../Model/PlayerOnlineResponse.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

