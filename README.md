# Sketch Pro Dashboard

A dynamic, multi-market dashboard designed for TV display with real-time performance metrics and trend visualization.

![Dashboard Preview](preview.png)

## Features

✨ **Multi-Market Support** - Display multiple markets side-by-side with individual performance cards
📊 **Dynamic Trending Graph** - Combined sparkline showing all markets' monthly asset trends
🎨 **Color-Coded Metrics** - Visual indicators for ROI and NPS score performance
📈 **Auto-Calculated Totals** - Automatically sums assets and savings across all markets
🏆 **Dynamic Rankings** - Top performing markets list updates based on monthly assets
📺 **TV-Optimized** - Clean, readable design perfect for wall-mounted displays

## Live Demo

[View Dashboard](https://yourusername.github.io/sketch-pro-dashboard/)

## Quick Start

### View Locally

1. Download all files
2. Open `index.html` in your browser
3. That's it!

### Customize Data

Edit the `marketsData` object in `index.html` (starting around line 270) to update:
- Market names
- Performance metrics
- Monthly trends
- Flags and visual elements

## Data Structure

Each market includes:
- **Monthly Metrics**: ROI, Savings, Assets (with trend indicators)
- **Complexity Breakdown**: High/Mid/Low complexity percentages with average days
- **Utilization**: AI usage and team utilization percentages
- **YTD Performance**: Total assets, savings, ROI, and NPS score
- **Trend Data**: 12 monthly data points for sparkline visualization

## Deployment on GitHub Pages

### Step 1: Create Repository
1. Go to [GitHub](https://github.com)
2. Click "New Repository"
3. Name it `sketch-pro-dashboard`
4. Make it Public
5. Click "Create Repository"

### Step 2: Upload Files
1. Click "uploading an existing file"
2. Drag and drop all files:
   - `index.html`
   - `README.md`
   - `Sketch-Pro-data-multimarket.xlsx` (optional)
3. Click "Commit changes"

### Step 3: Enable GitHub Pages
1. Go to repository Settings
2. Click "Pages" in the left sidebar
3. Under "Source", select "main" branch
4. Click "Save"
5. Your dashboard will be live at: `https://yourusername.github.io/sketch-pro-dashboard/`

## Adding New Markets

To add a new market to the dashboard:

1. Open `index.html`
2. Find the `marketsData` object (around line 270)
3. Add a new market entry:

```javascript
'Germany': {
    'market-flag': 'https://upload.wikimedia.org/wikipedia/en/b/ba/Flag_of_Germany.svg',
    'monthly-roi': '1.9',
    'monthly-saving': '11,500',
    'monthly-arrow': 'up',
    'monthly-assets': '38',
    'monthly-assets-difference': '8',
    'monthly-high-complexity': '60',
    'monthly-mid-complexity': '28',
    'monthly-low-complexity': '12',
    'monthly-high-complexity-days': '3.7',
    'monthly-mid-complexity-days': '2.3',
    'monthly-low-complexity-days': '0.7',
    'monthly-ai-usage': '28',
    'monthly-team-utilsation': '70',
    'ytd-assets-total': '17,200',
    'ytd-savings-total': '22,300',
    'ytd-roi-total': '2.8',
    'market-nps-score': '84',
    'monthly-trend': [18, 21, 24, 27, 30, 32, 34, 35, 36, 37, 38, 38]
}
```

4. Save and refresh - the new market card will appear automatically!

## Customization

### Change Refresh Behavior
The dashboard is designed for static display. Data updates require refreshing the page or editing the HTML file.

### Modify Color Thresholds

**ROI Thresholds** (around line 290):
- Green: ≥ 2.0
- Yellow: 1.5-1.9
- Red: < 1.5

**NPS Score Thresholds** (around line 310):
- Green: ≥ 80
- Yellow: 70-79
- Red: < 70

### Update Styling
All styling is inline in the HTML. Search for specific elements by class name or data-layer attribute to modify colors, sizes, and layouts.

## Browser Compatibility

✅ Chrome, Edge, Firefox, Safari
✅ Modern Smart TVs with web browsers
✅ Tablets and desktop displays

## Technical Details

- **Pure HTML/CSS/JavaScript** - No build process required
- **SVG Graphics** - Scalable sparklines and trend visualization
- **Responsive Design** - Adapts to different screen sizes
- **No External Dependencies** - Except for flag images from Wikimedia

## File Structure

```
sketch-pro-dashboard/
├── index.html                          # Main dashboard file
├── README.md                           # This file
├── Sketch-Pro-data-multimarket.xlsx    # Example data structure (optional)
└── preview.png                         # Dashboard screenshot (optional)
```

## Support

For questions or issues:
1. Check the code comments in `index.html`
2. Verify data structure matches the expected format
3. Test in a modern browser with JavaScript enabled

## License

Free to use and modify for your projects.

## Acknowledgments

- Flag images from [Wikimedia Commons](https://commons.wikimedia.org/)
- Font: Inter (loaded from browser defaults)

---

**Made with ❤️ for Sketch Pro**
