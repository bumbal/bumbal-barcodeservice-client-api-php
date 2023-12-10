# BarcodeService\BarcodesApi

All URIs are relative to https://barcode-shared-service.bumbal.eu/api, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createBarcode()**](BarcodesApi.md#createBarcode) | **POST** /barcodes/create | Create an unique barcode |
| [**showBarcode()**](BarcodesApi.md#showBarcode) | **GET** /barcodes/show/{code} | Show the barcode for a code |


## `createBarcode()`

```php
createBarcode($instance): \BarcodeService\Model\CreateBarcodeResponse
```

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
$instance = stage; // string

try {
    $result = $apiInstance->createBarcode($instance);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BarcodesApi->createBarcode: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **instance** | **string**|  | |

### Return type

[**\BarcodeService\Model\CreateBarcodeResponse**](../Model/CreateBarcodeResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `showBarcode()`

```php
showBarcode($code, $accept): \BarcodeService\Model\ShowBarcodeResponse
```

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
$code = bumbal-instance-unixTimestamp-1; // string
$accept = 'accept_example'; // string

try {
    $result = $apiInstance->showBarcode($code, $accept);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BarcodesApi->showBarcode: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **code** | **string**|  | |
| **accept** | **string**|  | |

### Return type

[**\BarcodeService\Model\ShowBarcodeResponse**](../Model/ShowBarcodeResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
