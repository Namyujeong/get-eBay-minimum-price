# eBay Minimum Price Finder
This Google Apps Script fetches the minimum price of a specified item from eBay using the eBay API. The script is designed to be used within Google Sheets, allowing users to input an item name and retrieve the lowest price available on eBay.

## Features
Fetches minimum price for a specified item
Handles API responses robustly to prevent errors
Logs and handles potential issues with API data

## Installation
Open Google Sheets and go to Extensions > Apps Script.
Copy and paste the getEbayPrice script from this repository into the script editor.
Save and close the script editor.
Use the =getEbayPrice("item_name") function in any cell to fetch the minimum price from eBay.

## Usage
In your Google Sheets, enter the formula:

```
=getEbayPrice("Nintendo Gameboy")
This will return the minimum price for the item from eBay.
```

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contributions
Contributions are welcome! Please fork this repository, make your changes, and submit a pull request.
