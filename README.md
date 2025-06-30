Polygon Validator Monitoring Tool

This is a lightweight, containerized monitoring tool for tracking Polygon validator node performance. It monitors critical metrics such as checkpoints signed/proposed, Bor and Heimdall sync status, and alerts the operator if any issues arise. Designed for reliability and easy deployment via Docker, the tool helps ensure optimal uptime and network participation for validators.

Features

- Tracks validator activity (signed/proposed checkpoints)
- Monitors sync status of Bor and Heimdall nodes
- Sends real-time alerts via Telegram for:
- Missed checkpoints
- Out-of-sync Bor or Heimdall nodes
- Easy configuration through a single file
- Dockerized for smooth deployment


Project Structure

.
├── .env                        # Environment variables (Telegram Bot, RPCs)
├── config.js                  # Project configuration (Validator address, RPCs, etc.)
├── index.js                   # Core monitoring logic
├── Dockerfile                 # Containerization script
├── package.json               # Node.js dependencies and metadata
└── README.md                  # Documentation (You are here)
