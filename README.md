# SmartDealHunter_DealPricer_AI

A sophisticated multi-agent system that leverages AI for real-time deal detection and accurate price prediction. The system combines multiple specialized AI agents and advanced pricing models to identify deals, predict true market values, and notify users instantly.

## Key Features

- **Advanced Price Prediction**
  - Ensemble model combining multiple prediction approaches
  - RAG (Retrieval Augmented Generation) for market value analysis
  - Category-specific pricing models
  - Random Forest model for feature-based predictions

- **Autonomous Agent System**
  - Scanner Agent for deal identification
  - Frontier Agent for RAG-based pricing
  - Ensemble Agent for model combination
  - Specialist Agent for domain analysis
  - Messaging Agent for notifications

- **Real-time Monitoring**
  - Live deal tracking dashboard
  - Push notifications for promising deals
  - Deal analysis with price comparisons
  - Automated alerts system

## Setup Instructions

1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/SmartDealHunter_DealPricer_AI.git
cd SmartDealHunter_DealPricer_AI
```

2. **Install dependencies:**
```bash
pip install -r requirements.txt
```

3. **Configure environment variables:**

Create a `.env` file in the root directory with the following variables:
```
# Required API Keys
PUSHOVER_USER=your_pushover_user_key    # For notifications
PUSHOVER_TOKEN=your_pushover_token      # For notifications
HF_TOKEN=your_huggingface_token        # For model access
```

4. **Run the application:**
```bash
python pricer_is_right_gradio.py
```

## Project Structure
```
SmartDealHunter_DealPricer_AI/
├── agents/                      # Agent implementations
│   ├── scanner_agent.py        # Deal detection
│   ├── frontier_agent.py       # RAG-based pricing
│   ├── ensemble_agent.py       # Model combination
│   ├── specialist_agent.py     # Domain expertise
│   └── messaging_agent.py      # Notifications
├── notebooks/                   # Development notebooks
├── scripts/                     # Utility scripts
└── pricer_is_right_gradio.py   # Main UI application
```

## Environment Setup

The application requires several API keys stored in a `.env` file:

1. **Pushover Keys** (for notifications):
   - Create account at pushover.net
   - Get your user key and app token
   - Add to .env as PUSHOVER_USER and PUSHOVER_TOKEN

2. **HuggingFace Token** (for models):
   - Get token from huggingface.co
   - Add to .env as HF_TOKEN

## Model Performance

- Multi-model ensemble for robust predictions
- Category-specific optimization
- Historical data validation
- Continuous learning from market data

## How It Works

1. Scanner Agent monitors for potential deals
2. Frontier Agent estimates true market value
3. Ensemble Agent combines multiple model predictions
4. System calculates potential savings
5. Messaging Agent sends notifications for good deals

## Future Development

- Enhanced market trend analysis
- Additional pricing models
- Extended product categories
- Improved deal relevance scoring

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Note on Large Files

This repository does not include model files (*.pkl) and the vector store due to size limitations. These will be generated when running the application.

