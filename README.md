# YYYHH (Hall8) & JCH Student Residence Website

A welcoming website for student residents to connect with their floor communities and join hall activities.

## 🎯 Features

- **Welcome Section**: Warm greeting and introduction to the residence community
- **Floor Groups**: QR codes for each floor's WeChat groups
- **Activities**: QR codes for various hall activities (DIY, sports, social events)
- **Responsive Design**: Works perfectly on desktop and mobile devices
- **Modern UI**: Beautiful gradients, animations, and hover effects

## 📁 File Structure

```
residence/
├── index.html          # Main website file
├── styles.css          # CSS styling
├── logo.png           # Residence logo
├── code.jpg           # Example QR code (template)
├── qr-codes/          # Organized QR code folder
│   ├── floor_1.jpg    # Floor QR codes
│   ├── floor_2.jpg
│   ├── ...
│   ├── diy_workshop.jpg # Activity QR codes
│   ├── badminton.jpg
│   └── ...
└── README.md          # Documentation
```

## 🔄 How to Update QR Codes

The website is designed for easy QR code updates. Simply replace the image files with your actual QR codes:

### Floor QR Codes (in qr-codes/ folder):
- `qr-codes/floor_1.jpg` - Floor 1 WeChat Group
- `qr-codes/floor_2.jpg` - Floor 2 WeChat Group  
- `qr-codes/floor_3.jpg` - Floor 3 WeChat Group
- `qr-codes/floor_4.jpg` - Floor 4 WeChat Group
- `qr-codes/floor_5.jpg` - Floor 5 WeChat Group
- `qr-codes/floor_6.jpg` - Floor 6 WeChat Group

### Activity QR Codes (in qr-codes/ folder):
- `qr-codes/diy_workshop.jpg` - DIY Workshop
- `qr-codes/badminton.jpg` - Badminton Group
- `qr-codes/tennis.jpg` - Tennis Group
- `qr-codes/board_game.jpg` - Board Games
- `qr-codes/hiking.jpg` - Hiking Group
- `qr-codes/movie_night.jpg` - Movie Night
- `qr-codes/book_club.jpg` - Book Club
- `qr-codes/cooking.jpg` - Cooking Club
- `qr-codes/fitness.jpg` - Fitness Group

## 📱 QR Code Format

For best results, use QR code images that:
- Are square (1:1 aspect ratio)
- Have good contrast (dark pattern on light background)
- Are at least 300x300 pixels
- Include the WeChat icon like the example in `code.jpg`

## 🎨 Customization

### Adding New Activities:
1. Add a new QR card in the HTML within the activities section
2. Follow this template:

```html
<div class="qr-card">
    <div class="qr-container">
        <img src="your-activity-qr.jpg" alt="Your Activity QR Code" class="qr-code">
    </div>
    <h3 class="qr-title">🎯 Your Activity</h3>
    <p class="qr-description">Description of your activity</p>
</div>
```

### Adding More Floors:
1. Add new QR cards in the floor groups section
2. Update the image src and alt text
3. Modify the title and description

### Changing Colors:
- Main gradient: Modify the `background` property in the `body` selector
- Card colors: Update the `background` in `.qr-card`
- Text colors: Adjust color values throughout the CSS

## 🚀 Deployment

1. Upload all files to your web server
2. Ensure the logo.png and QR code images are accessible
3. The website will work immediately - no build process required!

## 📞 Support

For technical questions about the website structure, refer to the HTML comments and CSS organization. The code is well-documented and modular for easy maintenance.
