# Case Study 3: E-commerce Marketplace — "ShopHub"

## Background

ShopHub is an online marketplace where independent sellers list products and customers purchase them. It operates like a platform between buyers and sellers, handling discovery, checkout, payment, and logistics coordination. The platform currently has 3,000 active sellers and 200,000 registered customers.

## The Organisation

- **Customers** browse, search, purchase, and review products
- **Sellers** list products, manage inventory, and fulfil orders
- **Delivery partners** (third-party couriers) pick up and ship orders
- **ShopHub admin** verifies seller accounts, mediates disputes, and runs promotions

## Current Situation

ShopHub processes an average of 8,000 orders per day. During seasonal sales events (e.g., holidays, flash sales), order volume spikes to 10× the normal rate. The current system was built quickly and was not designed for this scale.

**Known problems:**
- Product search is slow and often returns irrelevant results
- Inventory shown to customers sometimes does not match actual seller stock, causing cancelled orders
- The checkout process times out during traffic spikes
- Sellers have no real-time visibility into their sales or stock levels
- Fraudulent seller accounts and fake reviews are difficult to detect

## What the System Needs to Do

The new system must allow:

1. Customers to search and filter products across all sellers
2. Customers to add items to a cart and complete checkout with payment
3. Sellers to manage their product listings and view inventory levels in real time
4. The system to reserve stock when a customer adds an item to cart, releasing it if checkout is abandoned
5. Delivery partners to receive shipment requests and update tracking status
6. Admin to manage seller verification, promotions, and dispute resolution

## Your Task

Design a software architecture for ShopHub that addresses the problems above.

Your design should consider:
- How to handle extreme traffic spikes without the system going down
- How to keep product inventory consistent across many concurrent buyers
- How to protect customers' payment information
- How to make product search fast and relevant at scale
