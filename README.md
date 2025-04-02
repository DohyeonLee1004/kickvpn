KickVPN

🧠 This VPN project was co-developed with ChatGPT, used as an assistant for system design, backend logic, networking, and full-stack coding.

KickVPN is a fully functional VPN MVP (Minimum Viable Product) designed for real-world usage. It includes user authentication, proxy-based traffic routing, traffic metering, a GUI client, and a reward system.

🚀 Features

✅ User Authentication (JWT-based)

✅ Traffic Proxy Server (HTTP CONNECT support)

✅ Traffic Limiting per User

✅ Premium/Free Server System

✅ Reward Code System (+MB rewards)

✅ VPN GUI Client App (Python + CustomTkinter)

✅ Traffic Log Storage & Viewer

✅ System Proxy Configuration for real IP tunneling

✅ Deployable on VPS for real IP changing

📂 Project Structure

VPNproject/
├── vpn_gui_client.py          # GUI desktop client
├── relay_proxy_server.py      # Proxy server supporting CONNECT
├── traffic_log_api.py         # FastAPI backend for login + logs
├── vpn_users.db               # SQLite DB (user data + logs)
├── README.md
└── requirements.txt           # Python dependencies

🧪 How to Run (Local Test)

Install dependencies:

pip install fastapi uvicorn python-jose[cryptography] passlib[bcrypt] pydantic requests customtkinter

Run servers:

python3 traffic_log_api.py
python3 relay_proxy_server.py

Run client:

python3 vpn_gui_client.py

Set system proxy (macOS example):

sudo networksetup -setwebproxy Wi-Fi 127.0.0.1 9001
sudo networksetup -setsecurewebproxy Wi-Fi 127.0.0.1 9001

Visit https://whatismyipaddress.com to verify VPN IP change.

📌 Notes

Developed in collaboration with GPT as the technical assistant.

All networking code, GUI logic, and server systems were reviewed and improved using AI feedback.

This project is educational and a great starting point for commercial VPN systems.
