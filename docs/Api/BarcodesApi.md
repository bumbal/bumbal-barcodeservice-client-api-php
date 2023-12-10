# BarcodeService\BarcodesApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createBarcode**](BarcodesApi.md#createBarcode) | **POST** /barcodes/create | Create an unique barcode
[**showBarcode**](BarcodesApi.md#showBarcode) | **GET** /barcodes/show/{code} | Show the barcode for a code


# **createBarcode**
> createBarcode($instance)

Create an unique barcode

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new BarcodeService\Api\BarcodesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$instance = new \stdClass; // object | 

try {
    $apiInstance->createBarcode($instance);
} catch (Exception $e) {
    echo 'Exception when calling BarcodesApi->createBarcode: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **instance** | [**object**](../Model/.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **showBarcode**
> showBarcode($code, $accept)

Show the barcode for a code

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new BarcodeService\Api\BarcodesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$code = new \stdClass; // object | 
$accept = new \stdClass; // object | 

try {
    $apiInstance->showBarcode($code, $accept);
} catch (Exception $e) {
    echo 'Exception when calling BarcodesApi->showBarcode: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **code** | [**object**](../Model/.md)|  |
 **accept** | [**object**](../Model/.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

