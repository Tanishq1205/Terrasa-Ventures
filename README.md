# Terrasa Ventures — B2B Packaging & Supply Platform

A fast, mobile-first digital catalog and B2B ordering portal for **Terrasa Ventures**, a food service packaging distributor supplying restaurants, cloud kitchens, caterers, and cafes.

The platform operates across two dedicated commercial product divisions: **Certified Compostable (Plant-Pulp)** and **High-Barrier Recyclable (Aluminum Foil & Virgin PP)**, pairing a high-contrast industrial UI (Primary White, Secondary Red, Tertiary Black) with a 1-click WhatsApp procurement workflow.

---

## 🚀 Live Deployments

[![Vercel Deployment](https://img.shields.io/badge/Deployed%20with-Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://terrasa-ventures.vercel.app)

* **Production URL:** [https://terrasa-ventures.vercel.app](https://terrasa-ventures.vercel.app)
* **Hosting Platform:** Vercel Global Edge Network
* **CI/CD:** Automatic production deployments connected to the GitHub repository

### Development & Build

* **Install dependencies:**
  ```bash
  npm install
---

## 📦 Commercial Product Architecture

The platform separates packaging inventory into two distinct operational lines via an interactive catalog toggle:

### 1. Certified Compostable Division
*Target: Eco-conscious cafes, salad bars, QSR brands, and corporate dining.*
* **Sugarcane Bagasse (5% GST):** Hinged clamshells (6"x6", 9"x6", 9"x9"), round gravy containers (250ml–750ml), rectangular meal boxes (500ml–1000ml), and multi-compartment lunch trays.
* **Cornstarch PLA (18% GST):** Heavy-duty bowls (150ml–650ml), snap-lid round & rectangular tubs, and 160mm rigid plant cutlery.
* **Kraft & White Paper (18% GST):** Round tubs, deep broth containers, wide 148-dia salad bowls with clear anti-fog lids, and folded lock-tab boxes.
* **Birchwood Cutlery (5% GST):** 14cm & 16cm spoons, forks, knives, sporks, and beverage stirrers (100% splinter-free).

### 2. High-Barrier Recyclable Division
*Target: Biryani houses, high-volume cloud kitchens, traditional curries, and bulk takeaways.*
* **Aluminum Foil Containers (18% GST):** Standard 450ml, 650ml, 750ml, and 1000ml wrinkle-wall meal containers with heat-retentive poly/foil lids.
* **Food-Grade Virgin PP Containers (18% GST):** Microwavable airtight round tubs (250ml–750ml) and heavy rectangular delivery boxes with snap-fit lids.
* **Commercial Wraps:** Heavyweight aluminum kitchen foil rolls (11-micron & 18-micron).

---

## ✨ Core Features

* **Dual-Division Catalog Toggle:** Switch instantly between *Certified Compostable* and *Foil & Recyclable* lines without reloading the page.
* **Material-Level Subcategory Filtering:** Dynamic client-side filtering by specific materials (Bagasse, Cornstarch, Kraft, Foil, PP, Birchwood).
* **Smart Sample Request Modal:** Automatically captures the selected SKU name into the request form and prepares an operational dispatch payload.
* **Direct WhatsApp Order Routing:** Converts user inputs (Outlet Name, Location, Contact Phone, Selected SKU) into a formatted WhatsApp order string sent to `+91 77100 74227`.
* **Zero-Dependency Architecture:** Pure HTML5, utility-first styling with Tailwind CSS, and Vanilla JavaScript. Fast initial load times with no complex npm build steps.

---

## 🛠️ Tech Stack

* **Frontend:** Semantic HTML5, [Tailwind CSS](https://tailwindcss.com/) (JIT CDN), Vanilla JavaScript (ES6+)
* **Typography:** [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans) (Headings & Body), [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) (Specs & Badges)
* **Lead Ingestion:** WhatsApp Business Click-to-Chat API
* **Hosting / CI-CD:** Render (Static Site Service) / Vercel
* **Operations Backend (Planned):** Airtable CRM (Suppliers, Inventory, Leads, Samples)

---

## 📁 Repository Structure

```text
terrasa-ventures/
├── index.html        # Complete application layout, catalog data, styles & logic
├── images/           # Product photography, container renders, and logos
│   ├── bagasse/
│   ├── cornstarch/
│   ├── paper/
│   ├── foil/
│   └── plastic/
└── README.md         # Platform documentation & operational setup
