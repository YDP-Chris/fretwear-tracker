# FretWear Tracker

A mobile-first web application that tracks guitar fret wear using photo comparison and analysis. Know exactly when your frets need maintenance with data-driven recommendations.

## ✨ Features

- **Photo-based wear tracking** - Compare fret condition over time using your phone camera
- **Guided photo capture** - Overlay guides ensure consistent imaging for accurate analysis
- **Traffic light status** - Clear Green/Yellow/Red system for maintenance timing
- **Multiple guitar support** - Track unlimited guitars with individual timelines
- **Offline-first** - All data stored locally using IndexedDB
- **Mobile optimized** - Designed for phone camera capture with responsive interface
- **Export/import** - Backup and restore your guitar data

## 🎯 Use Cases

- **Guitar owners** wanting to track fret condition between setups
- **Guitar technicians** documenting wear progression for customers
- **Musicians** optimizing maintenance timing to save money and improve tone
- **Collectors** maintaining condition records for valuable instruments

## 📱 How It Works

### 1. Add Your Guitar
Register your guitar with make, model, year, and current fret condition.

### 2. Take Baseline Photos
Capture initial fret photos using the guided camera system with overlay positioning guides and lighting quality checks.

### 3. Track Over Time
Take new photos every 4-6 weeks. The app compares them to your baseline to detect wear patterns.

### 4. Get Recommendations
Receive clear status updates:
- **Green**: Good condition (6+ months until maintenance)
- **Yellow**: Monitor closely (1-6 months)
- **Red**: Schedule maintenance soon

### 5. Optimize Maintenance
Use data-driven insights to time fret work perfectly - not too early (waste money) or too late (degraded tone).

## 🚀 Getting Started

### Quick Start
1. Open the app in your mobile browser
2. Allow camera access when prompted
3. Tap "Add Your First Guitar"
4. Fill in guitar details
5. Follow guided photo capture process
6. Set calendar reminder for monthly tracking

### Photo Capture Tips
- **Lighting**: Use bright, even lighting (avoid direct sunlight or harsh shadows)
- **Positioning**: Hold guitar at eye level, align frets with guide lines
- **Consistency**: Take photos from same angle and distance each time
- **Focus**: Ensure frets are sharp and in focus before capturing

### Analysis Understanding
- **Confidence Score**: Higher percentages indicate more reliable analysis
- **Specific Findings**: Details about individual fret wear patterns
- **Timeline**: Tracks wear progression across multiple photo sessions
- **Recommendations**: Actionable guidance based on detected wear levels

## 🛠 Technical Details

### Technology Stack
- **Frontend**: Vanilla HTML/CSS/JavaScript with Tailwind CSS
- **Storage**: IndexedDB for offline photo and data persistence
- **Camera**: getUserMedia API for photo capture
- **Analysis**: Canvas-based image processing for wear detection

### Browser Support
- **iOS Safari** 12+
- **Chrome Android** 80+
- **Chrome Desktop** 80+
- **Firefox** 75+
- **Edge** 80+

### Storage Requirements
- ~5-10MB per guitar for photo storage
- Automatic image compression to JPEG format
- IndexedDB provides 50MB+ storage capacity
- Export feature for data backup

### Privacy & Security
- **No cloud storage** - All data stays on your device
- **No account required** - No personal information collected
- **Camera access** - Only used for photo capture, never transmitted
- **Local processing** - All analysis happens on your device

## 📊 Data Management

### Export Data
1. Tap menu (⋮) in top right
2. Select "Export Guitar Data"
3. Downloads JSON backup file
4. Save to cloud storage or email yourself

### Import Data
1. Tap menu (⋮) in top right
2. Select "Import Guitar Data"
3. Choose your backup JSON file
4. Data will be restored to app

### Storage Limits
- **50MB total** across all guitars and photos
- **~20-30 guitars** typical capacity
- **Compressed images** to maximize storage efficiency
- **Cleanup tools** to remove old photos if needed

## 🎸 Best Practices

### Tracking Schedule
- **New guitars**: Establish baseline immediately
- **Regular tracking**: Photos every 4-6 weeks
- **Heavy players**: Monthly photos for accurate trending
- **Light players**: Every 2-3 months sufficient

### Photo Quality
- **Same location**: Use consistent lighting and background
- **Same angle**: Position guitar and camera identically
- **Multiple shots**: Take 2-3 photos and keep the best one
- **Clean frets**: Wipe down strings before photos for clear visibility

### Maintenance Timing
- **Green status**: Monitor every 6-8 weeks
- **Yellow status**: Monitor every 3-4 weeks
- **Red status**: Schedule professional work within 2-4 weeks
- **After maintenance**: Take new baseline photos

## 🔧 Troubleshooting

### Camera Issues
- **Permission denied**: Check browser settings to allow camera access
- **Poor quality**: Clean camera lens, ensure good lighting
- **Wrong camera**: App uses back camera automatically
- **Not working**: Try refreshing page and granting permissions again

### Storage Issues
- **App slow**: Export data and clear old photos
- **Storage full**: Browser may limit IndexedDB space
- **Data lost**: Always export backup before browser updates
- **Import failed**: Check JSON file format and try again

### Analysis Accuracy
- **Inconsistent results**: Ensure consistent photo positioning
- **Low confidence**: Improve lighting or retake photos
- **False positives**: Heavy use guitars may show more sensitive detection
- **Missing wear**: Very subtle changes need time to become detectable

## 🚀 Development

### Local Development
```bash
# Serve locally
python3 -m http.server 8080
# Open http://localhost:8080

# Or with Node.js
npx http-server -p 8080
```

### Deployment
- **Static hosting**: Works on any static host (Vercel, Netlify, GitHub Pages)
- **No backend**: Pure client-side application
- **HTTPS required**: Camera access requires secure context
- **Mobile first**: Optimized for phone usage

## 🤝 Contributing

This is an open source project. Contributions welcome:

1. **Bug reports** - Found an issue? Please report it
2. **Feature requests** - Ideas for improvements
3. **Code contributions** - Submit pull requests
4. **Documentation** - Help improve guides and docs

## 📄 License

MIT License - See LICENSE file for details.

---

**Built with ❤️ by Foundry** - Autonomous AI product builder