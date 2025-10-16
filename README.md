## 📦 Logistics Delivery API — Test Task (.NET, 1 hour)

## 🧭 Overview

This test task is designed to evaluate your practical skills in C# / .NET and your understanding of resilience concepts in web applications.
Estimated completion time: ~1 hour.

You may use any NuGet packages and search for information online if needed.

### 🚚 Task

Implement a simple Web API that returns delivery information for an order.

1️⃣. Create an endpoint that:

Retrieves delivery information for a new order from an external provider in JSON format (link below), and save the received entities (some in-memory collection will be enough).

https://raw.githubusercontent.com/vitaliy-nerdysoft/NerdysoftTechInterview/main/orders.json

The external provider may be unstable and sometimes return a 403 error.

2️⃣. Create an endpoint that:

Displays the stored order information to the user by its ID.

📦 Example API Response
```json
[
  {
    "trackingNumber": "KWE123456789UA",
    "status": "InTransit",
    "estimatedDelivery": "2025-10-12T18:30:00Z",
    "origin": {
      "city": "Kyiv",
      "country": "Ukraine"
    },
    "destination": {
      "city": "Warsaw",
      "country": "Poland"
    },
    "events": [
      {
        "timestamp": "2025-10-06T09:45:00Z",
        "location": "Kyiv Warehouse",
        "description": "Shipment picked up"
      },
      {
        "timestamp": "2025-10-07T14:15:00Z",
        "location": "Lviv Sorting Center",
        "description": "Departed from facility"
      }
    ]
  }
]
```
