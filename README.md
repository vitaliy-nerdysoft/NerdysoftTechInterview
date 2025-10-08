# 📦 Logistics Delivery API — Test Task (.NET, 1 hour)

## 🧭 Overview

Це тестове завдання створене для оцінки ваших практичних навичок у C# / .NET, а також розуміння концепцій відмовостійкості у веб-додатках.  
Тривалість виконання: **~1 година**.

Можна використовувати будь-які nuget пакети. За потреби можна гуглити інформацію.
---

### 🚚 Завдання

Реалізуйте простий Web API, який повертає **інформацію про доставку замовлення**.

## 1️. Створіть endpoint який:

Дістає від стороннього провайдеру інформацію про нову доставку у форматі JSON (приклад нижче).

https://raw.githubusercontent.com/vitaliy-nerdysoft/NerdysoftTechInterview/main/orders.json

Данний провайдер може працювати зі збоями та іноді повертати 403 помилку.
Та зберігає це замовлення (In-memory колекції буде достатньо).

## 2. Створіть endpoint який:

Відображає данне замовлення користувачеві.
---

## 📦 Приклад відповіді API

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

## 3. Якщо вистачить часу:
* Додайте кешування відповіді
* Додайте тести
