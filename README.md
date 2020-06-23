# Swagger\Client\DefaultApi

All URIs are relative to *https://virtserver.swaggerhub.com/Roman2410/No-Code-Expert/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getExpert**](DefaultApi.md#getexpert) | **GET** /expert/{id} | Get a Specific Expert Profile
[**listCategories**](DefaultApi.md#listcategories) | **GET** /categories | List Categories
[**listCountries**](DefaultApi.md#listcountries) | **GET** /countries | List Countries
[**listExperts**](DefaultApi.md#listexperts) | **GET** /experts | List Experts

# **getExpert**
> \Swagger\Client\Model\ExpertsItem getExpert($api_key, $id)

Get a Specific Expert Profile

Get a specific Expert profile

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$api_key = "api_key_example"; // string | valid API key
$id = 1.2; // float | ID of an Expert

try {
    $result = $apiInstance->getExpert($api_key, $id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getExpert: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| valid API key |
 **id** | **float**| ID of an Expert |

### Return type

[**\Swagger\Client\Model\ExpertsItem**](../Model/ExpertsItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listCategories**
> \Swagger\Client\Model\CategoryItem[] listCategories($api_key)

List Categories

List categories available in No-Code.expert directory

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$api_key = "api_key_example"; // string | valid API key

try {
    $result = $apiInstance->listCategories($api_key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->listCategories: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| valid API key |

### Return type

[**\Swagger\Client\Model\CategoryItem[]**](../Model/CategoryItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listCountries**
> \Swagger\Client\Model\CountryItem[] listCountries($api_key)

List Countries

List countries available in No-Code.expert directory

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$api_key = "api_key_example"; // string | valid API key

try {
    $result = $apiInstance->listCountries($api_key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->listCountries: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| valid API key |

### Return type

[**\Swagger\Client\Model\CountryItem[]**](../Model/CountryItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listExperts**
> \Swagger\Client\Model\ExpertsItem[] listExperts($api_key, $country_slug, $category_id)

List Experts

List experts within a specific country or category

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$api_key = "api_key_example"; // string | valid API key
$country_slug = "country_slug_example"; // string | Country slug is required to fetch experts within a specific country. Can be combined with category_id
$category_id = 1.2; // float | Category id is required to fetch experts within a specific category. Can be combined with country_slug

try {
    $result = $apiInstance->listExperts($api_key, $country_slug, $category_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->listExperts: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| valid API key |
 **country_slug** | **string**| Country slug is required to fetch experts within a specific country. Can be combined with category_id | [optional]
 **category_id** | **float**| Category id is required to fetch experts within a specific category. Can be combined with country_slug | [optional]

### Return type

[**\Swagger\Client\Model\ExpertsItem[]**](../Model/ExpertsItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

