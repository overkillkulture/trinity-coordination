# 📱 Phone Setup - 5 Minutes

## Method 1: GitHub Codespaces (EASIEST)

1. Open GitHub Mobile app on your phone
2. Navigate to this repo: `trinity-coordination`
3. Tap "Code" → "Codespaces" → "Create codespace"
4. VS Code opens in browser
5. Open Terminal (hamburger menu)
6. Type: `claude`
7. **You're connected to Trinity!**

## Method 2: Termux (Android)

```bash
# Install Termux from F-Droid (https://f-droid.org/en/packages/com.termux/)

# In Termux, run:
pkg update
pkg install git nodejs
npm install -g @anthropic-ai/claude-code

# Clone this repo:
cd ~
git clone https://github.com/overkillkulture/trinity-coordination.git
cd trinity-coordination

# Set API key:
export ANTHROPIC_API_KEY="your-key-here"

# Start Claude:
claude
```

## Method 3: a-Shell (iOS)

```bash
# Install a-Shell from App Store

# In a-Shell:
npm install -g @anthropic-ai/claude-code

# Clone repo:
git clone https://github.com/overkillkulture/trinity-coordination.git
cd trinity-coordination

# Start Claude:
claude
```

## First Mission

Once connected, ask Claude:

```
"Read the Trinity coordination hub. What's my first mission?"
```

Claude will check `.trinity/convergence_hub.json` and tell you what needs to be done.

## Test Connection

```bash
# Pull latest from desktop:
git pull

# Check what desktop Trinity is working on:
cat .trinity/computer_1_status.json

# Do your phone mission (example: test mobile site)

# Update your status:
# (Claude will help you create computer_3_phone_status.json)

# Push your update:
git add .
git commit -m "Phone: Mobile testing complete"
git push
```

---

**Welcome to Trinity!** 🌀📱⚡
