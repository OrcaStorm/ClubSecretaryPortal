# Secretary Club Tracker

A modern, feature-rich web application for tracking student volunteer hours, club points, and achievement tiers for any school club or organization.

[![Launch Tracker](https://img.shields.io/badge/🚀_Launch-Club_Tracker-6366f1?style=for-the-badge)](https://YOUR_USERNAME.github.io/REPO_NAME/)

![Club Tracker](https://img.shields.io/badge/status-active-success.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

## ✨ Features

### 📊 Member Management
- Add and manage club members with student IDs and grade levels
- Track individual member profiles with detailed activity history
- Search and filter by name, ID, grade, or achievement tier
- Quick action buttons for instant point tracking

### ⏱️ Hours & Points Tracking
- **Volunteering**: Direct service hour logging (1 hr = 1 service hr)
- **Workshops/Events**: 2 points per attendance
- **Socials/Meetings**: 1 point per attendance
- **Automatic Conversion**: 4 points = 1 club hour (max 5 club hours per semester)
- Bulk logging for group activities and meeting attendance

### 🏆 Achievement Tiers
Three progressive achievement levels (customizable to your club's needs):
- **Active Membership Certificate**: 20 total hrs (15+ service hrs)
- **Senior Graduation Cord**: 25 total hrs (20+ service hrs, Seniors only)
- **Recognition Pin**: 30+ total hrs (25+ service hrs)

### 💾 Data Management
- **Local Browser Storage**: All data saved automatically in your browser
- **Export Backup**: Download complete data as JSON for backup/transfer
- **Import Backup**: Restore data on any device or browser
- **Export CSV**: Generate reports for Excel/Google Sheets

### 🎨 Modern UI/UX
- Clean, professional interface with Tailwind CSS
- Fully responsive design (mobile, tablet, desktop)
- Real-time statistics dashboard
- Intuitive modal-based workflows
- Toast notifications for user feedback

## 🚀 Quick Start

### Option 1: Use Online (Instant - No Download)
**[🚀 Launch the Tracker Now](https://YOUR_USERNAME.github.io/REPO_NAME/)**

Your data stays private in your browser - nothing is sent to any server!

### Option 2: Download and Use Offline
1. Download `index.html` from this repository
2. Open it in any modern web browser
3. Start tracking immediately - no setup required!

### Option 3: Deploy to Your Own Hosting
Upload `index.html` to any static web host:
- Your own GitHub Pages
- Netlify
- Vercel
- Traditional web hosting (via FTP)

No build process, no dependencies, no server required.

## 📖 How to Use

### Adding Members
1. Click **"Add Member"** button
2. Enter student name, ID, and grade level
3. Member appears in the roster instantly

### Logging Activities

**Quick Point Bumps:**
- Use **+1 Pt** button for meetings/socials
- Use **+2 Pts** button for workshops/events

**Bulk Logging:**
1. Click **"Quick Log"** button
2. Select activity type (volunteering/workshop/social)
3. Enter event details
4. Check off all attending members
5. Submit to log for everyone at once

### Viewing Member Details
- Click any member name to view full activity history
- See detailed breakdown of hours, points, and tier progress
- Delete individual log entries if needed

### Backup & Transfer

**To backup your data:**
1. Click **"Backup/Export"** dropdown
2. Select **"Export Backup"**
3. Save the `.json` file safely

**To transfer between computers:**
1. Export backup from Computer A
2. Transfer the `.json` file (email, USB drive, cloud storage)
3. On Computer B, click **"Import Backup"**
4. Select your backup file

**For reports:**
- Use **"Export CSV Report"** for Excel/Google Sheets

## 🔧 Technical Details

### Built With
- **Pure HTML/CSS/JavaScript** - No frameworks, no build tools
- **Tailwind CSS** (via CDN) - Modern utility-first styling
- **Font Awesome** (via CDN) - Icon library
- **localStorage API** - Browser-based data persistence

### Browser Compatibility
Works in all modern browsers:
- Chrome/Edge (recommended)
- Firefox
- Safari
- Opera

Requires JavaScript enabled.

### Data Storage
- Data stored locally in browser using `localStorage`
- No external servers or databases
- No internet connection required after initial load (CDNs cached)
- Data persists until browser cache is cleared

### Calculation Rules
```javascript
// Point Conversion
4 points = 1 club hour
Max conversion: 20 points = 5 club hours per semester

// Achievement Tiers (Customizable)
Active Certificate:   20 total hrs (15+ service)
Senior Cord:          25 total hrs (20+ service, Seniors only)
Recognition Pin:      30+ total hrs (25+ service)

// Total Hours Formula
Total Club Hours = Service Hours + Converted Club Hours
```

## 📋 Club Hours Guidelines

| Activity Type | Points | Service Hours |
|--------------|--------|---------------|
| Volunteering | 0 | Actual time logged |
| Workshop/Event | 2 pts | 0 |
| Social/Meeting | 1 pt | 0 |

**Example:**
- 18 service hours from volunteering
- 12 points from workshops (6 events × 2 pts)
- 4 points from meetings (4 meetings × 1 pt)
- Total: 16 points → 4 club hours
- **Final: 18 + 4 = 22 total club hours** ✅ Active Certificate achieved!

## 🛡️ Privacy & Security

- ✅ All data stays on your device
- ✅ No data collection or tracking
- ✅ No external servers or databases
- ✅ No user accounts or authentication required
- ✅ Complete offline functionality after initial load

## 📱 Mobile Support

Fully responsive design optimized for:
- Smartphones (portrait & landscape)
- Tablets
- Desktop monitors

## 🎓 Perfect For Any Club

This tracker is universally designed for:
- Service clubs (Key Club, Interact, NHS, etc.)
- Honor societies
- Student government
- Academic clubs
- Special interest clubs
- Any organization tracking member participation

**Customize the achievement tiers and point values to match your club's requirements!**

## 🤝 Contributing

This is a self-contained single-file application. To modify:
1. Edit `club_tracker.html` directly
2. Test in your browser
3. Submit pull requests for improvements

## 📄 License

MIT License - feel free to use, modify, and distribute for your school or organization.

## 💡 Tips & Best Practices

1. **Regular Backups**: Export JSON backups weekly or after major events
2. **CSV Reports**: Export CSV at end of each semester for records
3. **Browser Choice**: Stick to one browser for consistency
4. **Clear Instructions**: Train all club officers on the backup/restore process
5. **Multiple Devices**: Use Import/Export to sync between school and home computers

## 🐛 Troubleshooting

**Data disappeared after clearing browser:**
- Import your most recent backup JSON file

**Can't see some members:**
- Check your search and filter settings
- Click "All Grades" and "All Achievement Tiers"

**Import not working:**
- Ensure you're using a backup file (`.json`) not a CSV report
- Check that the file isn't corrupted

## 📞 Support

For issues, suggestions, or questions, please open an issue on GitHub.

---

**Made with ❤️ for student club secretaries everywhere**
