# Privacy Policy for SMS Translator

**Last Updated:** October 16, 2026  
**Application:** SMS Translator (`com.smstranslator.app`)

Welcome to SMS Translator ("we", "our", or "the app"). We respect your privacy and are committed to protecting your personal information. This Privacy Policy explains how our application handles your data when you use SMS Translator as your default SMS messaging application on Android.

---

## 1. Overview & Core Privacy Principles

SMS Translator is designed from the ground up with **privacy-first, on-device processing**:
- **On-Device Machine Learning:** All text translations are performed locally on your device using on-device machine learning models (Google ML Kit). **Your messages and SMS content are never sent to external servers or cloud services for translation.**
- **No Data Selling or Sharing:** We do not sell, rent, monetize, or share your messages, contacts, or personal data with any third parties or advertisers.
- **Minimal Permissions:** We only request permissions necessary to provide core SMS messaging, contact display, and translation features.

---

## 2. Information Accessed and Processed

### A. SMS and MMS Messages (`RECEIVE_SMS`, `READ_SMS`, `SEND_SMS`, `RECEIVE_MMS`, `RECEIVE_WAP_PUSH`)
- **Purpose:** SMS Translator operates as a **Default SMS Handler**. It accesses your SMS and MMS messages strictly to allow you to send, receive, view, organize, and search your messages, including picture messages and group conversations.
- **Delivery:** Messages you send, and picture messages you receive, travel through your mobile carrier's SMS/MMS service, exactly as with any other messaging app. SMS Translator does not route them through any server of its own.
- **Translation:** When you view or translate a message, the translation occurs 100% locally on your device. Message contents are never transmitted across the network for translation.
- **Storage:** Messages are stored in the standard Android system telephony database on your device.

### B. Photos You Attach
- **How you pick them:** When you attach a photo, SMS Translator uses Android's system photo picker. The app only receives the photo you select; it does **not** request access to your photo library or storage.
- **Processing:** The selected photo is resized and compressed **on your device** so it fits your carrier's size limit, then sent as an MMS to the recipients you chose.
- **Storage:** Sent and received pictures are stored in the standard Android system telephony database, like your other messages. When you open an attachment in another app, a temporary copy is placed in SMS Translator's private cache so that app can display it.

### C. Phone State (`READ_PHONE_STATE`)
- **Purpose:** To let you choose which SIM card sends a message on dual-SIM phones, and to recognize your own phone number so group picture messages are filed in the right conversation.
- **Processing:** This information is used only on your device and is never stored outside Android's own records or transmitted.

### D. Contacts (`READ_CONTACTS`)
- **Purpose:** To associate phone numbers with your contacts and display familiar contact names and profile pictures in conversation lists.
- **Processing:** Contact lookups occur entirely in-memory and on-device. Your contact list is never uploaded or shared.

### E. Blocked Numbers & Spam Protection
- **Purpose:** To filter unwanted messages and block spam numbers.
- **Processing:** Blocked numbers are stored in a local SQLite database on your device and synchronized with Android's system-level blocked number provider (`BlockedNumberContract`).

### F. Notifications (`POST_NOTIFICATIONS`)
- **Purpose:** To notify you of incoming text messages and translation status.

### G. Translation Language Packs
- **Purpose:** On-device translation needs a language pack for each language (about 30 MB each). SMS Translator downloads these packs from Google's servers when you choose them in Settings or during setup.
- **Processing:** Only the request for the language pack is sent. **No message content is ever included.**

---

## 3. Google Services & Diagnostics

### Firebase Crashlytics
To monitor application stability and fix bugs, SMS Translator uses **Firebase Crashlytics** (provided by Google LLC).
- **What is collected:** Anonymous diagnostic data, including crash stack traces, app version, operating system version, device model, and free RAM/disk space.
- **Zero Personal Identifiable Information (Zero PII):** Our crash reporting configuration strictly strips and excludes all personal data. **No SMS message bodies, phone numbers, contact names, or one-time passcodes (OTPs) are ever transmitted to Crashlytics.**
- For more details, review Google's Privacy Policy: [https://policies.google.com/privacy](https://policies.google.com/privacy).

### Google ML Kit (on-device translation)
Translation runs entirely on your device with **Google ML Kit**. Like other Google SDKs, ML Kit sends Google anonymous diagnostic and usage information so Google can keep it working well.
- **What is sent:** Device information (manufacturer, model, Android version), app package name and version, a per-installation identifier that is not intended to identify you or your device, performance metrics, error codes, the language pair you translate between, and the language ML Kit detected for a message.
- **What is never sent:** The text of your messages, their translations, phone numbers, or contact names.
- This data is encrypted in transit and is not shared with third parties. See Google's description: [https://developers.google.com/ml-kit/android-data-disclosure](https://developers.google.com/ml-kit/android-data-disclosure).

---

## 4. Data Sharing and Disclosure

We do **not** sell, rent, disclose, or share any personal data with third parties. Apart from the anonymous Google diagnostics described in Section 3, we use no analytics trackers, advertising networks, or data brokers.

---

## 5. Data Retention, Security, and Deletion

- **Local Storage:** All app preferences, translation history, and blocked numbers reside exclusively in protected private app storage on your device.
- **Deletion:** You can delete individual messages or entire conversations at any time directly from the app, which removes them from your device.
- **App Data Clear:** You can permanently clear all local application data or uninstall the application at any time through Android Settings (**Settings > Apps > SMS Translator > Storage > Clear Data**).

---

## 6. Children's Privacy

SMS Translator is not directed to children under the age of 13, and we do not knowingly collect personal information from children.

---

## 7. Changes to This Privacy Policy

We may update our Privacy Policy from time to time. Any changes will be posted on this page with an updated "Last Updated" date.

---

## 8. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy or your data, please contact us:
- **Email:** slava.v.guskov@gmail.com