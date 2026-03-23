# Case Study 12: Supply Chain & Inventory Management System — "StockFlow"

## Background

StockFlow serves a mid-sized retail chain with 80 physical stores and an online shop. The company sells consumer electronics and manages relationships with 120 suppliers across 8 countries. Getting the right products to the right stores at the right time is critical to avoiding both stockouts and excess inventory.

## The Organisation

- **Store managers** monitor local stock levels and request replenishment
- **Warehouse staff** receive supplier shipments, pick orders, and dispatch stock to stores and online customers
- **Procurement team** places orders with suppliers based on demand forecasts
- **Suppliers** receive purchase orders and confirm shipment dates
- **Finance team** reconciles invoices against received goods

## Current Situation

The company currently manages inventory through a mix of spreadsheets and a 10-year-old system that does not integrate with the online store. Stock levels are updated once a day overnight, meaning staff work with information that can be up to 24 hours old.

**Known problems:**
- Popular products sell out in stores but surplus stock sits in the warehouse because there is no real-time visibility
- Online orders are occasionally accepted for products that are actually out of stock
- Procurement makes ordering decisions based on stale data, leading to both over-ordering and under-ordering
- Receiving a supplier shipment at the warehouse is a fully manual paper process
- There is no way to track where a specific product is in the supply chain — warehouse, in transit, or at which store

## What the System Needs to Do

The new system must allow:

1. Real-time tracking of stock levels across all stores, the warehouse, and in-transit shipments
2. Automatic reorder suggestions when stock at a location falls below a threshold
3. Procurement staff to raise purchase orders and send them directly to suppliers
4. Warehouse staff to receive shipments by scanning barcodes and updating stock digitally
5. The online store to reflect actual available stock in real time
6. Finance to automatically match supplier invoices against received purchase orders

## Your Task

Design a software architecture for StockFlow that addresses the problems above.

Your design should consider:
- How to keep stock counts accurate and consistent across 80 stores, a warehouse, and an online shop simultaneously
- How to handle poor or no internet connectivity in some store locations
- How to integrate with suppliers who each have different ordering systems and communication methods
- How to alert the right people quickly when a critical product is about to run out
