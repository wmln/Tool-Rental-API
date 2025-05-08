# Tool Rental API – Postman Collection

This repository contains a Postman collection for interacting with the [Simple Tool Rental API](https://simple-tool-rental-api.glitch.me).

## 📌 About the API

The Simple Tool Rental API allows you to:
- Check API status
- Retrieve tools from an inventory
- Place and manage tool rental orders
- Authenticate via an API client

## 🔗 Live API Endpoint

[https://simple-tool-rental-api.glitch.me](https://simple-tool-rental-api.glitch.me)

## 📁 Contents

- `Tool-Rental-API.postman_collection.json` – The main Postman collection

## 📚 Key Endpoints

### Status
- `GET /status` – Check API status (UP/DOWN)

### Tools
- `GET /tools` – Get all tools (filterable by category, availability, results)
- `GET /tools/:toolId` – Get a specific tool (optionally include user manual)

### Orders (Require Authentication)
- `GET /orders` – View all orders
- `GET /orders/:orderId` – View a specific order (optionally with invoice)
- `POST /orders` – Create a new order
- `PATCH /orders/:orderId` – Update an existing order
- `DELETE /orders/:orderId` – Cancel/delete an order

### Authentication
- `POST /api-clients` – Register a new API client to receive a bearer token

> **Note**: All authenticated endpoints require the `Authorization: Bearer YOUR_TOKEN` header.

## 🧪 How to Use

1. Import the `.postman_collection.json` file into [Postman](https://postman.com).
2. Register your API client using `POST /api-clients`.
3. Use the returned token to access authenticated routes.
4. Explore and test available API endpoints.

## 📝 Reference

This Postman collection is based on the [Simple Tool Rental API](https://glitch.com/edit/#!/simple-tool-rental-api) originally developed and hosted on Glitch.

---

Feel free to fork, modify, or extend this collection to suit your project needs.
