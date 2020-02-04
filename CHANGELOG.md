# Changelog

### v2.0.0 (January 3, 2019)
- Fetch `collections`, `products`, `collectionByHandle` and `productByHandle` from the QueryRoot instead of from the Shop object.
- Return `checkoutUserErrors` instead of `userErrors` when present. This will add an extra field called code.
- Expose `checkoutLineItemsReplace` mutation (to replace deprecated `checkoutLineItemsAdd`, `checkoutLineItemsRemove`, and `checkoutLineItemsUpdate` mutations).
- Remove unused fixtures

### v1.11.0 (November 27, 2018)
- Added availableForSale field to Product query fragment
- Removed tags field from Product query fragment
- Add field aliasing to deprecated fields in affected query fragments:
   - availableForSale on VariantFragment
   - countryCode on CheckoutFragment
   - src on CollectionFragment and VariantFragment

### v1.10.0 (November 7, 2018)
- Updates deprecated Storefront API methods used for some checkout mutations.

### v1.9.1 (October 24, 2018)
- Specifies pageInfo for discountApplications connection

### [UNSAFE] v1.9.0 (October 23, 2018)
- Updates schema.json
- Support checkoutDiscountCodeRemove mutation
- Exposes discounts on the checkout Object
- Allows a null checkout response from CheckoutResource.fetch (#563)

### v1.8.0 (August 30, 2018)
- Support checkoutEmailUpdate mutation

### v0.1.3 (March 30, 2016)
- Adds IE9 support for `atob` and `btoa` using polyfills via #52
- Cleans up some deployment noise (#54). Thanks @tessalt

### v0.1.0 (March 22, 2016)
