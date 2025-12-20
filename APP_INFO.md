# Xpensio - App Information

## Basic Information

| Field | Value |
|-------|-------|
| **App Name** | Xpensio - Expense Tracker |
| **Package Name** | limenss.xpensio |
| **Version Code** | 2 |
| **Version Name** | 1.1 |
| **Min SDK** | 24 (Android 7.0) |
| **Target SDK** | 34 (Android 14) |
| **Category** | Finance |

## Developer Information

| Field | Value |
|-------|-------|
| **Developer Name** | [Your Name/Company] |
| **Developer Email** | [Your Email] |
| **Developer Website** | [Your Website - Optional] |
| **Privacy Policy URL** | [Required - Host PRIVACY_POLICY.md] |

## Technical Details

| Specification | Value |
|---------------|-------|
| **APK Size** | ~1.7 MB |
| **Supported Architectures** | arm64-v8a, armeabi-v7a, x86, x86_64 |
| **Supported Languages** | English |
| **Orientation** | Portrait |

## Permissions

| Permission | Purpose |
|------------|---------|
| `POST_NOTIFICATIONS` | Daily expense reminders |
| `VIBRATE` | Haptic feedback |
| `WAKE_LOCK` | Ensure reminder delivery |

## Features

- ✅ Offline functionality (no internet required)
- ✅ No account/login required
- ✅ No ads
- ✅ No in-app purchases
- ✅ No subscription

## Store Assets Checklist

### Required
- [ ] High-res icon (512 x 512 px, PNG, 32-bit)
- [ ] Feature graphic (1024 x 500 px, PNG or JPG)
- [ ] Phone screenshots (min 2, max 8) - 16:9 aspect ratio
- [ ] Short description (max 80 characters)
- [ ] Full description (max 4000 characters)
- [ ] Privacy policy URL

### Optional but Recommended
- [ ] 7-inch tablet screenshots
- [ ] 10-inch tablet screenshots
- [ ] Promo video (YouTube URL)

## Screenshots Suggestions

1. **Dashboard** - Show the main balance card with gradient background
2. **Add Expense** - Show the expense form with savings toggle
3. **Analytics** - Show expense by category with colorful bars
4. **Savings View** - Show the green savings bars
5. **Financial Insights** - Show the smart insights widget
6. **Categories** - Show category management screen

## Signing Information

⚠️ **Important**: The current APK is signed with a debug keystore. For production release:

1. Generate a new release keystore:
   ```bash
   keytool -genkey -v -keystore release.keystore -alias xpensio -keyalg RSA -keysize 2048 -validity 10000
   ```

2. Update `app/build.gradle` with release keystore details

3. Keep the keystore file SAFE - you'll need it for all future updates!

## Testing Checklist

- [ ] App installs correctly
- [ ] App launches without crash
- [ ] Add income works
- [ ] Add expense works
- [ ] Savings toggle works (on Add Expense)
- [ ] Analytics display correctly
- [ ] Edit transaction works
- [ ] Delete transaction works
- [ ] Convert expense to savings works
- [ ] Convert savings back to expense works
- [ ] Categories can be managed
- [ ] App works offline
- [ ] No ANR (Application Not Responding)
- [ ] Back button works correctly

