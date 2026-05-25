# Commerce Layer (commerce-layer)
Commerce Layer is the headless, multi-market commerce API used by global brands to sell everywhere — web, mobile, in-store, chatbot, AI agent, and IoT. The platform exposes a JSON:API-compliant Core API with 130+ top-level resources covering orders, line items, SKUs, bundles, prices, markets, stores, inventory, customers, payments (Adyen, Stripe, Braintree, PayPal, Klarna, Checkout.com), tax (Avalara, TaxJar, Vertex, Stripe Tax), shipping, promotions, subscriptions, returns, and webhooks. It also ships a Provisioning API for organizations/SSO/credentials and a Metrics API for analytics — with a local MCP server for AI agents — plus hosted micro-frontends, dashboard apps, a CLI, CMS integrations, and SDKs.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/commerce-layer/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Headless Commerce, Composable Commerce, API-First, Ecommerce, JSON:API, OAuth 2.0, Multi-Market, Multi-Currency, B2C, B2B, Subscriptions, Promotions, Inventory, Order Management, Checkout

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Commerce Layer Core API
The JSON:API-compliant REST surface that powers headless commerce. 917 path operations across 130+ top-level resources — orders, line items, SKUs, bundles, prices, price lists, markets, stores, inventory (stock items, locations, transfers, reservations), customers, customer groups, customer subscriptions, payment gateways (Adyen, Stripe, Braintree, PayPal, Klarna, Checkout.com, Axerve, Satispay), tax calculators (Avalara, TaxJar, Vertex, Stripe Tax), shipping methods, shipping zones, carrier accounts, geocoders (Google, Bing), promotions (BXGY, percentage, fixed-amount, free-gift, free-shipping, flex), gift cards, coupons, returns, parcels, webhooks, imports, exports, tags.

**Base URL:** `https://{your-organization-slug}.commercelayer.io/api`
**Human URL:** [https://docs.commercelayer.io/core/](https://docs.commercelayer.io/core/)

- [Documentation](https://docs.commercelayer.io/core/)
- [Core API Reference](https://docs.commercelayer.io/core-api-reference/)
- [API Specification](https://docs.commercelayer.io/core/api-specification)
- [Authentication](https://docs.commercelayer.io/core/authentication)
- [Rate Limits](https://docs.commercelayer.io/core/rate-limits)
- [Webhooks](https://docs.commercelayer.io/core/real-time-webhooks)
- [Event Stream Hub (SSE)](https://docs.commercelayer.io/core/event-stream-hub)
- [Public OpenAPI Schema](https://data.commercelayer.app/schemas/openapi.json)
- [OpenAPI (local mirror)](openapi/commerce-layer-core-api-openapi.json)
- [JSON Schema — Order](json-schema/commerce-layer-order-schema.json)
- [JSON Schema — SKU](json-schema/commerce-layer-sku-schema.json)
- [JSON-LD](json-ld/commerce-layer-context.jsonld)
- [Naftiko Capability — Orders](capabilities/core-orders.yaml)
- [Naftiko Capability — SKUs](capabilities/core-skus.yaml)
- [Naftiko Capability — Customers](capabilities/core-customers.yaml)
- [Naftiko Capability — Markets](capabilities/core-markets.yaml)
- [Naftiko Capability — Prices](capabilities/core-prices.yaml)
- [Naftiko Capability — Shipments](capabilities/core-shipments.yaml)
- [Naftiko Capability — Promotions](capabilities/core-promotions.yaml)
- [Naftiko Capability — Webhooks and Events](capabilities/core-webhooks.yaml)

### Commerce Layer Provisioning API
Programmatic provisioning surface for Commerce Layer organizations, memberships, roles, API credentials, application memberships, identity providers (SSO), permissions, and user invitations. 48 path operations. Available on the Enterprise plan.

**Base URL:** `https://provisioning.commercelayer.io`
**Human URL:** [https://docs.commercelayer.io/provisioning](https://docs.commercelayer.io/provisioning)

- [Documentation](https://docs.commercelayer.io/provisioning)
- [Provisioning API Reference](https://docs.commercelayer.io/provisioning-api-reference/)
- [Public OpenAPI Schema](https://data.commercelayer.app/schemas/provisioning/openapi.json)
- [OpenAPI (local mirror)](openapi/commerce-layer-provisioning-api-openapi.json)
- [Naftiko Capability — Organizations](capabilities/provisioning-organizations.yaml)
- [Naftiko Capability — Memberships and Roles](capabilities/provisioning-memberships.yaml)
- [Naftiko Capability — API Credentials](capabilities/provisioning-api-credentials.yaml)
- [Naftiko Capability — Identity Providers](capabilities/provisioning-identity-providers.yaml)

### Commerce Layer Metrics API
Analytics surface over Commerce Layer's ecommerce history. Five query types — `breakdown`, `date_breakdown`, `stats`, `search`, `export` — across four domains: orders, carts, returns, usage. Includes a frequently-bought-together (FBT) analysis helper. Commerce Layer also publishes a local MCP server for the Metrics API so AI agents can query commerce data.

**Base URL:** `https://{your-domain}.commercelayer.io/metrics`
**Human URL:** [https://docs.commercelayer.io/metrics/welcome](https://docs.commercelayer.io/metrics/welcome)

- [Documentation](https://docs.commercelayer.io/metrics/welcome)
- [Metrics API Specification](https://docs.commercelayer.io/metrics/getting-started/api-specification)
- [Public OpenAPI Schema](https://data.commercelayer.app/schemas/metrics/openapi.json)
- [OpenAPI (local mirror)](openapi/commerce-layer-metrics-api-openapi.json)
- [Local MCP Server](https://github.com/commercelayer/mcp-server-metrics)
- [Naftiko Capability — Orders Analytics](capabilities/metrics-orders.yaml)
- [Naftiko Capability — Carts Analytics](capabilities/metrics-carts.yaml)
- [Naftiko Capability — Returns Analytics](capabilities/metrics-returns.yaml)
- [Naftiko Capability — Usage and FBT Analysis](capabilities/metrics-usage.yaml)

## Plans, Rate Limits, and FinOps

- [Plans and Pricing](plans/commerce-layer-plans-pricing.yml) — Free Developer plan, Enterprise plan (custom), Pro-bono plan; Distributed OMS and Promotion Engine add-ons.
- [Rate Limits](rate-limits/commerce-layer-rate-limits.yml) — Sliding-window per IP. Live/test split. Cacheable vs uncacheable read tiers. Auth at 30 req/min. Writes at 200 req/min live / 50 burst per endpoint.
- [FinOps](finops/commerce-layer-finops.yml) — FOCUS-aligned. Subscription + Add-on model, with live-order volume as the primary commerce-unit signal.

## SDKs, CLI, and Tooling

- [JavaScript / TypeScript SDK](https://github.com/commercelayer/commercelayer-sdk)
- [JavaScript Auth Library](https://github.com/commercelayer/commercelayer-js-auth)
- [SDK Utilities (batching, etc.)](https://github.com/commercelayer/commercelayer-sdk-utils)
- [Ruby SDK](https://github.com/commercelayer/commercelayer_ruby)
- [Provisioning SDK](https://github.com/commercelayer/provisioning-sdk)
- [Commerce Layer CLI](https://github.com/commercelayer/commercelayer-cli) — plus 15+ plugins (resources, webhooks, imports, exports, metrics, checkout, orders, provisioning, microstore, seeder, cleanups, triggers, tags, links, token)
- [React Components](https://github.com/commercelayer/commercelayer-react-components)
- [drop-in.js](https://github.com/commercelayer/drop-in.js)
- Hosted micro-frontends: [Checkout](https://github.com/commercelayer/mfe-checkout), [Cart](https://github.com/commercelayer/mfe-cart), [My Account](https://github.com/commercelayer/mfe-my-account), [Identity](https://github.com/commercelayer/mfe-identity), [Microstore](https://github.com/commercelayer/mfe-microstore)
- [Dashboard Apps](https://github.com/commercelayer/dashboard-apps) — orders, customers, shipments, returns, promotions, imports, exports, webhooks, skus, sku-lists, price-lists, inventory, stock-transfers, tags
- CMS integrations: [Sanity Commerce](https://github.com/commercelayer/sanity-commerce), [Contentful Commerce](https://github.com/commercelayer/contentful-commerce), [Contentstack Commerce](https://github.com/commercelayer/contentstack-commerce), [DatoCMS plugin](https://github.com/commercelayer/dato-plugin), [Gatsby plugin](https://github.com/commercelayer/gatsby-plugin-commercelayer)
- [MCP server for Metrics API](https://github.com/commercelayer/mcp-server-metrics)

## Demos and Examples

- [Demo Store](https://github.com/commercelayer/demo-store)
- [Demo Store Core](https://github.com/commercelayer/demo-store-core)
- [Demo Store Minimal](https://github.com/commercelayer/demo-store-minimal)
- [Examples Collection](https://github.com/commercelayer/examples)
- [Sanity / Next.js / Netlify multi-country template](https://github.com/commercelayer/commercelayer-sanity-template)

## Community and Operations

- [Sign Up (Free)](https://dashboard.commercelayer.io/sign_up)
- [Dashboard](https://dashboard.commercelayer.io/sign_in)
- [Discord Community](https://discord.com/commercelayer)
- [GitHub Organization](https://github.com/commercelayer)
- [Blog](https://commercelayer.io/blog)
- [Changelog](https://docs.commercelayer.io/changelog)
- [Privacy Policy](https://commercelayer.io/legal-embed/privacy-policy)
- [Terms and Conditions](https://commercelayer.io/legal-embed/terms-and-conditions)
