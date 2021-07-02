# Location Listing Displayed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData879 = window.appEventData879 || [];
appEventData879.push({
  "event": "Location Listing Displayed",
    "listingDisplayed": {
        "filterListLength": "<filterListLength>",
        "listingContext": "<listingContext>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|filterListLength|integer|The number of filterValue pairs in the filterList|0, 20, 12||||0|||
|listingContext|string|Describes the context of a listing display \(sort changed, filter added, filter removed\)|Filter Added, Filter Removed, Sort Change, Pagination|||||||
