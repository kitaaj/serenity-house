# Serenity House - Legal Pages

This folder contains the Privacy Policy and Terms of Service pages for Serenity House, ready to be deployed as a GitHub Pages site.

## Contents

- `index.html` - Landing page with links to legal documents
- `privacy-policy.html` - Comprehensive Privacy Policy
- `terms-of-service.html` - Terms of Service
- `styles.css` - Shared styling

## Deployment Instructions

### Option 1: Create a new repository

1. Create a new **public** repository on GitHub (e.g., `serenity-house-legal`)
2. Copy all files from this folder to the new repo
3. Go to **Settings** → **Pages**
4. Under "Source", select **Deploy from a branch**
5. Select the `main` branch and `/ (root)` folder
6. Click **Save**
7. Your site will be live at `https://your-username.github.io/serenity-house-legal/`

### Option 2: Use a custom domain

1. Follow Option 1 steps
2. In **Settings** → **Pages**, enter your custom domain
3. Create a CNAME record pointing to `your-username.github.io`
4. Wait for DNS propagation and SSL certificate generation

## Linking from the App

After deployment, update the app to link to these pages:

### Example URLs

```
Privacy Policy: https://your-username.github.io/serenity-house-legal/privacy-policy.html
Terms of Service: https://your-username.github.io/serenity-house-legal/terms-of-service.html
```

### Update in Flutter

In `lib/screens/profile/profile_view.dart`, you can update the Privacy Policy and Terms of Service sections to open these URLs in a browser:

```dart
import 'package:url_launcher/url_launcher.dart';

// Add these constants
const String privacyPolicyUrl = 'https://your-username.github.io/serenity-house-legal/privacy-policy.html';
const String termsOfServiceUrl = 'https://your-username.github.io/serenity-house-legal/terms-of-service.html';

// Update the onTap handlers
onTap: () => launchUrl(Uri.parse(privacyPolicyUrl));
onTap: () => launchUrl(Uri.parse(termsOfServiceUrl));
```

## Customization

### Update Contact Information

Search for `@serenityhouse.app` in the HTML files and replace with your actual email addresses:

- `privacy@serenityhouse.app` - Privacy inquiries
- `legal@serenityhouse.app` - Legal/Terms inquiries
- `support@serenityhouse.app` - General support

### Update App Version

The privacy policy and terms reference version `1.0.0`. Update these when releasing new versions.

### Update Dates

The "Last updated" dates are currently set to January 2026. Update these when making changes.

## Features

- ✅ Responsive design (mobile-friendly)
- ✅ Dark mode support (follows system preference)
- ✅ Print-friendly styles
- ✅ Table of contents with anchor links
- ✅ Accessible navigation
- ✅ Professional, calming design matching app branding

## Data Categories Documented

The Privacy Policy comprehensively covers all data collected by the app:

1. **Account Data** - Email, display name, profile photo
2. **Mood Tracking** - Moods, emotions, activities, energy levels
3. **Journal Entries** - Titles, content, AI feedback, tags
4. **AI Chat** - Conversation history
5. **Preferences** - Goals, reminders, theme, streak data
6. **Achievements** - Gamification/milestone data

## Third-Party Services Disclosed

- Supabase (authentication & database)
- Google Gemini AI (chat & journal feedback)
- Formspree (feedback form)

## License

These legal documents are provided for use with Serenity House. Modify as needed for your specific requirements.

---

*Generated for Serenity House mental health support app*
