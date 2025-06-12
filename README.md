# Iran, Turkey & International Vehicle Plate Codes

A simple, clean, and structured JSON dataset of Iranian, Turkish provincial license plates, and international vehicle codes. This dataset is designed for easy integration into any development project requiring vehicle code data.

## Features

- **Iran Provinces:** All 31 provinces with Farsi and English names, each with a list of major cities and their specific license plate codes.
- **Turkey Provinces:** All 81 provinces with Turkish and Farsi names and their official plate codes.
- **International Vehicle Codes:** Official oval codes for countries worldwide, with English and Farsi names.

## Data Structure

### 1. Iranian Province Codes (`iran_provinces`)
Each province includes:
- `province_fa`: Farsi name
- `province_en`: English name
- `cities`: Array of objects (`city_fa`, `city_en`, `code`)

**Example:**
```json
{
  "province_fa": "تهران",
  "province_en": "Tehran",
  "cities": [
    { "city_fa": "تهران", "city_en": "Tehran", "code": "11, 22, 33, 44, 55, 66, 77, 88, 99" }
  ]
}
```

### 2. Turkey Province Codes (`turkey_provinces`)
Each entry includes:
- `code`: Numeric code
- `province_tr`: Turkish name
- `province_fa`: Farsi name

**Example:**
```json
{
  "code": "34",
  "province_tr": "İstanbul",
  "province_fa": "استانبول"
}
```

### 3. International Vehicle Codes (`international_vehicle_codes`)
Each entry includes:
- `country_fa`: Farsi name
- `country_en`: English name
- `code`: Official code

**Example:**
```json
{
  "country_fa": "ایران",
  "country_en": "Iran",
  "code": "IR"
}
```

## Usage

You can use this dataset in any language or platform that supports JSON. Here is a sample code in JavaScript and Python:

### JavaScript Example
```js
const data = require('./list-code.json');
console.log(data.iran_provinces[0].province_en); // Output: East Azerbaijan
```

### Python Example
```python
import json

with open('list-code.json', encoding='utf-8') as f:
    data = json.load(f)

print(data['iran_provinces'][0]['province_en'])  # Output: East Azerbaijan
```

## Applications

- Vehicle registration services
- Mobile or web apps showing regional information based on plate codes
- Data analytics and research on regional vehicle statistics

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---
