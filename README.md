# Anti Map Collision (Standalone)

**The ultimate fix for broken map collisions in FiveM.** This script provides a seamless solution for "invisible walls" or blocked doors caused by conflicting map files (MLOs) or duplicate collision data. Instead of editing game files, simply configure the location, and the script handles the rest—allowing players to walk through the blockage smoothly.

---

## 🎥 Showcase

> **[Click here to watch the full feature showcase on YouTube](https://youtu.be/bvVFJO3cDQo)**

---

## 🔥 Key Features

Designed to fix map bugs without complex file editing:

### 🛠️ Problem Solver
* **Fixes Blocked Doors:** Perfect for when two maps use the same collision file, causing one to override the other and block entry.
* **MLO Compatibility:** Works with any custom map or interior (MLO).
* **Standalone:** Zero dependencies. Works on ESX, QBCore, or any other framework.

### ⚡ Smooth Interaction
* **Auto-Detection:** Automatically detects when a player attempts to walk through a configured doorway.
* **Seamless Movement:** Temporarily disables collision and walks the player through the obstacle, then re-enables it immediately.
* **Directional Logic:** Only activates when the player is facing and moving toward the target, preventing accidental triggers.

### ⚙️ Optimization & Config
* **Easy Setup:** Just add the coordinates (Vector4) of the problematic door in `config.lua`.
* **Highly Optimized:** runs at low MS, checking distance efficiently to ensure server performance is not impacted.

---

## 📝 Configuration Guide

Setting up a new location is simple. Open `config.lua` and add a new entry to the `Config.Positions` table.

### **Instructions:**
1.  **Stand in the Center:** Go to the blocked door or wall and stand exactly in the center of where the passage should be.
2.  **Check Heading:** Face the direction you want to walk through (the heading matters for the path calculation).
3.  **Copy Coords:** Save your position as a `vector4(x, y, z, heading)`.
4.  **Double Doors:** If it is a double door, set the position in the center between both doors.

```lua
Config.Positions = {
    -- Example: vector4(x, y, z, heading)
    vector4(-55.04, 6392.4, 31.62, 226.0),
    vector4(-424.82, 23.38, 46.26, 359.71),
}
```

## 🔗 Links & Support
- ### 🛒 Buy Now (Tebex): https://menanak47.tebex.io/package/6875367

- ### 💬 Discord Support: https://discord.gg/RKZcVwh

- ### 📺 YouTube Channel: https://www.youtube.com/@menanak47