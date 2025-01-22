# HACKATHON-3-DOCUMENTATION
# E-Commerce Project

## **Project Overview**
This e-commerce project is built using **Next.js**, **Tailwind CSS**, and **Sanity CMS**, offering dynamic product displays, cart functionalities, and API integration for shipping and tracking. It aims to provide a user-friendly interface for browsing and purchasing furniture.

---

## **Features**
- Dynamic product listing and filtering.
- Add-to-cart functionality with real-time cart count updates.
- Integration with **Sanity CMS** for product management.
- API endpoints for shipping labels, tracking, and rate calculations using **ShipEngine**.
- Responsive design with **Tailwind CSS**.
- Deployed on **Vercel** for continuous integration and deployment.

---

## **File Structure**
```
project-root/
├── app/
│   ├── api/
│   │   ├── shipengine/
│   │   │   ├── label/
│   │   │   │   └── route.ts
│   │   │   ├── tracking/
│   │   │   │   └── route.ts
│   │   │   ├── get-rates/
│   │   │   │   └── route.ts
│   │   └── page.tsx
│   ├── components/
│   │   ├── latestproducts.tsx
│   │   ├── featuredproducts.tsx
│   │   └── cart.tsx
│   ├── pages/
│   │   └── index.tsx
├── lib/
│   └── helper/
│       └── shipEngine.ts
├── public/
│   ├── images/
│   └── assets/
├── styles/
│   └── globals.css
├── sanity/
│   ├── schemas/
│   └── config/
├── package.json
├── next.config.js
├── tailwind.config.js
├── README.md
```

---

## **Key Components and Directories**

### **1. app/api/shipengine/**
Contains API routes for interacting with ShipEngine:
- `label/route.ts`: Handles label creation.
- `tracking/route.ts`: Manages shipment tracking.
- `get-rates/route.ts`: Fetches shipping rates.

### **2. app/components/**
- `latestproducts.tsx`: Displays the latest products dynamically.
- `featuredproducts.tsx`: Highlights featured products.
- `cart.tsx`: Manages the shopping cart functionality, including dynamic updates.

### **3. lib/helper/**
- `shipEngine.ts`: Contains helper functions for API integration with ShipEngine.

### **4. sanity/**
- **Schemas:** Define the data structure for managing products in Sanity CMS.
- **Config:** Stores configuration files for connecting to the CMS.

---

## **Deployment**
https://template-4-hackathon-3.vercel.app/

### **Platform:**
The project is deployed on **Vercel** for seamless integration with Next.js.

### **Deployment Steps:**
1. Connected the GitHub repository to Vercel.
2. Verified the build command (`npm run build`) and output directory (`.next`).
3. Added necessary environment variables in the Vercel dashboard.
4. Deployed successfully with a live URL.

---

## **Technologies Used**
- **Next.js**: For server-side rendering and routing.
- **Tailwind CSS**: For styling and responsive design.
- **Sanity CMS**: For managing product data.
- **ShipEngine API**: For shipping label creation, tracking, and rate calculations.
- **React-Toastify**: For notifications (e.g., item added to cart).
- **Vercel**: For hosting and continuous deployment.

---

## **Future Improvements**
1. **Enhanced State Management:**
   - Implement Redux or Zustand for managing the global state.

2. **Improved Testing:**
   - Add unit and integration tests for key components and API routes.

3. **UI Consistency:**
   - Introduce a design system or component library.

4. **Error Handling:**
   - Implement better error boundaries and fallback UIs for API failures.

---

## **Contributions**
Feel free to fork the repository and submit pull requests for any improvements or bug fixes!

