# Iran & International Vehicle Plate Codes

A simple, clean, and structured JSON collection of Iranian provincial license plates and international vehicle codes. This dataset is designed for easy integration into any development project.

### 1. Iranian Province Codes

This list contains all 31 provinces of Iran. Each province object includes its name in both Persian and English, along with a list of major cities and their specific license plate codes.

**Structure Example:**
```json
{
  "provinces": [
    {
      "province_fa": "آذربایجان شرقی",
      "province_en": "East Azerbaijan",
      "cities": [
        { "city_fa": "تبریز", "city_en": "Tabriz", "code": "15" },
        { "city_fa": "مراغه", "city_en": "Maragheh", "code": "25" }
      ]
    },
    {
      "province_fa": "تهران",
      "province_en": "Tehran",
      "cities": [
        { "city_fa": "تهران", "city_en": "Tehran", "code": "11, 22, 33, 44, 55, 66, 77, 88, 99" }
      ]
    }
  ]
}
```

### 2. International Vehicle Codes

A comprehensive list of international vehicle registration codes (e.g., the oval stickers on cars). Each object contains the country's name in both Persian and English, and its official code.

**Structure Example:**
```json
{
  "international_vehicle_codes": [
    { "country_fa": "ایران", "country_en": "Iran", "code": "IR" },
    { "country_fa": "آلمان", "country_en": "Germany", "code": "D" },
    { "country_fa": "ژاپن", "country_en": "Japan", "code": "J" }
  ]
}
```

## Contributing

Found a mistake, have an update, or want to add more data? Contributions are welcome!

Please feel free to open an issue to report errors or submit a pull request with your changes.

## License

This project is licensed under the **MIT License**. See the `LICENSE` file for details.
