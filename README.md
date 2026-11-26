<div align="center">

# 👕 ƒιтѕу 👖

### 👚 Fashion · 360° Views · Virtual Runway 👗

**Explore your style. Discover every detail.**

A digital fashion app for browsing Men’s and Women’s collections, exploring garments in 360°, and previewing outfits on virtual models.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)

</div>

---

## 📖 Contents

- [About ƒιтѕу](#-about-ƒιтѕу)
- [Features](#-features)
- [Account Access](#-account-access)
- [Customer Shopping Journey](#-customer-shopping-journey)
- [Owner Dashboard](#-owner-dashboard)
- [System Architecture](#-system-architecture)
- [Technology Stack](#️-technology-stack)
- [Team](#-ƒιтѕу-team)

---

## ✨ About ƒιтѕу

**ƒιтѕу** is a digital fashion shopping app for exploring **Men’s and Women’s clothing**. Customers can browse the catalog, inspect garments from different angles using 360° views, and optionally preview an outfit on a virtual model before placing an order.

The app also includes an owner section for managing products, runway demonstrations, and customer orders.

---

## 🌟 Features

| Symbol | Feature | Description |
|:---:|---|---|
| 👕 | **Fashion Catalog** | Browse Men’s and Women’s collections. |
| 👖 | **Product Cart** | Add selected products to the cart. |
| 👗 | **360° Studio** | Explore garments from different angles. |
| 👚 | **Virtual Model Preview** | Optionally preview clothing on a model. |
| 📍 | **Delivery Details** | Enter an address for the order. |
| 💳 | **Payment** | Continue through the available payment option. |
| 📦 | **Order Confirmation** | Review the order after checkout. |
| 🎨 | **Owner Section** | Manage products, runway items, and orders. |

---

## 🔐 Account Access

New customers create an account first. After signup, they can log in through the same login page used by existing customers.

The shared login page provides separate access paths:

- **Customer:** Phone number and password.
- **Owner:** Phone number, email address, and password.
- Successful customer login opens the **Customer Dashboard**.
- Successful owner login opens the **Owner Dashboard**.

```mermaid
flowchart TD
    A["Open ƒιтѕу"] --> B["Shared Login Page"]
    B --> C{"New customer?"}

    C -->|"Yes"| D["Customer Sign Up"]
    D --> E["Account Created"]
    E --> F["Customer Login"]

    C -->|"No, existing customer"| F
    F --> G["Enter phone and password"]
    G --> H{"Customer details correct?"}
    H -->|"Yes"| I["Customer Dashboard"]
    H -->|"No"| X["Show login error"]

    B --> J["Owner Login"]
    J --> K["Enter phone, email, and password"]
    K --> L{"Owner details correct?"}
    L -->|"Yes"| M["Owner Dashboard"]
    L -->|"No"| X
```

---

## 🛍️ Customer Shopping Journey

From the customer dashboard, customers can browse the catalog, add products to their cart, and continue to checkout. Trying an outfit on a virtual model is optional.

```mermaid
flowchart LR
    A["Customer Login"] --> B["Customer Dashboard"]
    B --> C["Open Catalog"]
    C --> D["Browse Men’s and Women’s Clothing"]
    D --> E["Select Products"]
    E --> F["Add Products to Cart"]
    F --> G{"Preview on a model?"}
    G -->|"Yes"| H["Choose a model and preview outfit"]
    G -->|"No"| I["Continue to checkout"]
    H --> I
    I --> J["Enter delivery address"]
    J --> K["Choose payment option"]
    K --> L["Review and confirm order"]
    L --> M["Order Confirmation"]
```

---

## 🎨 Owner Dashboard

The owner can manage products, runway demonstrations, and customer orders. Product management may include creating, viewing, updating, and deleting product records.

```mermaid
flowchart TD
    A["Owner Login"] --> B["Owner Dashboard"]

    B --> C["Product Management"]
    B --> D["Runway Demonstrations"]
    B --> E["Customer Orders"]

    C --> C1["Create product"]
    C --> C2["View products"]
    C --> C3["Update product"]
    C --> C4["Delete product"]

    D --> D1["Add or update demonstration"]
    D --> D2["Remove demonstration"]

    E --> E1["View orders"]
    E --> E2["Update order details"]

    C1 --> F[("Application Database")]
    C2 --> F
    C3 --> F
    C4 --> F
    D1 --> F
    D2 --> F
    E1 --> F
    E2 --> F
```

---

## 🏗️ System Architecture

```mermaid
flowchart LR
    Customer["Customer"] --> Frontend["ƒιтѕу Web App"]
    Owner["Owner"] --> Frontend

    Frontend --> Catalog["Catalog and Cart"]
    Frontend --> Studio["360° Studio"]
    Frontend --> Runway["Virtual Model Preview"]
    Frontend --> Accounts["Signup and Login"]
    Frontend --> Dashboard["Owner Dashboard"]

    Catalog --> Server["Node.js Server"]
    Studio --> Server
    Runway --> Server
    Accounts --> Server
    Dashboard --> Server

    Server --> Database[("SQLite Database")]
```

---

## 🧰 Technology Stack

| Area | Technologies |
|---|---|
| **Frontend** | HTML5, CSS3, JavaScript, TypeScript |
| **3D Visualization** | Three.js, WebGL |
| **Build Tool** | Vite |
| **Backend** | Node.js |
| **Database** | SQLite |
| **Maps and Location** | Leaflet.js, OpenStreetMap Nominatim |
| **Version Control** | Git, GitHub |

---

## 👥 ƒιтѕу Team

<div align="center">

### ✨ The Team Behind ƒιтѕу ✨

| 🪪 Student ID | 👤 Team Member |
|:---:|:---|
| **2620030089** | **Manideep** |
| **2620030105** | **Gowtham Sai** |
| **2620030104** | **Vishwak** |

👕 &nbsp; 👖 &nbsp; 👗 &nbsp; 👚

</div>

---

<div align="center">

# 👕 ƒιтѕу 👖

### **Fashion for Men. Fashion for Women. Style for Everyone.**

*Find your style with ƒιTѕу.* 👗

</div>
