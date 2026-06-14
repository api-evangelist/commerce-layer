# Commerce Layer GraphQL Schema

Commerce Layer is a headless, multi-market commerce API built on a JSON:API-compliant REST surface. This document describes a conceptual GraphQL schema that maps the Commerce Layer data model to GraphQL types, queries, and mutations. Commerce Layer does not currently expose a native GraphQL endpoint; this schema is a faithful translation of the REST resources described at https://docs.commercelayer.io/core/v/api-reference/ and the public OpenAPI specification at https://data.commercelayer.app/schemas/openapi.json.

## Schema Source

- REST API Reference: https://docs.commercelayer.io/core-api-reference/
- OpenAPI Specification: https://data.commercelayer.app/schemas/openapi.json
- Data Model: https://docs.commercelayer.io/data-model/readme
- GitHub Organization: https://github.com/commercelayer

## Design Approach

The schema mirrors Commerce Layer's resource graph. Each JSON:API resource type becomes a GraphQL object type. Relationships become typed fields (single object or list). Enum types capture the allowed values for status, mode, and strategy fields documented in the API reference. Mutations follow a create/update/delete pattern matching the REST endpoints.

## Domain Areas

### Catalog
SKU, SKUOption, Bundle, BundleItem, ShippingCategory, Tag

### Pricing
Price, PriceList, PriceTier, PriceListRule, GiftCard, GiftCardRecipient, SKUList, SKUListItem

### Markets and Organization
Market, Organization, Channel, Merchant, Store

### Inventory
Inventory, InventoryModel, StockItem, StockLocation, StockTransfer, StockReservation, ReservedStock, DeliveryLeadTime, InventoryReturnLocation

### Orders
Order, LineItem, LineItemOption, Adjustment, Bundle, GiftCard, Coupon

### Promotions
PromotionRule, Promotion, PercentageDiscountPromotion, FixedAmountPromotion, FixedPricePromotion, FreeGiftPromotion, FreeShippingPromotion, BuyXPayYPromotion, ExternalPromotion, FlexPromotion, CouponCodesPromotionRule, CustomPromotionRule

### Customers
Customer, CustomerGroup, CustomerAddress, CustomerSubscription, CustomerPaymentSource, InStockSubscription

### Addresses
Address, Geocoder, BingGeocoder, GoogleGeocoder

### Payments
PaymentMethod, PaymentSource, Transaction, Authorization, Capture, Void, Refund, StripePayment, AdyenPayment, BraintreePayment, PaypalPayment, KlarnaPayment, CheckoutComPayment, AxervePayment, SatispayPayment, ExternalGateway, ManualGateway

### Tax
TaxCalculator, TaxCategory, ManualTaxCalculator, AvalaraTaxCalculator, TaxjarCalculator, VertexCalculator, StripeTaxCalculator, ExternalTaxCalculator

### Shipping
ShippingMethod, ShippingZone, ShippingRate, ShippingCategory, CarrierAccount, EasyPostPickup, Package, Parcel, ParcelLineItem, Shipment, ShipmentLineItem

### Returns
Return, ReturnLineItem

### Webhooks and Events
Webhook, Event, EventCallback

### Bulk Operations
Import, Export, Cleanup

### Provisioning
Membership, Role, APICredential, IdentityProvider, Permission

## Types Count

This schema defines 65 named GraphQL types covering all major Commerce Layer resource domains.
