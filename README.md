# space_hackathon
space_hackathon
📌 Overview This project is a Cargo Stowage Management System designed to optimize storage and retrieval operations aboard the International Space Station (ISS). It automates item placement, retrieval, waste management, and cargo return planning to reduce astronaut workload by 25%.

Built with efficient algorithms, a RESTful API, and a user-friendly UI, this system ensures: ✅ Optimal 3D bin packing for cargo placement. ✅ Fast retrieval with minimal obstruction. ✅ Automated waste tracking & disposal planning. ✅ Time simulation for mission planning.

🛠️ Tech Stack Category: Technologies Backend: Python (FastAPI/Flask) / Node.js Frontend: React.js / Vue.js Database: SQLite / PostgreSQL (Optional) Containerization: Docker (Ubuntu 22.04) API: RESTful (JSON)

cargo-stowage-iss/
├── backend/ # API & Algorithms
│ ├── app/ # FastAPI/Flask/Node.js
│ ├── models/ # Database models
│ └── utils/ # Helper functions
├── frontend/ # React/Vue UI
│ ├── src/
│ └── public/
├── data/ # Sample CSV files
├── Dockerfile # Docker configuration
├── requirements.txt # Python dependencies
├── package.json # Node.js dependencies
└── README.md

🚀 Key Features & API Endpoints

Placement Recommendations Endpoint: POST /api/placement
Input: List of items & containers

Output: Optimal placements & rearrangements

Item Search & Retrieval Search: GET /api/search?itemId=001
Retrieve: POST /api/retrieve (logs usage)

Place Back: POST /api/place (updates position)

Waste Management Identify Waste: GET /api/waste/identify
Return Plan: POST /api/waste/return-plan

Time Simulation Fast Forward Days: POST /api/simulate/day

Import/Export Import Items: POST /api/import/items (CSV upload)

Export Arrangement: GET /api/export/arrangement (CSV download)

Logging View Logs: GET /api/logs
