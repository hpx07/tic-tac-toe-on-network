# TIC-TAC-TOE TOURNAMENT 🎮

A stealth office-friendly multiplayer Tic-Tac-Toe game with dark CMD-like appearance. Perfect for playing during work hours without drawing attention! 😎

## 🎯 Features

✅ **Quick Match Mode** - Instantly pair with available players
✅ **Tournament Mode** - Organize brackets with 2-10+ players
✅ **Live Leaderboard** - Track wins, losses, and points
✅ **Chat System** - Communicate with other players
✅ **Stealth Design** - Looks like a terminal/CMD window
✅ **100% Browser-Based** - No installation needed on client machines
✅ **Real-time Multiplayer** - Play simultaneously with colleagues
✅ **Lightweight** - Minimal resource usage

## 📋 Requirements

- **Node.js** (v14 or higher)
- **LAN Network** (all players must be on same network)
- **Modern Browser** (Chrome, Firefox, Edge, Safari)

## 🚀 Quick Start (5 Minutes Setup)

### Step 1: Install Node.js
If you don't have Node.js installed:
1. Download from: https://nodejs.org/
2. Install the LTS version
3. Verify installation: Open CMD and type `node --version`

### Step 2: Setup Game Server

1. **Extract files** to a folder (e.g., `C:\TicTacToe`)

2. **Open Command Prompt** in that folder:
   - Navigate to folder in File Explorer
   - Type `cmd` in the address bar and press Enter

3. **Install dependencies**:
   ```bash
   npm install
   ```

4. **Find your IP address**:
   ```bash
   ipconfig
   ```
   Look for "IPv4 Address" (e.g., 192.168.1.100)

5. **Start the server**:
   ```bash
   npm start
   ```

   You should see:
   ```
   ============================================================
   >> TIC-TAC-TOE TOURNAMENT SERVER
   >> Server running on port 3000
   >> Local: http://localhost:3000
   >> Network: http://YOUR_IP:3000
   ============================================================
   ```

### Step 3: Players Join

All players on the LAN open their browser and visit:
```
http://SERVER_IP:3000
```
(Replace SERVER_IP with the IP from Step 2.4)

Example: `http://192.168.1.100:3000`

## 🎮 How to Play

### Login
1. Enter any username (max 15 characters)
2. Click "CONNECT"

### Quick Match
1. Click "QUICK MATCH" button
2. System will pair you with another available player
3. Game starts automatically
4. Take turns clicking cells to place X or O
5. Win by getting 3 in a row (horizontal, vertical, or diagonal)

### Tournament Mode
1. All players join the lobby
2. Any player clicks "START TOURNAMENT"
3. System creates bracket pairs
4. All first-round matches start simultaneously
5. Winners advance to next round
6. Continue until champion is crowned!

### Scoring System
- **Win**: +3 points
- **Draw**: +1 point each
- **Loss**: 0 points

## 🎯 Game Modes Explained

### Quick Match Mode
- Instant matchmaking
- Best for casual play
- Play as many games as you want
- Points accumulate on leaderboard

### Tournament Mode
- Structured bracket system
- All players compete
- Single elimination (or multiple rounds)
- Great for organized competitions

## 💬 Chat Feature
- Click "TOGGLE CHAT" button in sidebar
- Type messages and click "SEND"
- All players can see chat messages
- Perfect for trash talk! 😄

## 📊 Leaderboard
- Automatically tracks all player stats
- Sorts by total points
- Shows wins, losses, draws
- Updates in real-time

## 🔧 Troubleshooting

### Server won't start
```bash
# If port 3000 is in use, edit server.js line 6:
const PORT = 3000;  // Change to 3001, 3002, etc.
```

### Players can't connect
1. Check firewall - allow Node.js through Windows Firewall
2. Verify all devices on same network
3. Make sure server is running
4. Try using server computer's IP address

### Game feels slow
- Check network connection
- Reduce number of active players
- Close unnecessary programs on server

## 🎨 Customization

### Change Colors (in public/index.html)
```css
/* Find these in the <style> section: */
background-color: #0C0C0C;  /* Background */
color: #00FF00;              /* Text (green) */
border: 1px solid #1E1E1E;  /* Borders */
```

### Change Port (in server.js)
```javascript
const PORT = 3000;  // Change this number
```

### Change Scoring (in server.js)
```javascript
// Find this section and modify:
winnerStats.points += 3;  // Win points
stats1.points += 1;       // Draw points
```

## 🛡️ Office Stealth Tips

1. **Window Title**: Shows "System Process Manager" (looks like work)
2. **Dark Theme**: Resembles CMD/terminal window
3. **No Bright Colors**: Subtle green on black
4. **Minimize When Boss Comes**: Alt+Tab to safety!
5. **Run on Personal Device**: If possible, use your laptop as server

## 📱 Mobile Support

Yes! The game works on mobile browsers too. Just visit the server URL on your phone while connected to the same WiFi.

## 🔒 Security Notes

- Game runs on **local network only**
- No internet connection required
- No data leaves your LAN
- No external servers involved
- Safe for corporate networks

## ⚡ Performance

- **Server RAM**: ~50MB
- **Client RAM**: ~30MB per browser tab
- **Network Usage**: Minimal (<1KB per move)
- **CPU Usage**: <1% on modern hardware

## 🎯 Best Practices

1. **Designate one stable computer as server**
2. **Keep server running throughout game session**
3. **Use wired connection for server if possible**
4. **Close chat if you want pure stealth**
5. **Set username rules** (e.g., real names vs. nicknames)

## 📞 Support

If you encounter issues:
1. Check firewall settings
2. Verify Node.js is installed correctly
3. Ensure all devices on same network
4. Try restarting server
5. Check server console for error messages

## 🎊 Tournament Ideas

### Daily Champion
- Play throughout the day
- Most points by 5 PM wins
- Winner gets coffee privilege

### Lunch Break Tournament
- Quick 8-player bracket
- 15-minute time limit
- Fast and fun!

### Team Battle
- Divide office into teams
- Team with most total points wins
- Great for team building

## 🚨 Important Notes

- **Keep volume OFF** - Game has no sounds, but browser might
- **Don't use company computers as server** - Use personal device
- **Play during breaks** - Be responsible! 😊
- **Have fun but be discreet**

## 📝 File Structure

```
TicTacToe/
├── server.js          # Main server file
├── package.json       # Dependencies
├── README.md          # This file
└── public/
    └── index.html     # Client interface
```

## 🎮 Commands Reference

```bash
# Install dependencies
npm install

# Start server
npm start

# Stop server
Ctrl + C (in terminal)

# Check Node version
node --version

# Check IP address
ipconfig (Windows)
ifconfig (Mac/Linux)
```

## 🏆 Enjoy Your Game!

Have fun and may the best player win! Remember to stay productive and only play during appropriate times. 😉

---

**Made with 💡 for office warriors everywhere by [HPX07](https://github.com/hpx07)** 


