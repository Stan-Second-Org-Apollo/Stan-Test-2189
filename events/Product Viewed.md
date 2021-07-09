# Product Viewed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Product Viewed",
    "product": [
        {
            "fulfillment": {
                "isBopusOnly": "<isBopusOnly>"
            },
            "productInfo": {
                "isBoosted": "<isBoosted>",
                "productID": "<productID>"
            }
        }
    ]
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|isBoosted|integer|Count of times the product was a boosted product at the time of product view.||||||||
|isBopusOnly|integer|Count of times the user engaged with a product whose only available shipping method was Buy Online Pick Up In Store \(i.e., BOPUS\).||||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
