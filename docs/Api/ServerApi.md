# CryoFallStatisticsApiClient\ServerApi

All URIs are relative to *http://localhost:8071/CryoFallApi/Public/index.php*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getLeaderboardAction**](ServerApi.md#getleaderboardaction) | **GET** /server/{guid}/leaderboard | 
[**getOnlineAction**](ServerApi.md#getonlineaction) | **GET** /server/{guid}/player_online | 

# **getLeaderboardAction**
> \CryoFallStatisticsApiClient\Model\LeaderboardResponse getLeaderboardAction($guid, $from, $to)



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
$from = "from_example"; // string | Filter date from, format: 2004-02-12T15:19:21+00:00
$to = "to_example"; // string | Filter date to, format: 2004-02-12T15:19:21+00:00

try {
    $result = $apiInstance->getLeaderboardAction($guid, $from, $to);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ServerApi->getLeaderboardAction: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **guid** | **string**| The Server GUID |
 **from** | **string**| Filter date from, format: 2004-02-12T15:19:21+00:00 | [optional]
 **to** | **string**| Filter date to, format: 2004-02-12T15:19:21+00:00 | [optional]

### Return type

[**\CryoFallStatisticsApiClient\Model\LeaderboardResponse**](../Model/LeaderboardResponse.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getOnlineAction**
> \CryoFallStatisticsApiClient\Model\PlayerOnlineResponse getOnlineAction($guid)



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

[**\CryoFallStatisticsApiClient\Model\PlayerOnlineResponse**](../Model/PlayerOnlineResponse.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

