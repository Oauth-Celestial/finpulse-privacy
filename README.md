# Privacy Policy for FinPulse


This Privacy Policy describes how the **"FinPulse"** Android application ("the App," "we," "our," or "us") collects, uses, and protects your information.

We built FinPulse with a strict **local-first architecture**. We believe your digital habits, financial records, and app usage are strictly your own business. Therefore, our core privacy principle is simple: **all data processing happens directly on your device, and we do not collect, transmit, or store your personal or financial data on external servers.**

---

### 1. Information Collection and Use

To provide core features including "Resolve Mode" (mindful friction and impulse app interception), smart transaction detection, and offline budget tracking, FinPulse requires specific Android permissions. We want to be completely transparent about what these permissions do and how they are handled locally on your device:

#### Usage Access (Usage Stats)
* **Why we need it:** We use this permission to detect when you launch apps you have designated for mindful friction (such as impulse shopping, e-commerce, food delivery, or payment apps).
* **How it is handled:** Monitoring is conducted **100% locally on your device**. We do not track your general app usage history, nor do we record or transmit any information about what apps you open to our servers or any third parties.

#### Display Over Other Apps (System Alert Window)
* **Why we need it:** This permission allows FinPulse to display the "Resolve Mode" mindful friction overlay (breathing exercises, cooldown timers, budget checks, and reflection prompts) directly on top of the app you are trying to open before you make an impulsive purchase.
* **How it is handled:** This permission is strictly utilized to present the user interface overlay. It does not record your screen, log touch events outside its window, or inspect the content of the apps beneath the overlay.

#### Payment & Bank Notification Listener Access (`NotificationListenerService`)
* **Why we need it:** This permission allows FinPulse to detect incoming debit and payment alert notifications from banking and UPI applications, enabling 1-tap automated expense logging without tedious manual entry.
* **How it is handled:** Notification parsing is performed **exclusively on-device**:
  * FinPulse only extracts the debit amount, merchant/payee name, and timestamp.
  * Personal chat messages, One-Time Passwords (OTPs), verification codes, security credentials, and promotional alerts are strictly filtered out and immediately discarded.
  * Raw notification text is never stored, uploaded, or transmitted anywhere.

#### Foreground Service & System Notifications (`POST_NOTIFICATIONS`, `FOREGROUND_SERVICE`)
* **Why we need it:** To ensure the App can reliably detect selected app launches and run Resolve Mode without being terminated by Android's aggressive battery optimizations, FinPulse runs a local foreground service attached to a persistent system notification. It also allows us to send daily budget reviews and spending threshold alerts.
* **How it is handled:** This service runs strictly locally on your device. It does not collect, log, or broadcast personal data.

#### Exact Alarms & Boot Receiver (`SCHEDULE_EXACT_ALARM`, `RECEIVE_BOOT_COMPLETED`)
* **Why we need it:** To schedule and trigger precise daily review reminders, budget reset alerts, and custom financial check-ins, even after your device restarts.
* **How it is handled:** These operations rely entirely on native Android system alarms on your device. No data is shared or transmitted.

---

### 2. Data Storage and Security

Because FinPulse utilizes a local-first design:
* All your transactions, expense categories, budgets, Resolve Mode configurations, and app-blocking rules are saved locally in your device's internal private storage (sandboxed SQLite database).
* We **do not** maintain user accounts, require registration, or require a login.
* We **do not** host or maintain an external database of our users' transactions, bank accounts, or digital habits.
* If you uninstall the App or clear the App's data through Android Settings, all your local data and configurations will be permanently deleted from your device.
* We rely on the standard sandboxing and security protocols provided by the Android operating system to protect your local app data from other applications installed on your device.

---

### 3. Third-Party Services and Analytics

* We **do not** integrate third-party analytics trackers, advertising SDKs, or background telemetry tools that quietly harvest your data.
* We **do not** sell, rent, monetize, or share your personal, financial, or app usage data with data brokers, advertisers, or any external entities.
* Your interaction with the App is completely private.

---

### 4. Children’s Privacy

FinPulse does not knowingly collect personally identifiable information from anyone, including children under the age of 13. Because the App operates entirely offline and does not transmit data off your device, no personal data from children is collected or processed by us.

---

### 5. Changes to This Privacy Policy

We may update our Privacy Policy from time to time. We will notify you of any changes by posting the updated Privacy Policy on this page and updating the "Effective Date" at the top. We advise you to review this page periodically for any changes.

---

### 6. Contact Us

If you have any questions, concerns, or suggestions regarding this Privacy Policy or the way FinPulse handles your device permissions and privacy, please reach out:

* **Developer:** Ravi
* **Email:** [ravi983365@gmail.com](mailto:ravi983365@gmail.com)
