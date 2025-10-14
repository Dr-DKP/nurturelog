# 👶 Baby Care Tracker - Complete PWA

A comprehensive Progressive Web App for tracking your baby's feeding, sleep, health, milestones, and more. Features pediatric-approved guidelines and works 100% offline.

## ✨ Features

### Core Tracking
- **Smart Feeding Timer** - Auto-scheduling with live countdown
- **Sleep Tracker** - Duration tracking with quality notes
- **Diaper Log** - Track output with health indicators
- **Health Records** - Temperature, weight, medicine logs
- **Pumping Tracker** - Log breast milk pumping sessions
- **Tummy Time** - Track daily tummy time with goals
- **Milestone Tracker** - CDC-approved developmental milestones

### Smart Features
- **Missed Feeding Alerts** - Visual warnings when feedings are overdue
- **Breast Milk Flow Calculator** - Estimate intake by age (3-10ml/min)
- **Auto-Schedule Generation** - Creates full-day feeding schedule
- **Age-Based Guidelines** - Automatic recommendations as baby grows
- **Dark Mode** - Perfect for night feedings
- **Comprehensive Care Guide** - Midwife-approved medical information

### Data Management
- **100% Offline** - Works without internet
- **Local Storage** - All data stays on your device
- **Export Options** - JSON backup & Excel CSV export
- **Multi-format Reports** - Perfect for pediatrician visits

---

## 📱 Installation (PWA)

### ⚠️ IMPORTANT: HTTPS Requirement

**PWAs ONLY work on HTTPS or localhost.** Opening the file directly (`file://`) will NOT enable PWA features or show the install button.

### Quick Deploy Options:

#### Option 1: GitHub Pages (Recommended - Free & Easy)

1. Create a new GitHub repository
2. Upload these files:
   - `baby_tracker_enhanced.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.svg`
   - `icon-512.svg`
3. Go to Settings → Pages
4. Select "Deploy from main branch"
5. Visit `https://yourusername.github.io/repo-name/baby_tracker_enhanced.html`
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

Then visit: `https://localhost:8000/baby_tracker_enhanced.html`

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
3. **View Schedule** - See full day timeline with progress
4. **Check Stats** - Today's summary and weekly analytics
5. **Read Care Guide** - Access medical information anytime

### Key Features

**Smart Scheduling:**
- Feeds at 8:00 AM → Next automatically schedules at 10:30 AM (2.5h interval)
- Miss a feeding? Get alerted with options to log or skip
- Schedule regenerates after each feeding

**Milk Flow Calculator:**
- Settings → Milk Flow Rate
- Choose age-appropriate rate (3-10ml/min)
- Auto-estimates intake: "15 min = ~75ml"

**Pumping Tracker:**
- Log pump sessions with time and amounts
- Track left/right breast separately
- Monitor total milk stash

**Tummy Time:**
- Start/stop timer
- Track daily totals
- Age-based goal recommendations

**Milestones:**
- CDC developmental checklist
- Track physical, social, language milestones
- Perfect for pediatrician visits

---

## 📊 Data & Privacy

- **100% Local** - All data stored on your device only
- **No Account Required** - No sign-up, no cloud
- **No Tracking** - Zero analytics or data collection
- **Exportable** - Back up anytime to JSON or CSV
- **Secure** - Data never leaves your device

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
baby-tracker/
├── baby_tracker_enhanced.html  # Main app (open this)
├── manifest.json                # PWA manifest
├── sw.js                        # Service worker
├── icon-192.svg                 # App icon (192x192)
├── icon-512.svg                 # App icon (512x512)
└── README.md                    # This file
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
A: Currently single-device. Future update may add sync. For now, use Export/Import to transfer data.

**Q: Is my data safe?**
A: All data stays on your device. No cloud, no accounts, no tracking.

**Q: Can I print reports?**
A: Yes! Export to CSV and open in Excel, or use browser print function.

**Q: Will this drain my battery?**
A: No, it's a simple HTML app with minimal resources.

---

## 🎯 Quick Start Checklist

- [ ] Deploy files to HTTPS server (GitHub Pages / Netlify)
- [ ] Open URL on your phone
- [ ] Wait 30 seconds, interact with page
- [ ] Look for "📥 Install App" button in header
- [ ] Click to install
- [ ] Open from home screen
- [ ] Complete setup
- [ ] Start tracking!

---

## 📝 Version History

**v2.0 Enhanced** (Current)
- ✅ Proper PWA with installable app
- ✅ Custom install button
- ✅ Pumping tracker
- ✅ Tummy time tracker
- ✅ Milestone tracker
- ✅ Missed feeding alerts
- ✅ Milk flow calculator
- ✅ Comprehensive care guide
- ✅ Modern gradient design
- ✅ Full offline support

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
