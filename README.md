# 9xank_trapdeliveries — 9xdevelopmentz

**9xank_trapdeliveries** is a realistic trap delivery system built for FiveM roleplay servers.
It focuses on immersion, replayability, and security: negotiation and counter-offers, customer relationship progression, tiered clients, dynamic demand, car-based meets, and hardened server-side checks to prevent exploits.

> **Purchase + Support**
> Join the Discord to purchase, receive your license key, and get setup help:
> **Discord:** https://discord.gg/U9BGvErkys

---

## ✅ Core Features

### Immersive Delivery Flow
- **Car-based “pad meets” only** (NPC walks to driver side)
- **Interact from inside vehicle**
- Short-range delivery blips + visible zone radius
- NPC walks away cleanly after handoff
- Phone UI properly closes/holsters on Close & Accept
- Player can walk or drive while phone is open

### Negotiation + Buyer Personalities
- Buyers can **counter-offer** or send new offers
- Buyer personalities affect:
  - tips
  - order size
  - pricing behavior

### Relationship / Reputation System
- **Per-customer relationship (0–100%)**
- Tier progression: **Low → Medium → High clients**
- Higher relationships unlock:
  - better tips
  - larger quantities
  - more and better contacts
- Progressive contact cap up to **20 total contacts**

### Dynamic Demand & Pricing
- Item demand shifts based on what’s being sold
- Prices adjust with demand, buyer tier, and personality

---

## 🔒 Security / Anti-Exploit (Support-Proofed)
- Per-order security token (anti-replay)
- Strict stage/state validation
- Rate limiting on sensitive events
- Double-payout prevention
- Optional anti-teleport / abnormal speed detection
- Optional Discord webhook logging (payouts + flags)

---

## 📌 Requirements
- **ox_lib**
- **oxmysql**
- Framework:
  - **QBCore** or **ESX**
- Inventory:
  - **qb-inventory** or **ox_inventory**

---

## 📥 Installation (High-Level)
> Full step-by-step installation and live support are provided after purchase in Discord.

1) Place the resource in:

2) Ensure it in `server.cfg`:
```cfg
ensure 9xank_trapdeliveries


🔑 License System

This script uses a non-invasive license gate (no obfuscation).

Each customer receives a unique key.

Keys are validated server-side on start.

If your key is missing or invalid, the script will show:

Trap phone offline (license)

Keep your license key private.

📟 Discord Webhook Logging (Optional)

Logs:

Player identifiers

Item sold + quantity

Tip + payout totals

Delivery coordinates

Security flags (invalid state, token mismatch, abnormal movement, etc.)

🛰️ Anti-Teleport / Speed Detection (Optional)

When enabled, the script can detect:

impossible speed spikes

large position jumps during delivery actions

Actions on detection are configurable:

log only

cancel order

optional drop (recommended OFF by default)

⚙️ Configuration

After purchase, you can configure:

payout and tip scaling

relationship growth speed

tier unlock thresholds

contact cap progression

demand shift rates

cooldowns

logging and security thresholds

🧪 Troubleshooting
Script says “Trap phone offline (license)”

Confirm this line exists in server.cfg:

setr 9xank_trapdeliveries_key "YOUR_KEY_HERE"


Restart the server fully

If it still fails, open a support ticket in Discord with a server console screenshot

Deliveries won’t complete

Delivery flow is validated for security:

accept → arrive/ping → meet → complete

Skipping steps or calling events out of order will be blocked.

🧩 Support & Updates

All support, updates, and announcements are handled through Discord.

Discord: https://discord.gg/U9BGvErkys

📜 Terms

Server use only (no reselling or re-uploading)

No leaking or redistribution

Support is provided only for unmodified versions unless approved
