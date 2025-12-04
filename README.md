# Project Requirements — AL HARAM STORE (Custom E-Commerce Website + Admin Panel)

This document describes the complete functional, technical, and design requirements for building a **fully custom e-commerce website** and **full admin panel** for **AL HARAM STORE**, including backend, frontend, database, API, admin features, brand guidelines, deployment, testing, and security.

No part of HomeShopping.pk should be copied.  
Only a **unique, original** system should be created.

---

## 🔵 Brand Identity
**Store Name:** AL HARAM STORE  
**Theme:** Hybrid (Royal Blue + Electric Cyan + Black + Navy)  
Colors:
- Electric Cyan: #19F0D8  
- Royal Blue: #1A4DFF  
- Black: #000000  
- Navy Dark: #0A1A3C  
- White: #FFFFFF  
- Grey: #C9C9C9

**Logo Style:**  
Techy / digital feel — cyan circuit-style icon + “AL HARAM STORE” text.  
Logo must be delivered in SVG + PNG.

---

## 🔵 Store Contact Info (Default Values)
- **Phone:** +92 300 9250960  
- **Email:** info@alharamstore.pk  
- **Address:** Your shop address here, City, Pakistan  

These must be editable from the **Admin Panel → Settings**.

---

## 🔵 Frontend (Storefront) Requirements
Tech: React or Next.js + TailwindCSS.

Pages required:
- Home (hero slider, categories, top deals, new arrivals)
- Category listing (filters: brand, price, rating)
- Product page (images gallery, variants, stock, specs, warranty info, add to cart)
- Cart + Checkout (Cash on Delivery + payment gateway test integration)
- Search (with auto-suggestions)
- User Account pages (orders, addresses, profile)
- Wishlist
- Static pages (About, Contact, Terms, Privacy)

---

## 🔵 Admin Panel Requirements
Tech: React Admin UI OR modern dashboard UI.

Admin features:
1. Login + JWT auth (+ optional 2FA for SuperAdmin)
2. Dashboard (today’s sales, orders, low stock, charts)
3. Products (add/edit/delete, upload images, variants, bulk CSV import)
4. Categories (CRUD + drag-drop sorting)
5. Orders (full workflow: pending → processing → shipped → delivered)
6. Payments & Transactions (log all gateway events)
7. Payouts (mark vendor payouts as Paid/Unpaid)
8. Coupons (create promotions, flash sales)
9. Banners (upload promo slider images)
10. Customers (view accounts, order history)
11. Returns (approve/reject + refund flow)
12. Reports (sales, payouts, orders ➝ downloadable CSV)
13. Settings (phone, email, address, logo, SMTP, payment keys)
14. Admin Users & Roles (SuperAdmin, Admin, Staff)
15. Audit Logs (track changes)

---

## 🔵 Backend Requirements
Tech: Node.js (Express or NestJS)  
DB: MySQL or PostgreSQL  
Auth: JWT (access + refresh tokens)

REST API endpoints required:
- Authentication (admin + customer)
- Products CRUD
- Categories CRUD
- Orders CRUD + status updates
- Cart API
- Checkout + mock payment gateway
- Coupons
- Transactions
- Payouts
- Settings API (read/write)
- Upload API (product images, banners)
- Reports API

---

## 🔵 Database Schema (Required Tables)
- settings
- admin_users
- users
- categories
- products
- product_variants
- orders
- order_items
- transactions
- payouts
- coupons
- banners
- returns
- audit_logs

Migrations + seed data must be included.

Seed Data:
- SuperAdmin account
- Store settings (phone/email/address)
- Sample categories
- Sample product

---

## 🔵 File Storage
Use local storage for dev, abstract service for S3/Spaces for production.

---

## 🔵 Deployment Requirements
Deliver:
- Dockerfile (frontend + backend)
- docker-compose.yml (app + DB)
- Nginx reverse proxy config
- Certbot SSL instructions
- Environment variables template (.env.example)

Supported deployment:
- DigitalOcean Droplet OR
- Render / Railway OR
- Vercel (frontend) + Render (backend)

---

## 🔵 Payment Integration
Mock/test integration first.
Real integrations required later:
- EasyPaisa
- JazzCash
- Stripe

Webhook endpoint must be included.

---

## 🔵 Testing Requirements
- Backend unit tests
- API integration tests
- Frontend e2e tests (Cypress or Playwright)
- Test checkout flow with mock payment

---

## 🔵 Acceptance Criteria
A complete working system must include:
- Fully functional frontend with responsive UI  
- Fully functional admin panel  
- Working product management  
- Working order management  
- Working settings page (phone: +92 300 9250960 visible on frontend)  
- Working checkout (mock payment)  
- Deployment-ready Docker setup  
- SSL-enabled Nginx configuration  
- Clear README with setup steps + environment variables  

---

## Deliverables
- Full source code
- Database migrations + seeds
- Docker compose setup
- Nginx config
- Logo files (SVG/PNG)
- README with full installation + deployment instructions
