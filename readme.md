# 🌍 Climatopia

> An AI-powered, planet-scale simulation engine for "what if" scenarios across climate, economy, and humanity.

**Built by Team T3Coders**

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Problem Statement](#problem-statement)
- [Our Solution](#our-solution)
- [Credit System & Subscriptions](#credit-system--subscriptions)
- [Architecture](#architecture)
- [Tech Stack](#tech-stack)
- [API Documentation](#api-documentation)
- [Installation Guide](#installation-guide)
- [Python Packages](#python-packages)
- [Project Members](#project-members)
- [License](#license)

## 🚀 Project Overview

Climatopia is a comprehensive platform that leverages advanced machine learning techniques, multi-agent reinforcement learning, and graph neural networks to simulate complex "what if" scenarios across climate, economy, and social systems. Our platform enables researchers, policymakers, businesses, and concerned citizens to explore the potential impacts of various interventions and policy decisions on our planet's future.

The project combines cutting-edge AI technologies with real-world datasets from NASA, NOAA, IMF, World Bank, and other authoritative sources to create accurate, data-driven simulations that can help inform critical decisions about our collective future.

## ✨ Key Features

### 🌦️ Real-time Weather Monitoring
- **Location-based Weather**: Users can enter their city/location to view real-time weather data
- **Comprehensive Metrics**: Temperature, humidity, wind speed, pressure, and more
- **Interactive Visualizations**: Dynamic charts and weather maps

### 🔮 Future Climate Prediction (AI/ML)
- **Custom ML Models**: Trained on historical weather and climate datasets
- **Predictive Analytics**: Forecast future conditions including:
  - Wind speed and direction
  - Rainfall patterns
  - Sea level changes
  - Temperature trends
- **Visual Analytics**: Dynamic graphs and interactive charts for data visualization

### 🤔 "What If" Scenario Engine
- **Natural Language Queries**: Users ask hypothetical climate questions
  - Example: *"What if it rains today at 4 PM in Mumbai?"*
- **AI-Powered Responses**: Context-aware AI processes queries using:
  - Historical data analysis
  - ML model predictions
  - Real-time weather conditions
- **Multi-format Answers**: Responses delivered via text, charts, or interactive visualizations

### 👥 Social Community Features
- **Public Feed**: Users can publish their "What If" questions and AI responses
- **Engagement System**: Like and comment on community posts
- **Knowledge Sharing**: Learn from others' climate curiosity and insights

### 🏆 Achievement Badge System
- **Like-based Rewards**: Earn badges based on total likes across posts
  - 🥉 **Bronze Badge**: 10+ likes
  - 🥈 **Silver Badge**: 50+ likes
  - 🥇 **Gold Badge**: 100+ likes
  - 💎 **Diamond Badge**: 500+ likes
- **Web3 Integration**: Optional NFT conversion for badges (blockchain-based)

## 🔍 Problem Statement

Our world faces unprecedented challenges:

- **Climate Crisis**: Rising temperatures, extreme weather events, and ecological disruption threaten global stability.
- **Economic Uncertainty**: Traditional economic models struggle to account for climate impacts and resource constraints.
- **Policy Complexity**: Decision-makers lack tools to understand the complex, interconnected consequences of their choices.
- **Data Silos**: Critical information exists in disconnected systems, making holistic analysis difficult.
- **Public Understanding**: Complex scientific models are often inaccessible to the general public.

## 💡 Our Solution

Climatopia addresses these challenges through:

1. **Integrated Modeling**: Combining climate science, economics, and social dynamics in a unified simulation framework.
2. **AI-Powered Predictions**: Using advanced machine learning to model complex system interactions and emergent behaviors.
3. **Accessible Interface**: Providing intuitive visualizations and plain-language explanations of complex scenarios.
4. **Community Engagement**: Enabling users to share, discuss, and collaborate on simulation scenarios.
5. **Real-World Data**: Incorporating authoritative datasets to ground simulations in empirical reality.

## 💳 Credit System & Subscriptions

### 🎁 Free Credits
- **New User Bonus**: 50 free credits for every new user
- **Question Cost**: Each "What If" question costs 10 credits

### 💰 Subscription Plans

| Plan | Credits | Price (INR) | Best For |
|------|---------|-------------|----------|
| **Starter** | 100 credits | ₹99 | Casual users |
| **Explorer** | 150 credits | ₹139 | Regular users |
| **Researcher** | 500 credits | ₹449 | Power users & professionals |

### 🔄 Payment Options
- **Fiat Payments**: Stripe integration for INR transactions
- **Web3 Payments** *(Optional)*: Crypto token payments
- **Subscription Management**: Automatic renewal and credit top-ups

## 🏗️ Architecture

Climatopia is built as a scalable monorepo with the following components:

```
Climatopia/ 
├── website/                     # Frontend (Next.js App)
│   ├── public/
│   ├── src/
│   │   ├── app/
│   │   ├── components/
│   │   ├── data/
│   │   ├── models/
│   │   ├── types/
│   │   ├── util/
│   │   └── middleware.js
│   ├── .env
│   ├── package.json
│   └── README.md                ✅ README for frontend

├── web3/                        # Smart Contract & Badge Logic
│   ├── badges/                 # JSON badge metadata
│   ├── contract.sol            # Solidity smart contract
│   ├── index.js                # JavaScript interface
│   └── README.md               ✅ README for web3 logic

├── Python Backend/                 # Python ML Backend 
│   ├── Datasets/
│   ├── eco_xbg/
│   ├── electricity_prediction/
│   ├── fastapis/
│   ├── pretrained_models/      ✅ Optional: Move pretrained files here
│   ├── .env
│   ├── *.py
│   ├── *.json
│   └── README.md               ✅ README for backend

├── README.md                   ✅ Main project overview
└── LICENSE
└── CODE_OF_CONDUCT.md
└── CONTRIBUTING.md
└── SECURITY.md
```

### Core Modules:

1. **Simulation Engine (Python)**
   - Multi-Agent Reinforcement Learning with Ray RLlib/PettingZoo
   - Graph Neural Networks for modeling interdependencies using PyTorch Geometric/DGL
   - Physics-Informed Neural Networks for accurate physical modeling
   - FastAPI server for exposing simulation capabilities

2. **Backend API (Next.js/Node.js)**
   - Scenario configuration and management
   - User profiles, social features
   - Credit system and subscription management
   - Payment processing (Stripe integration)
   - Notification system

3. **Frontend Interface (Next.js)**
   - Interactive map-based visualizations
   - Scenario creation and management
   - Community features and social feed
   - Subscription management dashboard
   - Real-time weather monitoring

4. **GenAI Module**
   - LLM-powered explanations of simulation results
   - Chain-of-thought reasoning for transparent analysis
   - Natural language processing for "What If" queries

5. **Authentication & User Management**
   - Clerk integration for secure authentication
   - User profile management
   - Credit tracking and usage analytics

6. **Social Sharing System**
   - Community features for sharing simulation results
   - Discussion and collaboration tools
   - Like/comment system
   - Trending scenarios and leaderboards

7. **Web3 Rewards** *(Optional)*
   - Achievement badges as NFTs
   - Crypto payment integration
   - Contributor recognition system

## 🛠️ Tech Stack

### Frontend
- **Framework**: Next.js 14 with App Router
- **Styling**: Tailwind CSS
- **Charts**: Recharts / Chart.js
- **UI Components**: Custom component library
- **State Management**: React Context / Zustand

### Backend
- **Runtime**: Node.js
- **Database**: MongoDB with Mongoose
- **Authentication**: Clerk
- **File Storage**: Cloudinary
- **Payments**: Stripe API

### AI/ML Engine
- **Language**: Python
- **Framework**: FastAPI
- **ML Libraries**: PyTorch, scikit-learn, XGBoost
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Plotly

### Web3 (Optional)
- **Wallet Integration**: WalletConnect / MetaMask
- **Smart Contracts**: Solidity (ERC-721 for badges)
- **Protocol**: Unlock Protocol for subscriptions

### Deployment
- **Frontend/Backend**: Vercel
- **ML Engine**: Railway / Google Cloud Run
- **Database**: MongoDB Atlas
- **CDN**: Cloudinary

### Deployment

The project is set up for deployment on Vercel (frontend/backend) and Railway (Python APIs).

```bash
# Deploy frontend and backend
npm run deploy

# Deploy ML engine
cd "Python Backend"
railway up
```

## 📦 Python Packages

The ML engine relies on the following key Python packages:

- **FastAPI**: Web framework for API development
- **PyTorch**: Deep learning framework
- **PyTorch Geometric**: Graph neural network library
- **Ray RLlib**: Distributed reinforcement learning
- **PettingZoo**: Multi-agent reinforcement learning environments
- **SciANN**: Scientific computing with neural networks
- **NumPy/Pandas**: Data manipulation and analysis
- **Matplotlib/Plotly**: Data visualization
- **LangChain**: LLM integration framework
- **scikit-learn**: Machine learning utilities
- **xgboost/lightgbm**: Gradient boosting frameworks
- **NetworkX**: Graph analysis
- **Geopandas**: Geospatial data handling
- **Dask**: Parallel computing
- **Requests**: HTTP library for API calls
- **Python-dotenv**: Environment variable management

Full requirements can be found in `Python Backend/requirements.txt`

## 👥 Project Members

| Name | Role | Contact |
|------|------|---------|
| [Manil Modi] | ML Developer | [GitHub](https://github.com/ManilModi) |
| [Milan bhadarka] | Full Stack Web Developer | [GitHub](https://github.com/milanbhadarka) |
| [Devan Chanuhan] | Full Stack Web Developer | [GitHub](https://github.com/Devan019) |
| [Suryadeepsinh Gohil] | Web3 Developer | [GitHub](https://github.com/Suryadeep36) |

**Team**: T3Coders  
**Project**: Climatopia - Hackathon Entry

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-repo/climatopia.git
   cd climatopia
   ```

2. **Install dependencies**
   ```bash
   # Frontend
   cd website
   npm install
   
   # Python Backend
   cd "../Python Backend"
   pip install -r requirements.txt
   ```

3. **Set up environment variables**
   ```bash
   # Copy example env files
   cp website/.env.example website/.env
   cp "Python Backend"/.env.example "Python Backend"/.env
   ```

4. **Start development servers**
   ```bash
   # Frontend (port 3000)
   cd website
   npm run dev
   
   # Python Backend (port 8000)
   cd "../Python Backend"
   python main.py
   ```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<p align="center">
  Built with ❤️ by <strong>Team T3Coders</strong><br>
  © 2025 Climatopia. All rights reserved.
</p>
# 🌍 Climatopia

> An AI-powered, planet-scale simulation engine for "what if" scenarios across climate, economy, and humanity.

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Our Solution](#our-solution)
- [Architecture](#architecture)
- [API Documentation](#api-documentation)
- [Installation Guide](#installation-guide)
- [Python Packages](#python-packages)
- [Project Members](#project-members)
- [License](#license)

## 🚀 Project Overview

Climatopia is a comprehensive platform that leverages advanced machine learning techniques, multi-agent reinforcement learning, and graph neural networks to simulate complex "what if" scenarios across climate, economy, and social systems. Our platform enables researchers, policymakers, businesses, and concerned citizens to explore the potential impacts of various interventions and policy decisions on our planet's future.

The project combines cutting-edge AI technologies with real-world datasets from NASA, NOAA, IMF, World Bank, and other authoritative sources to create accurate, data-driven simulations that can help inform critical decisions about our collective future.

## 🔍 Problem Statement

Our world faces unprecedented challenges:

- **Climate Crisis**: Rising temperatures, extreme weather events, and ecological disruption threaten global stability.
- **Economic Uncertainty**: Traditional economic models struggle to account for climate impacts and resource constraints.
- **Policy Complexity**: Decision-makers lack tools to understand the complex, interconnected consequences of their choices.
- **Data Silos**: Critical information exists in disconnected systems, making holistic analysis difficult.
- **Public Understanding**: Complex scientific models are often inaccessible to the general public.

## 💡 Our Solution

Climatopia addresses these challenges through:

1. **Integrated Modeling**: Combining climate science, economics, and social dynamics in a unified simulation framework.
2. **AI-Powered Predictions**: Using advanced machine learning to model complex system interactions and emergent behaviors.
3. **Accessible Interface**: Providing intuitive visualizations and plain-language explanations of complex scenarios.
4. **Community Engagement**: Enabling users to share, discuss, and collaborate on simulation scenarios.
5. **Real-World Data**: Incorporating authoritative datasets to ground simulations in empirical reality.

## 🏗️ Architecture

Climatopia is built as a scalable monorepo with the following components:

```
Climatopia/ 
├── website/                     # Frontend (Next.js App)
│   ├── public/
│   ├── src/
│   │   ├── app/
│   │   ├── components/
│   │   ├── data/
│   │   ├── models/
│   │   ├── types/
│   │   ├── util/
│   │   └── middleware.js
│   ├── .env
│   ├── package.json
│   └── README.md                ✅ README for frontend

├── web3/                        # Smart Contract & Badge Logic
│   ├── badges/                 # JSON badge metadata
│   ├── contract.sol            # Solidity smart contract
│   ├── index.js                # JavaScript interface
│   └── README.md               ✅ README for web3 logic

├── Python Backend/                 # Python ML Backend 
│   ├── Datasets/
│   ├── eco_xbg/
│   ├── electricity_prediction/
│   ├── fastapis/
│   ├── pretrained_models/      ✅ Optional: Move pretrained files here
│   ├── .env
│   ├── *.py
│   ├── *.json
│   └── README.md               ✅ README for backend

├── README.md                   ✅ Main project overview
└── LICENSE
└── CODE_OF_CONDUCT.md
└── CONTRIBUTING.md
└── SECURITY.md
```

### Core Modules:

1. **Simulation Engine (Python)**
   - Multi-Agent Reinforcement Learning with Ray RLlib/PettingZoo
   - Graph Neural Networks for modeling interdependencies using PyTorch Geometric/DGL
   - Physics-Informed Neural Networks for accurate physical modeling
   - FastAPI server for exposing simulation capabilities

2. **Backend API (Next.js/Express)**
   - Scenario configuration and management
   - User profiles, social features
   - Credit system and Web3 integration
   - Notification system

3. **Frontend Interface (Next.js)**
   - Interactive map-based visualizations
   - Scenario creation and management
   - Community features
   - Subscription management

4. **GenAI Module**
   - LLM-powered explanations of simulation results
   - Chain-of-thought reasoning for transparent analysis
   - Natural language processing for scenario creation

5. **Subscription & Credit System**
   - Tiered access model (Free/Pro/NGO)
   - Usage tracking and analytics
   - Payment processing

6. **Social Sharing System**
   - Community features for sharing simulation results
   - Discussion and collaboration tools
   - Leaderboards and trending scenarios

7. **Web3 Rewards**
   - Achievement badges as NFTs
   - Contributor recognition
   - Verification system for organizations


### **Access the application**

Open your browser and navigate to `http://localhost:3000`

### Deployment

The project is set up for deployment on Vercel (frontend/backend) and Railway (Python APIs).

\`\`\`bash
# Deploy frontend and backend
npm run deploy

# Deploy ML engine
cd packages/ml-core
railway up
\`\`\`

## 📦 Python Packages

The ML engine relies on the following key Python packages:

- **FastAPI**: Web framework for API development
- **PyTorch**: Deep learning framework
- **PyTorch Geometric**: Graph neural network library
- **Ray RLlib**: Distributed reinforcement learning
- **PettingZoo**: Multi-agent reinforcement learning environments
- **SciANN**: Scientific computing with neural networks
- **NumPy/Pandas**: Data manipulation and analysis
- **Matplotlib/Plotly**: Data visualization
- **LangChain**: LLM integration framework
- **scikit-learn**: Machine learning utilities
- **xgboost/lightgbm**: Gradient boosting frameworks
- **NetworkX**: Graph analysis
- **Geopandas**: Geospatial data handling
- **Dask**: Parallel computing

Full requirements can be found in `packages/ml-core/requirements.txt`

## 👥 Project Members

| Name | Role | Contact |
|------|------|---------|
| [Team Member 1] | Project Lead | [email/github] |
| [Team Member 2] | ML Engineer | [email/github] |
| [Team Member 3] | Frontend Developer | [email/github] |
| [Team Member 4] | Backend Developer | [email/github] |
| [Team Member 5] | Data Scientist | [email/github] |
| [Team Member 6] | DevOps Engineer | [email/github] |

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<p align="center">© 2025 Climatopia Team. All rights reserved.</p>
\`\`\`

<CodeProject id="earthsim_project">
