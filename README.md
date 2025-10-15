# 🌱 NurtureLog - Smart Baby Care Tracker

[![PWA](https://img.shields.io/badge/PWA-enabled-blue.svg)](https://developers.google.com/web/progressive-web-apps/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/demo-live-success.svg)](https://dr-dkp.github.io/nurturelog/)

A comprehensive Progressive Web App for tracking your baby's feeding schedules, sleep patterns, health records, developmental milestones, and more. Features medically accurate, pediatric-approved guidelines and works 100% offline with advanced analytics and insights.

**Perfect for:** New parents, caregivers, pediatrician visits, newborn care (0-12 months)

## ✨ Features

### Core Tracking
- **Smart Feeding Timer** - Auto-scheduling with live countdown and 45-minute tolerance
- **Sleep Tracker** - Duration tracking with quality notes
- **Diaper Log** - Track output with health indicators and timestamps
- **Health Records** - Temperature, weight, medicine logs
- **Delete Entries** - Easily remove wrong entries with confirmation
- **Custom Time Entry** - Backdate any activity if you forgot to log

### Advanced Analytics & Insights
- **📅 Detailed Timeline View** - Day-by-day expandable history with exact timestamps
- **📊 7-Day Activity Charts** - Visual bar charts for feedings, diapers, sleep
- **🎯 Interactive Charts** - Click any bar to jump to detailed timeline for that day
- **⚡ At a Glance Widget** - Real-time status: last feeding, diaper, current sleep, schedule status
- **🧠 Smart Insights** - AI-like pattern detection:
  - Longest sleep stretch achievements
  - Average feeding intervals analysis
  - Diaper-to-feeding correlation detection
  - Low activity alerts
  - Schedule consistency score

### Data Management
- **💾 Export to CSV** - Open in Excel/Google Sheets for analysis
- **💾 Export to JSON** - Complete backup for restore/transfer
- **📅 Date Range Selection** - Export last 7 days, 30 days, or all time
- **100% Offline** - Works without internet after installation
- **Local Storage** - All data stays on your device

### Smart Features
- **Visual Timeline** - Color-coded dots and connecting lines for activity flow
- **Missed Feeding Alerts** - Visual warnings when feedings are overdue
- **Medically Accurate Flow Calculator** - Estimate intake by age (0.5-5ml/min based on research)
- **Auto-Schedule Generation** - Creates full-day feeding schedule with smart tolerance
- **Age-Based Guidelines** - Automatic recommendations as baby grows
- **Comprehensive Care Guide** - Midwife-approved medical information

---

## 📱 Installation (PWA)

### ⚠️ IMPORTANT: HTTPS Requirement

**PWAs ONLY work on HTTPS or localhost.** Opening the file directly (`file://`) will NOT enable PWA features or show the install button.

### Quick Deploy Options:

#### Option 1: GitHub Pages (Recommended - Free & Easy)

1. Create a new GitHub repository
2. Upload these files:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.svg`
   - `icon-512.svg`
3. Go to Settings → Pages
4. Select "Deploy from main branch"
5. Visit `https://yourusername.github.io/repo-name/`
6. **Install button will now appear!**

#### Option 2: Netlify Drop (Easiest - No Account Initially)

1. Visit https://app.netlify.com/drop
2. Drag all files into the drop zone
3. Get instant HTTPS URL
4. Open URL on your phone
5. **Install button will appear!**

#### Option 3: Local HTTPS Server (For Testing)

**Using Python:**
```bash
# Generate self-signed certificate (one time)
openssl req -x509 -newkey rsa:4096 -keyout key.pem -out cert.pem -days 365 -nodes

# Run HTTPS server
python3 -m http.server 8000 --bind 0.0.0.0
```

**Using Node.js:**
```bash
npx http-server -S -C cert.pem -K key.pem -p 8000
```

Then visit: `https://localhost:8000/`

---

## 📲 Installing on Your Device

### Android (Chrome)

Once served over HTTPS:

1. **Automatic Prompt**: After 30 seconds, Chrome may show install banner
2. **Manual Install**:
   - Tap the "📥 Install App" button in the header
   - OR: Menu (⋮) → "Install app" or "Add to Home screen"
3. App will install to your home screen like a native app!

### iPhone (Safari)

1. Open the page in Safari
2. Tap the Share button (square with arrow)
3. Scroll down and tap "Add to Home Screen"
4. Tap "Add"

### Desktop (Chrome/Edge)

1. Look for install icon (⊕) in address bar
2. Click to install
3. App opens in its own window

---

## 🚀 Usage

### First Time Setup
1. Enter baby's name and birthdate
2. Choose feeding interval (2-3 hours for newborns)
3. Set first feeding time
4. Start tracking!

### Daily Use
1. **Monitor the Timer** - Large countdown shows time until next feeding
2. **Quick Actions** - One-tap buttons for Feed, Sleep, Diaper, Health
3. **At a Glance Widget** - Quick status of all recent activities
4. **View Timeline** - Click on any day in charts to see detailed breakdown
5. **Check Insights** - See smart pattern detection and recommendations
6. **Export Data** - Backup or prepare reports for pediatrician visits

### Key Features

**Smart Scheduling:**
- Feeds at 8:00 AM → Next automatically schedules at 10:30 AM (2.5h interval)
- 45-minute tolerance window reduces false "missed" alerts
- Schedule regenerates after each feeding
- Real-time status indicator (on track/feeding soon/behind)

**Interactive Timeline:**
- Click any bar in the 7-day charts
- Automatically switches to Activity tab
- Expands and scrolls to that day's detailed timeline
- See exact times for every feeding, diaper, sleep

**Smart Insights:**
- "Best Sleep: 6.5h! Great progress!"
- "Feeding every 3.2h on average"
- "Baby usually needs diaper change within 30min after feeding"
- "Only 2 feedings today - did you forget to log?"
- "Your feeding schedule is very consistent!"

**Export for Doctor Visits:**
- Stats Tab → Export Data
- Choose date range (7 days, 30 days, all time)
- Export to CSV for Excel analysis
- Export to JSON for complete backup

---

## 📊 Data & Privacy

- **100% Local** - All data stored on your device only
- **No Account Required** - No sign-up, no cloud
- **No Tracking** - Zero analytics or data collection
- **Exportable** - Back up anytime to JSON or CSV
- **Secure** - Data never leaves your device
- **Safe Updates** - localStorage preserved when app updates

---

## 🔧 Troubleshooting

### "Install App" Button Doesn't Show

**Possible Reasons:**
1. ❌ **Not using HTTPS** - File must be on HTTPS server or localhost
2. ❌ **Already installed** - Check your home screen/app drawer
3. ❌ **Browser doesn't support** - Use Chrome/Edge (Android) or Safari (iOS)
4. ❌ **Not engaged enough** - Chrome requires 30 seconds on page + one interaction

**Solutions:**
- Deploy to GitHub Pages or Netlify (see above)
- Use local HTTPS server
- Wait 30 seconds and click/scroll on the page
- Check browser console for errors (F12 → Console)

### Charts Not Clickable

**Solution:**
- Ensure JavaScript is enabled in browser
- Try refreshing the page
- Check browser console for errors

### Export Not Downloading

**Solution:**
- Check browser download permissions
- Ensure pop-ups are not blocked
- Try different browser if issue persists

### App Won't Open from File

PWAs don't work from `file://` protocol. Must be served over HTTP/HTTPS.

### Service Worker Not Registering

Check:
1. All files in same directory
2. Served over HTTPS or localhost
3. Browser console for specific errors

---

## 📁 File Structure

```
nurturelog/
├── index.html          # Main app file
├── manifest.json       # PWA manifest
├── sw.js              # Service worker (v7)
├── icon-192.svg       # App icon (192x192)
├── icon-512.svg       # App icon (512x512)
└── README.md          # This file
```

**Note:** PNG icons are recommended but SVG works fine for testing. For production, convert SVGs to PNGs:
- 192x192 pixels (icon-192.png)
- 512x512 pixels (icon-512.png)

---

## 🆘 Support & Feedback

### Common Questions

**Q: Can I use this without internet?**
A: Yes! Once installed, works 100% offline.

**Q: Can I share with my partner?**
A: Currently single-device. Use Export/Import to transfer data between devices via JSON backup.

**Q: Is my data safe during updates?**
A: Yes! Your activity data is in localStorage (permanent), while app code is in cache (updateable). Updates never delete your data.

**Q: Can I print reports?**
A: Yes! Export to CSV and open in Excel, or use browser print function.

**Q: Will this drain my battery?**
A: No, it's a lightweight HTML app with minimal resources.

**Q: How do I backup my data?**
A: Go to Stats tab → Export Data → Export to JSON. Save the file somewhere safe.

---

## 🎯 Quick Start Checklist

- [ ] Deploy files to HTTPS server (GitHub Pages / Netlify)
- [ ] Open URL on your phone
- [ ] Wait 30 seconds, interact with page
- [ ] Look for "📥 Install App" button in header
- [ ] Click to install
- [ ] Open from home screen
- [ ] Complete setup (baby name, birthdate, feeding interval)
- [ ] Start tracking activities
- [ ] Explore timeline, charts, and insights
- [ ] Export data regularly for backup

---

## 📝 Version History

**v3.0 Advanced** (Current)
- ✅ Detailed timeline with day-by-day expandable sections
- ✅ Interactive clickable 7-day charts
- ✅ "At a Glance" quick stats widget with real-time updates
- ✅ Smart pattern insights (sleep, feeding, diaper analysis)
- ✅ Export to CSV and JSON with date range selection
- ✅ Delete wrong entries with confirmation
- ✅ 45-minute feed tolerance (reduced false alerts)
- ✅ Visual timeline with colored dots and connecting lines
- ✅ Click charts to navigate to detailed timeline
- ✅ Modern gradient design with smooth animations
- ✅ Full offline support with service worker v7

**v2.0 Enhanced**
- ✅ Proper PWA with installable app
- ✅ Custom install button
- ✅ Missed feeding alerts
- ✅ Milk flow calculator
- ✅ Comprehensive care guide
- ✅ Full offline support

**v1.0 Initial**
- ✅ Basic tracking (feed, sleep, diaper, health)
- ✅ Simple scheduling
- ✅ Local storage

---

## 🙏 Credits

Built with ❤️ for new parents everywhere.

**Medical Guidelines:**
- CDC Milestone Tracker
- WHO Growth Standards
- AAP Safe Sleep Guidelines
- Evidence-based pediatric care

**No data collection • No ads • No tracking • Just parenting tools**

---

## 📜 License

Free to use, share, and modify. No attribution required.

**Remember:** This app is a tracking tool, not medical advice. Always consult your pediatrician for health concerns.

---

## 🚀 Ready to Start?

1. **Deploy** to GitHub Pages or Netlify
2. **Open** on your phone
3. **Install** as app
4. **Track** your baby's journey!

Happy parenting! 👶💕

---

## 🔍 Keywords & Topics

**For GitHub Discovery:**
baby-tracker • progressive-web-app • newborn-care • pediatric-health • parenting-app • feeding-tracker • sleep-tracker • offline-first • medical-tracking • baby-care • infant-health • pwa • breastfeeding • baby-monitor • childcare • newborn-tracking • baby-journal • parenting-tools • baby-log • healthcare • baby-analytics • smart-insights • data-export • timeline-view

**Technologies:**
JavaScript • PWA • Service Worker • LocalStorage • Responsive Design • Mobile-First • Offline Capable • HTML5 • CSS3 • Data Visualization • Pattern Recognition
