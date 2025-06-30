Polygon Validator Monitoring Tool

A Node.js and Docker-based monitoring tool that observes and ensures the proper functioning of a Polygon validator node. It's designed to help operators detect issues like missed checkpoints and synchronization problems between Bor and Heimdall (the two key components of the Polygon network infrastructure).

🧩 Use Case
Imagine you're running a validator node on the Polygon PoS network. This tool keeps watch on it 24/7 and notifies you instantly via Telegram if something goes wrong — helping you prevent slashing, downtime, or missed rewards.

Features

- Tracks validator activity (signed/proposed checkpoints)
- Monitors sync status of Bor and Heimdall nodes
- Sends real-time alerts via Telegram for:
- Missed checkpoints
- Out-of-sync Bor or Heimdall nodes
- Easy configuration through a single file
- Dockerized for smooth deployment

  🔔 Alerts
This monitor sends alerts to Telegram using a bot. You will receive alerts if:
  Your validator misses checkpoints
  Heimdall or Bor fall out of sync
Ensure your Telegram Bot and Chat ID are configured in .env.



Project Structure

.
├── .env                        # Environment variables (Telegram Bot, RPCs)
├── config.js                  # Project configuration (Validator address, RPCs, etc.)
├── index.js                   # Core monitoring logic
├── Dockerfile                 # Containerization script
├── package.json               # Node.js dependencies and metadata
└── README.md                  # Documentation (You are here)
