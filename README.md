# Commerce Layer (commerce-layer)

Commerce Layer is the headless, multi-market commerce API used by global brands to sell everywhere — web, mobile, in-store, chatbot, AI agent, and IoT. The company exposes a JSON:API-compliant Core API with 130+ top-level resources covering orders, line items, SKUs, bundles, prices, markets, stores, inventory, customers, payments (Adyen, Stripe, Braintree, PayPal, Klarna, Checkout.com), tax calculation (Avalara, TaxJar, Vertex, Stripe Tax), shipping, promotions, subscriptions, returns, and webhooks. The platform also ships a Provisioning API for organizations/SSO/credentials and a Metrics API for analytics (with a local MCP server for AI agents), plus hosted micro-frontends, dashboard apps, a CLI, CMS integrations, and SDKs for JavaScript/TypeScript, Ruby, React, and drop-in.js.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/commerce-layer/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/commerce-layer/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Headless Commerce
- Composable Commerce
- API-First
- Ecommerce
- JSON:API
- OAuth 2.0
- Multi-Market
- Multi-Currency
- B2C
- B2B
- Subscriptions
- Promotions
- Inventory
- Order Management
- Checkout

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Commerce Layer Core API

The Commerce Layer Core API is the JSON:API-compliant REST API that powers headless commerce. It exposes 130+ top-level resources covering orders, line items, SKUs, bundles, prices, price lists, markets, stores, inventory (stock items, locations, transfers), customers, customer groups, customer subscriptions, payment gateways (Adyen, Stripe, Braintree, PayPal, Klarna, Checkout.com, Axerve, Satispay), payment methods, tax calculators (Avalara, TaxJar, Vertex, Stripe Tax), shipping methods, shipping zones, carrier accounts, geocoders (Google, Bing), promotions (fixed amount, percentage, free gift, free shipping, BXGY, flex), gift cards, coupons, returns, parcels, packages, webhooks, imports, exports, and tags. 917 path operations across the live OpenAPI 3.1 specification.

- **Human URL:** [https://docs.commercelayer.io/core/](https://docs.commercelayer.io/core/)
- **Base URL:** `https://{your-organization-slug}.commercelayer.io/api`

#### Tags

- Commerce
- Headless Commerce
- Multi-Market
- JSON:API
- Checkout
- Orders
- Catalog
- Inventory
- Promotions

#### Properties

- [Documentation](https://docs.commercelayer.io/core/)
- [Documentation](https://docs.commercelayer.io/core-api-reference/)
- [Documentation](https://docs.commercelayer.io/core/api-specification)
- [Authentication](https://docs.commercelayer.io/core/authentication)
- [Rate Limits](https://docs.commercelayer.io/core/rate-limits)
- [Webhooks](https://docs.commercelayer.io/core/real-time-webhooks)
- [Documentation](https://docs.commercelayer.io/core/event-stream-hub)
- [OpenAPI](https://data.commercelayer.app/schemas/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/commerce-layer-core-api-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/commerce-layer-core-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/commerce-layer-core-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/commerce-layer-order-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/commerce-layer-sku-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/commerce-layer-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Commerce Layer Provisioning API

Programmatic provisioning surface for Commerce Layer organizations, memberships, roles, API credentials, application memberships, identity providers (SSO), permissions, and user invitations. 48 path operations. Required for headless onboarding flows, infrastructure-as-code organization management, and enterprise identity federation. Available on Developer and Enterprise plans (Provisioning API access is an enterprise feature).

- **Human URL:** [https://docs.commercelayer.io/provisioning](https://docs.commercelayer.io/provisioning)
- **Base URL:** `https://provisioning.commercelayer.io`

#### Tags

- Administration
- Provisioning
- Organizations
- SSO
- JSON:API

#### Properties

- [Documentation](https://docs.commercelayer.io/provisioning)
- [Documentation](https://docs.commercelayer.io/provisioning-api-reference/)
- [OpenAPI](https://data.commercelayer.app/schemas/provisioning/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/commerce-layer-provisioning-api-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/commerce-layer-provisioning-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/commerce-layer-provisioning-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Commerce Layer Metrics API

Analytics surface over Commerce Layer's ecommerce history. Five query types (breakdown, date_breakdown, stats, search, export) across four domains (orders, carts, returns, usage) plus frequently-bought-together (FBT) analysis helpers. Useful for KPI dashboards, cohort and funnel reporting, catalog merchandising signals, and feeding downstream warehouses. Commerce Layer also publishes a local MCP server that exposes the Metrics API to AI agents.

- **Human URL:** [https://docs.commercelayer.io/metrics/welcome](https://docs.commercelayer.io/metrics/welcome)
- **Base URL:** `https://{your-domain}.commercelayer.io/metrics`

#### Tags

- Analytics
- Metrics
- Reporting
- Commerce Analytics
- Data

#### Properties

- [Documentation](https://docs.commercelayer.io/metrics/welcome)
- [Documentation](https://docs.commercelayer.io/metrics/getting-started/api-specification)
- [OpenAPI](https://data.commercelayer.app/schemas/metrics/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/commerce-layer-metrics-api-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/commerce-layer-metrics-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/commerce-layer-metrics-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [M C P Server](https://github.com/commercelayer/mcp-server-metrics)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://commercelayer.io)
- [Portal](https://commercelayer.io/product)
- [Documentation](https://docs.commercelayer.io)
- [Documentation](https://docs.commercelayer.io/core-api-reference/)
- [Documentation](https://docs.commercelayer.io/provisioning-api-reference/)
- [Documentation](https://docs.commercelayer.io/metrics/welcome)
- [Documentation](https://docs.commercelayer.io/data-model/readme)
- [Getting Started](https://docs.commercelayer.io/core/onboarding)
- [Authentication](https://docs.commercelayer.io/core/authentication)
- [Documentation](https://docs.commercelayer.io/core/api-credentials)
- [Documentation](https://docs.commercelayer.io/core/roles-and-permissions)
- [Rate Limits](https://docs.commercelayer.io/core/rate-limits)
- [Errors](https://docs.commercelayer.io/core/handling-errors)
- [Webhooks](https://docs.commercelayer.io/core/real-time-webhooks)
- [Documentation](https://docs.commercelayer.io/core/event-stream-hub)
- [Security](https://docs.commercelayer.io/core/callbacks-security)
- [Documentation](https://docs.commercelayer.io/public-endpoints)
- [Changelog](https://docs.commercelayer.io/changelog)
- [Blog](https://commercelayer.io/blog)
- [Pricing](https://commercelayer.io/pricing)
- [About](https://commercelayer.io/about)
- [Contact](https://commercelayer.io/contact)
- [Privacy Policy](https://commercelayer.io/legal-embed/privacy-policy)
- [Terms of Service](https://commercelayer.io/legal-embed/terms-and-conditions)
- [Sign Up](https://dashboard.commercelayer.io/sign_up)
- [Login](https://dashboard.commercelayer.io/sign_in)
- [Forum](https://discord.com/commercelayer)
- [GitHub Organization](https://github.com/commercelayer)
- [SDK](https://github.com/commercelayer/commercelayer-sdk)
- [SDK](https://github.com/commercelayer/commercelayer-js-auth)
- [SDK](https://github.com/commercelayer/commercelayer_ruby)
- [SDK](https://github.com/commercelayer/commercelayer-sdk-utils)
- [SDK](https://github.com/commercelayer/provisioning-sdk)
- [C L I](https://github.com/commercelayer/commercelayer-cli)
- [SDK](https://github.com/commercelayer/commercelayer-react-components)
- [Tool](https://github.com/commercelayer/drop-in.js)
- [Tool](https://github.com/commercelayer/mfe-checkout)
- [Tool](https://github.com/commercelayer/mfe-cart)
- [Tool](https://github.com/commercelayer/mfe-my-account)
- [Tool](https://github.com/commercelayer/mfe-identity)
- [Tool](https://github.com/commercelayer/mfe-microstore)
- [Tool](https://github.com/commercelayer/dashboard-apps)
- [M C P Server](https://github.com/commercelayer/mcp-server-metrics)
- [Code Examples](https://github.com/commercelayer/demo-store)
- [Code Examples](https://github.com/commercelayer/demo-store-core)
- [Code Examples](https://github.com/commercelayer/demo-store-minimal)
- [Code Examples](https://github.com/commercelayer/examples)
- [Code Examples](https://github.com/commercelayer/commercelayer-sanity-template)
- [Plugins](https://github.com/commercelayer/sanity-commerce)
- [Plugins](https://github.com/commercelayer/contentful-commerce)
- [Plugins](https://github.com/commercelayer/contentstack-commerce)
- [Plugins](https://github.com/commercelayer/dato-plugin)
- [Plugins](https://github.com/commercelayer/gatsby-plugin-commercelayer)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-resources)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-webhooks)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-imports)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-exports)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-metrics)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-checkout)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-orders)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-provisioning)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-microstore)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-seeder)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-cleanups)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-triggers)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-tags)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-links)
- [Plugins](https://github.com/commercelayer/commercelayer-cli-plugin-token)
- [Documentation](https://jsonapi.org/format/)
- [Plans](plans/commerce-layer-plans-pricing.yml)
- [Rate Limits](rate-limits/commerce-layer-rate-limits.yml)
- [Fin Ops](finops/commerce-layer-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
