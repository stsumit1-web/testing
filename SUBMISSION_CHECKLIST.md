# Google Play Store Submission Checklist

## Pre-Submission Requirements

### 1. Google Play Developer Account
- [ ] Create Google Play Developer Account ($25 one-time fee)
- [ ] Complete identity verification
- [ ] Set up payment profile (if monetizing)

### 2. App Assets (MUST HAVE)

#### App Icon
- [ ] **High-res icon**: 512 x 512 pixels, PNG (32-bit with alpha)
  - No transparency
  - No rounded corners (Google adds them automatically)

#### Feature Graphic
- [ ] **Feature graphic**: 1024 x 500 pixels, PNG or JPG
  - Used for Play Store promotion
  - No text in unsafe zones

#### Screenshots
- [ ] **Phone screenshots**: At least 2, max 8
  - Minimum dimension: 320px
  - Maximum dimension: 3840px
  - 16:9 or 9:16 aspect ratio
  - PNG or JPG (no alpha)

### 3. Store Listing Content
- [x] Short description (80 chars max) - See STORE_LISTING.md
- [x] Full description (4000 chars max) - See STORE_LISTING.md
- [ ] App name (50 chars max) - "Xpensio - Expense Tracker"

### 4. Privacy & Data
- [ ] Privacy policy URL (REQUIRED)
  - Host PRIVACY_POLICY.md on a public URL
  - Options: GitHub Pages, your website, Firebase Hosting
- [x] Data safety form responses - See DATA_SAFETY.md

### 5. Content Rating
- [x] Content rating questionnaire - See CONTENT_RATING.md
- [ ] Complete IARC rating in Play Console

### 6. App Bundle/APK
- [x] Signed APK (Xpensio-v1.0-release.apk)
- [ ] Consider generating AAB (Android App Bundle) for smaller downloads:
  ```bash
  ./gradlew bundleRelease
  ```

---

## Play Console Setup Steps

### Step 1: Create App
1. Go to [Google Play Console](https://play.google.com/console)
2. Click "Create app"
3. Fill in:
   - App name: `Xpensio - Expense Tracker`
   - Default language: English (US)
   - App or game: App
   - Free or paid: Free
4. Accept declarations

### Step 2: Store Listing
1. Go to "Main store listing"
2. Fill in from STORE_LISTING.md:
   - Short description
   - Full description
3. Upload graphics:
   - App icon (512x512)
   - Feature graphic (1024x500)
   - Phone screenshots (min 2)

### Step 3: App Content
1. **Privacy policy**: Add your hosted URL
2. **App access**: All functionality available without special access
3. **Ads**: App does not contain ads
4. **Content rating**: Complete questionnaire (use CONTENT_RATING.md)
5. **Target audience**: 18+ (financial app)
6. **News apps**: Not a news app
7. **COVID-19 apps**: Not a COVID app
8. **Data safety**: Complete form (use DATA_SAFETY.md)
9. **Government apps**: Not a government app

### Step 4: App Release
1. Go to "Production" → "Create new release"
2. Upload Xpensio-v1.0-release.apk
3. Add release notes (use RELEASE_NOTES.md)
4. Review and roll out

---

## Post-Submission

### Timeline
- Initial review: 1-7 days (can be longer for new accounts)
- Status updates via email

### Common Rejection Reasons to Avoid
✅ Already addressed:
- No SMS permissions requested (removed sync feature)
- Privacy policy provided
- No misleading functionality
- App works offline
- No hidden charges

### If Rejected
1. Read rejection email carefully
2. Check the specific policy violation
3. Fix the issue
4. Resubmit with explanation

---

## Files in This Folder

| File | Purpose |
|------|---------|
| `Xpensio-v1.0-release.apk` | Signed release APK |
| `STORE_LISTING.md` | Store listing content |
| `RELEASE_NOTES.md` | Version 1.0 release notes |
| `DATA_SAFETY.md` | Data safety form responses |
| `CONTENT_RATING.md` | Content rating questionnaire |
| `APP_INFO.md` | App technical information |
| `SUBMISSION_CHECKLIST.md` | This checklist |

---

## Quick Commands

Generate App Bundle (recommended over APK):
```bash
cd /path/to/Calc
./gradlew bundleRelease
# Output: app/build/outputs/bundle/release/app-release.aab
```

Generate signed APK:
```bash
./gradlew assembleRelease
# Output: app/build/outputs/apk/release/app-release.apk
```

---

**Good luck with your submission! 🚀**

