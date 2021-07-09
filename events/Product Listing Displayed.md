# Product Listing Displayed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Product Listing Displayed",
    "listingDisplayed": {
        "listing": [
            {
                "productInfo": {
                    "isBoosted": "<isBoosted>"
                }
            }
        ]
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|isBoosted|integer|Count of times the product was a boosted product at the time a listing was viewed.||||||||
