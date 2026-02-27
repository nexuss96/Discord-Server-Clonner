# Discord Server Cloner

A modern, easy-to-use Discord server cloner with a clean purple/black themed interface.

## Features

✨ **Complete Server Cloning**
- Clone all roles with permissions and colors
- Clone all categories with proper structure
- Clone all text and voice channels
- Clone channel permissions and settings
- Clone messages from selected channels

🎨 **Modern Interface**
- Clean purple/black themed UI
- Easy-to-use configuration panel
- Channel selection with checkboxes
- Real-time progress logging
- Smooth scrolling

⚙️ **Customizable Options**
- Select specific channels for message cloning
- Configure message limit per channel (1-1000)
- Toggle message cloning on/off
- Select/deselect all channels quickly

## Installation

### Requirements
- Python 3.8 or higher
- Windows, macOS, or Linux

### Step 1: Install Python
Download and install Python from [python.org](https://www.python.org/downloads/)

### Step 2: Install Dependencies
Open terminal/command prompt and run:
```bash
pip install requests
```

### Step 3: Run the Application
```bash
python server_cloner.py
```

## How to Use

### 1. Get Your Discord Token
Click the "? How to get token" button in the app for detailed instructions, or:

1. Open Discord in your browser (discord.com)
2. Press `F12` to open Developer Console
3. Go to the **Console** tab
4. Paste this code and press Enter:
```javascript
const iframe = document.createElement('iframe');
console.log('Token: %c%s','font-size:16px;',
JSON.parse(document.body.appendChild(iframe)
.contentWindow.localStorage.token));
iframe.remove();
```
5. Copy the token that appears

### 2. Get Server IDs
1. Enable Developer Mode in Discord:
   - Settings → Advanced → Developer Mode (toggle ON)
2. Right-click on a server icon
3. Click "Copy ID"

### 3. Clone Your Server
1. **Enter Account Token** - Paste your Discord token
2. **Enter Source Server ID** - The server you want to clone from
3. **Enter Destination Server ID** - The empty server to clone to
4. **Click "FETCH CHANNELS"** - Load all channels from source server
5. **Select Channels** - Choose which channels to clone messages from
6. **Configure Settings**:
   - Toggle "Clone Messages" on/off
   - Set message limit per channel (default: 100)
7. **Click "START CLONING"** - Begin the cloning process

## What Gets Cloned

### Server Structure
- ✅ All roles (with permissions, colors, hoisting)
- ✅ All categories (with positions and permissions)
- ✅ All text channels (with topics, NSFW settings, slowmode)
- ✅ All voice channels (with bitrate, user limits)
- ✅ Channel permissions (role-based and user-based)

### Messages (Optional)
- ✅ Message content and embeds
- ✅ Author names and timestamps
- ✅ Attachment links
- ✅ Configurable message limit (1-1000 per channel)
- ✅ Select specific channels to clone messages from

## Important Notes

⚠️ **Before Cloning:**
- You must be a member of both servers
- You need admin permissions in the destination server (permission required on specific clone, not required most time)
- The destination server will be cleaned (all channels/roles deleted)
- Cloning may take several minutes for large servers

⚠️ **Limitations:**
- Cannot clone server icon, banner, or emojis
- Cannot clone member data or nicknames
- Attachments are linked, not re-uploaded
- Rate limits apply (automatic handling included)

⚠️ **Security Warning:**
- Never share your Discord token with anyone
- Your token gives full access to your account
- Use at your own risk
- Discord may ban accounts using automation tools

## Troubleshooting

### "Invalid token" error
- Make sure you copied the full token
- Token should be 70+ characters long
- Try getting a fresh token from Discord

### "No permission" error
- Verify you're a member of both servers
- Check you have admin permissions in destination server
- Make sure the server IDs are correct

### Cloning is slow
- This is normal for large servers
- Rate limits are automatically handled
- Do not close the application while cloning

### Channels not showing
- Click "FETCH CHANNELS" after entering token and source ID
- Verify the source server ID is correct
- Check your token is valid

## Support

For issues or questions:
1. Check the troubleshooting section above
2. Verify all requirements are met
3. Make sure you're using the latest version

## Disclaimer

This tool is for educational purposes only. Use responsibly and only on servers you own or have permission to modify. Violating Discord's Terms of Service may result in account termination.

## License

MIT License - Free to use and modify
