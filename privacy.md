# Privacy Policy for FortunomiX

**Last updated: June 22, 2026**

This privacy policy applies to the FortunomiX mobile application (herein referred to as "the Application") for Android devices, created by Audaxio Dev (herein referred to as "the Service Provider") as a Freemium service.

At FortunomiX, we take privacy and data security seriously. The Application is designed with a **Privacy-by-Design** and **Offline-First** philosophy to give you absolute control and sovereignty over your financial data.

---

## 1. General No-Data-Collection Commitment
FortunomiX is built on a strict zero-data-collection infrastructure. We do not harvest, aggregate, sell, rent, or share personal, transactional, or financial data from any user of any age. We do not maintain any central user profiles or databases on our servers. Your financial records belong strictly to you and remain entirely under your local custody.

---

## 2. Core Philosophy: Offline-First & Data Sovereignty
The Application is fundamentally designed to operate without requiring any data to leave your physical device.
*   **Local Financial Data:** All financial records, including income, expenses, categories, recurrent rules, budget goals, and projection scenarios that you enter manually, are stored locally and exclusively on your physical device within a secure, internal SQLite database.
*   **No Central Server Logging:** By default, the Service Provider does not host, view, or maintain any backup of your personal financial records. You are the sole custodian and owner of your local database.

---

## 3. Optional Cloud Synchronization & Family Pairing (PRO Feature)
If you choose to purchase our PRO tier and pair devices with a family member (using our QR Pairing feature), the Application will synchronize data across those devices.
*   **Secure Infrastructure (Supabase):** Synchronization is powered by Supabase (PostgreSQL). 
*   **Encryption in Transit:** All synced data is transmitted securely over the internet using industry-standard Transport Layer Security (TLS/HTTPS) encryption.
*   **Row-Level Security (RLS):** Our cloud database is fortified with strict PostgreSQL Row-Level Security. This policy of access control ensures that only authenticated devices belonging specifically to your unique family ID (`family_id`) can read or write your synced data.

---

## 4. Smart Capture & AI Ticket Scanner (PRO Feature)
If you utilize our smart receipt scanner or upload PDF bank statements:
*   **Transient AI Processing:** The Application uses a secure, encrypted transit gateway and Supabase Edge Functions connected to Groq (utilizing Llama 3) to extract transaction values, installment counts, dates, and store names.
*   **No Persistent Cloud Storage:** This OCR and AI processing is completely **transient and in-memory**. The uploaded image or document is analyzed in-transit and immediately destroyed from the cloud memory after the structured transaction data is returned to your local SQLite database. We do not store, retain, or train AI models with your personal financial documents.

---

## 5. Android App Usage Tracking (UsageStatsManager)
The Application includes a smart tracking feature (Android-only) to detect your engagement with digital subscription apps (e.g., streaming, productivity, or gaming software).
*   **Purpose & Permission:** To use this automated optimization tool, the Application requests the specialized Android permission **`android.permission.PACKAGE_USAGE_STATS`**.
*   **Strictly Local Execution:** The querying of screen-time and usage metrics is processed **strictly and exclusively on your physical device** . Under no circumstances are your app usage habits, active packages, or engagement statistics sent to Audaxio Dev, Supabase, or any other third party.

---

## 6. Third-Party Services & Monetization
To keep our core features free, we display advertisements and process transactions through secure global partners. These third-party services may collect data to identify your device.

*   **Google AdMob (Advertising):** We use Google AdMob as our ad provider. AdMob may collect and process device-specific data, such as your Advertising ID, IP address, and usage patterns to deliver targeted or non-targeted ads.
    *   [Google AdMob Privacy Policy](https://policies.google.com/privacy)
*   **RevenueCat (In-App Purchases):** We use RevenueCat to process store receipts, validate premium entitlements, and manage active subscriptions. RevenueCat receives an anonymous subscriber identifier and your encrypted Google Play purchase token. No raw credit card numbers or personal identity data are shared with us.
    *   [RevenueCat Privacy Policy](https://www.revenuecat.com/privacy)

---

## 7. Local Notifications & Reminders
The Application uses local notifications to provide daily reminders for expense logging. These notifications are generated entirely within your device's local operating system and do not involve data transmission of any kind to external servers.

---

## 8. Data Control & International Privacy Rights (GDPR & CCPA)
We respect and support global data protection frameworks, including the European Union's General Data Protection Regulation (GDPR) and the California Consumer Privacy Act (CCPA).

Even though we are an offline-first app, we guarantee the following rights:
*   **Right to Access and Portability:** Since your data lives on your device, you can view all your transactions in the app at any time.
*   **Right to Deletion:**
    *   **Local Data:** You can permanently delete all local SQLite records by clearing the app data/cache in your Android system settings or by uninstalling the app.
    *   **Cloud Data (PRO Sync):** If you utilized our Cloud Sync, you can permanently purge all family records from our Supabase servers at any time by executing a "Factory Reset" inside the Application settings or by emailing us at audaxiodev@gmail.com.

---

## 9. Children’s Privacy (COPPA & GDPR-K Compliance)
Because the Service Provider maintains a strict, universal No-Data-Collection Policy for all users, we naturally do not knowingly collect, solicit, or process personal or financial information from children under the age of 18. If you are a parent or guardian and believe your child has used the Application, please be assured that any data they entered remains strictly stored on their physical device and cannot be accessed by us.

---

## 10. Security Limitations
We implement reasonable administrative, technical, and physical security measures to protect your synchronized cloud data (such as SSL/TLS and Postgres RLS policies). However, because the primary source of truth resides on your device, the security of your financial records ultimately depends on the physical security of your smartphone, your passcode protection, and your data backup practices. No method of internet transmission is 100% secure.

---

## 11. Changes to This Privacy Policy
We may update our Privacy Policy from time to time to align with new features or store policies. Any changes will be posted on this page with an updated "Last updated" date. We recommend reviewing this page periodically.

---

## 12. Contact Us
If you have any questions, suggestions, or requests regarding this Privacy Policy or your data, please contact us at:

*   **Email:** audaxiodev@gmail.com
