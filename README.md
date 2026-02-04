# 💕 Valentine's Proposal 💕

A romantic interactive web application for proposing to your Valentine!

## Features

✨ **Beautiful UI** - Stunning gradient background with smooth animations
❤️ **Interactive Buttons** - "Yes" button celebrates your love, "No" button playfully runs away
🎉 **Confetti Animation** - Celebratory confetti falls when they say yes
🌹 **Rose Animation** - Floating roses appear when proposal is accepted
📊 **Backend Logging** - Python Flask server logs all responses

## Files

- `index.html` - Main HTML file with styling
- `proposal.js` - JavaScript for interactivity and animations
- `app.py` - Python Flask backend server

## How to Use

### Option 1: Simple (No Backend)
1. Just open `index.html` in your web browser
2. The full proposal experience works without the backend
3. Responses won't be logged, but animations will work perfectly

### Option 2: With Backend Logging
1. Install Python dependencies:
   ```
   pip install flask flask-cors
   ```

2. Start the Flask server:
   ```
   python app.py
   ```

3. Open `index.html` in your web browser

4. When someone clicks "Yes" or "No", the response is logged to `proposal_responses.json`

5. View statistics at: `http://localhost:5000/stats`

6. View all responses at: `http://localhost:5000/responses`

## Customization

### Change the Message
Edit the `<p class="message">` in `index.html` to personalize the proposal message.

### Change the Colors
Modify the color values in the CSS (look for hex codes like `#ff1744`)

### Change the Emojis
Replace any emoji with your preferred ones throughout the HTML

### Add Music
Add this to the `handleYes()` function:
```javascript
const audio = new Audio('romantic-song.mp3');
audio.play();
```

## API Endpoints (Backend)

- `GET /` - Server status
- `POST /proposal` - Log a proposal response
- `GET /responses` - View all responses
- `GET /stats` - View proposal statistics

## Enjoy! 💝

Good luck with your proposal! Make it memorable! 🌹✨
