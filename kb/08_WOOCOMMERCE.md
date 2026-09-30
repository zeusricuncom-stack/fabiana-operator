# KB 08 — WooCommerce

## Purpose
Handle ecommerce structure, design and dynamic data without converting transactional behavior into static mock content.

## Context detection
Identify whether the site uses classic templates, Woo Blocks, Divi Woo modules, Theme Builder templates, hooks, custom code or a mixed setup.

## Operation classes
### DESIGN OPERATIONS
Product cards, archives, PDP layout, visual hierarchy and merchandising presentation.

### CATALOG OPERATIONS
Products, variations, attributes, categories, tags, prices, stock and sale dates.

### TRANSACTIONAL OPERATIONS
Cart, checkout, orders, payment gateways, taxes, shipping, emails and permissions. Treat as higher risk.

## Technical preference
Prefer, in order when appropriate:
setting -> native Divi/Woo module or Woo Block -> shortcode -> CSS -> hook/filter -> API -> mini-plugin -> template override.
Never edit WooCommerce core or a parent theme.

## Dynamic integrity
- Keep price, stock, attributes and order data dynamic.
- Never hardcode transactional values that should come from WooCommerce.
- Distinguish cart/checkout classic vs blocks before customization.
- Validate product/variation relationships.

## QA requirements
For relevant projects validate product archives, product detail, variation selection, cart, checkout path, responsive behavior and dynamic values.

## Safety
Transactional changes require explicit intent and risk-aware approval. Do not place test orders or alter live orders/payments unless specifically authorized.
