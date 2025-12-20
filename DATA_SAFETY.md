# Data Safety Information for Google Play

## Data Safety Form Responses

### Does your app collect or share any of the required user data types?
**No**

### Data Collection Details

| Data Type | Collected | Shared | Purpose |
|-----------|-----------|--------|---------|
| Personal info (name, email, etc.) | ❌ No | ❌ No | N/A |
| Financial info | ❌ No | ❌ No | N/A |
| Location | ❌ No | ❌ No | N/A |
| Web browsing history | ❌ No | ❌ No | N/A |
| Photos and videos | ❌ No | ❌ No | N/A |
| Audio files | ❌ No | ❌ No | N/A |
| Files and docs | ❌ No | ❌ No | N/A |
| Calendar | ❌ No | ❌ No | N/A |
| Contacts | ❌ No | ❌ No | N/A |
| App activity | ❌ No | ❌ No | N/A |
| Device or other IDs | ❌ No | ❌ No | N/A |

### Security Practices

**Is data encrypted in transit?**
N/A - No data is transmitted to external servers.

**Can users request that their data be deleted?**
N/A - No user data is collected. All transaction data is stored locally on the device and can be cleared by the user through app settings or by uninstalling the app.

**Does this app follow the Families Policy?**
Yes - The app is suitable for all ages and contains no inappropriate content.

### Data Storage

- **Location**: All data is stored locally on the user's device
- **Type**: SharedPreferences (encrypted by Android system)
- **Retention**: Data persists until user clears app data or uninstalls
- **Access**: Only the Xpensio app can access this data

### Permissions Used

| Permission | Purpose | Required |
|------------|---------|----------|
| POST_NOTIFICATIONS | Send daily expense reminders | Optional |
| VIBRATE | Haptic feedback for transactions | Optional |
| WAKE_LOCK | Ensure reminders are delivered | Optional |

### Third-Party Libraries

| Library | Purpose | Data Collected |
|---------|---------|----------------|
| AndroidX Compose | UI Framework | None |
| AndroidX Navigation | Screen navigation | None |
| Google Play Services Auth | SMS Retriever (optional, not used for data collection) | None |

---

## Summary for Data Safety Form

✅ **No data collected**
✅ **No data shared with third parties**
✅ **All data stored locally on device**
✅ **No account required**
✅ **No analytics or tracking**
✅ **No advertising SDKs**

