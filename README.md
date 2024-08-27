# eBay Minimum Price Finder
This Google Apps Script fetches the minimum price of a specified item from eBay using the eBay API. The script is designed to be used within Google Sheets, allowing users to input an item name and retrieve the lowest price available on eBay.

## Features
- Fetches minimum price for a specified item
- Handles API responses robustly to prevent errors
- Logs and handles potential issues with API data
- **Similarity Search**: Searches for items with similar names, not just exact matches, ensuring more relevant results.
- **Flexible Pricing**: The script can be easily modified to fetch average or highest prices instead of the minimum.

## Installation
- Open Google Sheets and go to Extensions > Apps Script.
- Copy and paste the getEbayPrice script from this repository into the script editor.
- Save and close the script editor.
- Use the =getEbayPrice("item_name") function in any cell to fetch the minimum price from eBay.

## Customization

### To fetch average or highest price:
- Modify the `sortOrder` parameter in the API request.
- Use `PricePlusShippingHighest` for the highest price and calculate the average by fetching multiple listings.

```
var url = '...&sortOrder=PricePlusShippingLowest';  // Change to PricePlusShippingHighest for highest price
```

## Usage
In your Google Sheets, enter the formula:

```
=getEbayPrice("Nintendo Gameboy")
```

- This will return the minimum price for the item from eBay.
- You can also use a cell reference like `=getEbayPrice(A1)` where A1 contains the item name.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contributions
Contributions are welcome! Please fork this repository, make your changes, and submit a pull request.
