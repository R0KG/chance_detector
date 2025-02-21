# Chance Detector - Crypto Tweet Monitor

A Python-based tool that monitors selected celebrities and podcast stars on X (formerly Twitter) for crypto and meme coin-related tweets. This tool helps track potential market-moving announcements and trends in the cryptocurrency space.

## Features

- Real-time monitoring of specified X (Twitter) accounts
- Keyword-based filtering for crypto and meme coin mentions
- Sentiment analysis of tweets
- Data storage and visualization capabilities
- Scheduled monitoring and alerts

## Prerequisites

- Python 3.8+
- Twitter API credentials (Developer Account required)
- Required Python packages (see `requirements.txt`)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/chance_detector.git
cd chance_detector
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Set up your environment variables:
```bash
# Create a .env file and add your Twitter API credentials
TWITTER_API_KEY=your_api_key
TWITTER_API_SECRET=your_api_secret
TWITTER_ACCESS_TOKEN=your_access_token
TWITTER_ACCESS_TOKEN_SECRET=your_access_token_secret
```

## Project Structure

```
chance_detector/
├── src/
│   ├── __init__.py
│   ├── twitter_monitor.py
│   ├── sentiment_analyzer.py
│   └── data_storage.py
├── config/
│   ├── accounts.json
│   └── keywords.json
├── data/
│   └── tweets.db
├── tests/
│   └── __init__.py
├── requirements.txt
├── .env
└── README.md
```

## Configuration

1. Edit `config/accounts.json` to specify the Twitter accounts you want to monitor
2. Modify `config/keywords.json` to customize the keywords for filtering tweets
3. Adjust scheduling parameters in the main script if needed

## Usage

Run the main monitoring script:
```bash
python src/twitter_monitor.py
```

## Features in Detail

### Tweet Collection
- Fetches tweets from specified accounts using Twitter API v2
- Configurable tweet fetch frequency
- Historical tweet collection capability

### Filtering System
- Keyword-based filtering
- Regular expression support for advanced pattern matching
- Customizable filtering rules

### Sentiment Analysis
- Uses VADER sentiment analysis
- Provides sentiment scores (positive, negative, neutral)
- Customizable sentiment thresholds

### Data Storage
- SQLite database for tweet storage
- Export capability to CSV/JSON
- Historical data maintenance

### Visualization (Coming Soon)
- Web dashboard for trend visualization
- Real-time updates
- Historical data analysis

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Twitter API Documentation
- VADER Sentiment Analysis
- All contributors and maintainers

## Disclaimer

This tool is for educational and research purposes only. Always comply with Twitter's Terms of Service and API usage guidelines. Trading cryptocurrencies carries significant risks - use this information at your own discretion.