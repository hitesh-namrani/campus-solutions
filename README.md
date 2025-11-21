🎓 Student Hub - Decentralized Campus Application

Student Hub is a blockchain-based Decentralized Application (DApp) designed to unify the campus experience. It leverages the Ethereum Sepolia Testnet to provide transparent, immutable, and student-governed solutions for events, notices, and grievance redressal.

🚀 Features

1. Immutable Notice Board & Events

Transparency: Official notices and event details are stored directly on the blockchain, ensuring they cannot be secretly altered or deleted.

Admin Control: Only verified university administrators can post updates via a secure Admin Panel.

Public Verification: Anyone can verify the timestamp and authenticity of an announcement on Etherscan.

2. Grievance Redressal DAO (Decentralized Governance)

Proposals: Students can submit proposals (e.g., "Fix Gym Equipment", "Extend Library Hours").

Voting Power: Students vote using $SHT (Student Hub Tokens).

Democratic Outcome: Decisions are made based on the collective vote count, ensuring administrative accountability.

3. Secure Admin Panel

Access Control: Password-protected dashboard for administrators.

Token Management: Admins can manually mint and distribute voting tokens to verified student wallets.

Content Management: Easy interface to post events and notices to the blockchain.

🛠️ Tech Stack

Blockchain: Ethereum (Sepolia Testnet)

Smart Contracts: Solidity (v0.8.20)

Frontend: HTML5, Tailwind CSS, Vanilla JavaScript

Backend: Node.js, Express.js (serves as the bridge and static file host)

Web3 Integration: Ethers.js

Wallet: MetaMask

📂 Project Structure

student-hub/
│
├── contracts/                  # Solidity Smart Contracts
│   ├── DCHToken.sol            # ERC-20 Voting Token ($SHT)
│   ├── DCHGovernance.sol       # DAO Logic (Proposals & Voting)
│   └── DCHEvents.sol           # Content Management (Events & Notices)
│
├── backend/                    # Node.js Server
│   ├── package.json            # Project Dependencies
│   └── server.js               # API & Static File Server
│
└── frontend/                   # User Interface
    └── index.html              # Main Dashboard (Glassmorphism UI)


⚙️ Prerequisites

Node.js (v14 or higher) installed.

MetaMask browser extension installed.

Sepolia ETH (for gas fees) in your MetaMask wallet. Get it from Google Cloud Faucet.

🚀 Setup & Installation

1. Clone the Repository

git clone <repository-url>
cd student-hub


2. Install Dependencies

Navigate to the backend folder and install the required packages:

cd backend
npm install


3. Configure Smart Contracts (If redeploying)

Note: The project comes pre-configured with deployed contracts. If you want to use your own:

Deploy DCHToken.sol, DCHGovernance.sol, and DCHEvents.sol using Remix IDE.

Update the contract addresses in backend/server.js.

4. Run the Application

Start the Node.js server:

node server.js


The terminal should show: Student Hub is LIVE at http://localhost:3000

5. Access the Dashboard

Open your browser and go to:
👉 http://localhost:3000

📖 How to Use

For Students

Connect Wallet: Click the "Connect Wallet" button (top-right). Ensure you are on Sepolia Testnet.

View Feed: Check the dashboard for the latest notices and upcoming events.

Vote: Go to the Grievance tab. If you have voting tokens ($SHT), you can vote "For" or "Against" active proposals.

For Admins

Access Panel: Click "Admin Access" in the sidebar.

Login: Enter the password (default: admin123).

Manage:

Post Feed/Notices: Broadcast updates to the entire campus.

Create Events: Add events with registration links and deadlines.

Distribute Tokens: Enter a student's wallet address to mint voting tokens for them.

🔗 Smart Contract Addresses (Sepolia)

Contract

Address

Description

Events

0xAfBBA52783dF148F7AF25d14c4D514Be0D2E3925

Stores feeds, notices, and event data.

Governance

0x9a0002a47E68bFb3b3e537d2DDFd3Cd586F6d72D

Manages proposals and voting logic.

Token

0x0b1e9AEc4a103a7Cae9876aF167750C9b9Fdc343

The $SHT ERC-20 token used for voting power.

👥 Team - Coding Ninjas

Hitesh Namrani - Blockchain Developer & Backend Logic

Nitin Pandey - Frontend Developer
