# bumbal-barcodeservice-client-api-php
Barcode Shared Service API

This PHP package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: 1.0
- Build package: org.openapitools.codegen.languages.PhpClientCodegen

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
      "url": "https://github.com/bumbal/bumbal-barcodeservice-client-api-php.git"
    }
  ],
  "require": {
    "bumbal/bumbal-barcodeservice-client-api-php": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/bumbal-barcodeservice-client-api-php/vendor/autoload.php');
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

$apiInstance = new BarcodeService\Api\BarcodesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$instance = 'instance_example'; // string | 

try {
    $result = $apiInstance->createBarcode($instance);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BarcodesApi->createBarcode: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *https://barcode-shared-service.bumbal.eu/api/*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*BarcodesApi* | [**createBarcode**](docs/Api/BarcodesApi.md#createbarcode) | **POST** /barcodes/create | Create an unique barcode
*BarcodesApi* | [**showBarcode**](docs/Api/BarcodesApi.md#showbarcode) | **GET** /barcodes/show/{code} | Show the barcode for a code


## Documentation For Models

 - [ApiResponse](docs/Model/ApiResponse.md)
 - [CreateBarcodeResponse](docs/Model/CreateBarcodeResponse.md)
 - [CreateBarcodeResponseData](docs/Model/CreateBarcodeResponseData.md)
 - [ShowBarcodeResponse](docs/Model/ShowBarcodeResponse.md)


## Documentation For Authorization

 All endpoints do not require authorization.


## Author



