# Event Listing Displayed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData879 = window.appEventData879 || [];
appEventData879.push({
  "event": "Event Listing Displayed",
    "listingDisplayed": {
        "filterListLength": "<filterListLength>",
        "listing": [
            {
                "price": {
                    "pointRangeHigh": "<pointRangeHigh>",
                    "pointRangeLow": "<pointRangeLow>",
                    "priceRangeHigh": "<priceRangeHigh>",
                    "priceRangeLow": "<priceRangeLow>"
                }
            }
        ],
        "listingType": "<listingType>",
        "resultsCount": "<resultsCount>",
        "sortOrder": "<sortOrder>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|filterListLength|integer|The number of filterValue pairs in the filterList|0, 20, 12||||0|||
|listingType|string|The type of results being listed|text, product, location, event, room, product location|||||||
|pointRangeHigh|integer|Upper end of the point range shown.|5000, 2520, 3200|||||||
|pointRangeLow|integer|Lower end of the point range shown.|1000, 1510, 1800|||||||
|priceRangeHigh|string|String representation of the upper end of the price range shown.||^[0-9]*(\.[0-9]{1,2})?$||||||
|priceRangeLow|string|String representation of the lower end of the price range shown.||^[0-9]*(\.[0-9]{1,2})?$||||||
|resultsCount|integer|The total number of items returned that matched the search criteria. \(Integer\)|1, 21, 111, 166||||0|||
|sortOrder|string|Indicates the sort order.|high-low, low-high, nearest-farthest, a-z, newest-oldest|||||||
