# Customer Events Code Documentation

This repository contains two `.gtag` format scripts designed for Shopify implementations to enhance tracking and analytics. These scripts are part of the Shopify Customer Events setup and provide seamless integration for GA4 Enhanced E-commerce tracking and Google Ads conversion tracking, including Enhanced Conversions.

---

## 📂 Files Overview

### 1. **`customer-events-ga4-googleads`**
   - **Purpose:** 
     - Comprehensive tracking for GA4 Enhanced E-commerce.
     - Google Ads conversion tracking.
     - Enhanced Conversions support for improved attribution.
   - **Features:**
     - Captures key e-commerce events, including:
       - `view_item`
       - `add_to_cart`
       - `begin_checkout`
       - `purchase`
     - Sends event data to both GA4 and Google Ads.
     - Ensures Enhanced Conversions data is passed securely for better cross-device attribution.

### 2. **`gTag-Enhanced-Conversions`**
   - **Purpose:** 
     - Google Ads Conversion Tracking.
   - **Features:**
     - Tracks critical conversion events like purchases, leads, or sign-ups.
     - Includes Enhanced Conversions functionality to improve data matching for attribution.

---

## 🛠️ Implementation Instructions for Shopify

1. **Navigate to Shopify Settings:**
   - Go to your Shopify Admin.
   - Click on **Settings** > **Customer Events**.

2. **Add a New Customer Event:**
   - For whichever script you choose to implement:
     - **GA4 Measurement ID:** Enter your GA4 Measurement ID for enhanced e-commerce tracking (if using the `customer-events-ga4-googleads` script).
     - **Google Ads Conversion ID and Label:** Enter your Google Ads Conversion ID and Conversion Label for tracking Google Ads conversions (if using either script).

3. **Save and Test:**
   - Save your customer event setup.
   - Use debugging tools like **GA4 DebugView** and **Google Tag Assistant** to validate that events are firing correctly.

---

## 📖 Supported Events and Data

### **GA4 Enhanced E-commerce (customer-events-ga4-googleads):**
   - Tracks full e-commerce funnel events:
     - `view_item`: Product detail views.
     - `add_to_cart`: Items added to the cart.
     - `begin_checkout`: Checkout initiation.
     - `purchase`: Successful purchases.

### **Google Ads Conversion Events (gTag-Enhanced-Conversions):**
   - Focuses on Google Ads conversions:
     - Purchase events.
     - Other custom conversions specified in your Google Ads setup.

---

## 🔍 Enhanced Conversions

Both scripts support Enhanced Conversions, which improve attribution accuracy by securely passing hashed customer data such as:
- Email
- Phone Number
- Address

This ensures better matching between online conversions and Google Ads click data.

---

## 🔔 Notes

- These scripts are designed specifically for Shopify and assume the presence of Shopify's Customer Events feature.
- Ensure you have the correct GA4 Measurement ID, Google Ads Conversion ID, and Conversion Label for optimal performance.
- Always test changes using Shopify’s preview feature or a test order before going live.
