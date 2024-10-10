# countrycoderm

`countrycoderm` is a simple npm package that allows you to retrieve country information like country codes, country names, and ISO country codes. It's useful for developers building applications that need to handle country-based data and internationalization.

## Features

- **Get country code from country name**
- **Get country name from country code**
- **Get country name from ISO country code**

## Installation

You can install the package via npm:

```bash
npm install countrycoderm
```

## Usage
After installing the package, you can import and use the following functions:

1. ```getCountryCodeFromName(countryName)```
Description: Retrieve the country code for a given country name.
Parameters: ```countryName (string)``` - The name of the country.
Returns: Country code(s) (string or array of strings) or ```undefined``` if the country is not found.
Example:
```bash 
const { getCountryCodeFromName } = require('countrycoderm');
console.log(getCountryCodeFromName('Mauritius'));  // Output: ['230']

```
2. ```getCountryNameFromCode(code)```
Description: Retrieve the country name for a given country code.
Parameters: ```code (string)``` - The country code (e.g., "91" for India).
Returns: Country name (string) or ```undefined``` if the country code is not found.
Example:
```bash
const { getCountryNameFromCode } = require('countrycoderm');
console.log(getCountryNameFromCode('91'));  // Output: 'India'
```
3. ```getCountryNameFromISO(isoCode)```
Description: Retrieve the country name for a given ISO country code.
Parameters: ```isoCode (string)``` - The ISO code of the country (e.g., "IN" for India).
Returns: Country name (string) or ```undefined``` if the ISO code is not found.
Example:
```bash
const { getCountryNameFromISO } = require('countrycoderm');
console.log(getCountryNameFromISO('IN'));  // Output: 'India'
```

## License
This project is licensed under the MIT License - see the LICENSE file for details.
