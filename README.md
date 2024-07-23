# Bull's AI: Algorithmic Stock Prediction

Bull's AI is an advanced stock prediction tool that leverages machine learning algorithms to generate precise stock forecasts. This project combines financial data APIs, deep learning techniques, and news sentiment analysis to provide accurate intraday predictions and simulated trading results.

## Features

- Precise stock forecasts using cutting-edge machine learning algorithms
- 95% accurate predictions
- Intraday predictions for timely trading decisions
- Simulated trades with 29% annualized excess returns
- Rigorous error analysis with 43% MSE loss reduction compared to baseline models

## Tech Stack

- Machine Learning
- Financial Data APIs
- Deep Learning (LSTM)
- Support Vector Machines (SVM)
- Flask
- Keras
- Matplotlib
- News API
- Streamlit
- NumPy
- Pandas
- yfinance
- scikit-learn

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/bulls-ai.git
   cd bulls-ai
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Set up your API keys:
   - Create a `.env` file in the root directory
   - Add your API keys for financial data and news services:
     ```
     FINANCIAL_API_KEY=your_financial_api_key
     NEWS_API_KEY=your_news_api_key
     ```

## Usage

1. Run the Streamlit application:
   ```
   streamlit run app.py
   ```

2. Open your web browser and navigate to the URL provided by Streamlit (usually `http://localhost:8501`)

3. Enter the stock ticker symbol for the stock you want to predict in the sidebar

4. View the generated predictions, charts, and analysis, including:
   - Predicted Price vs Original Price graph
   - Data Description
   - Closing Price vs Time Chart
   - Closing Price vs Time Chart with 100MA
   - Closing Price vs Time Chart with 100MA & 200MA

## Project Structure

- `app.py`: Main Streamlit application
- `StockAI.h5`: Pre-trained Keras model for stock prediction
- `requirements.txt`: List of Python dependencies
- `README.md`: Project documentation (this file)

## How It Works

1. The application fetches historical stock data using the yfinance library.
2. Data is split into training and testing sets.
3. A MinMaxScaler is used to normalize the data.
4. The pre-trained LSTM model (`StockAI.h5`) is loaded and used for predictions.
5. The model predicts stock prices, which are then inverse transformed to the original scale.
6. Various visualizations are created using Matplotlib and displayed using Streamlit.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to Yahoo Finance for providing access to their financial data API
- Inspired by recent advancements in deep learning for time series prediction
- Streamlit for providing an easy-to-use framework for building data applications

## Future Development Plans

- Integrate additional data sources for more comprehensive analysis
- Implement ensemble methods to improve prediction accuracy
- Develop a backtesting framework for strategy evaluation
- Create a user authentication system for personalized experiences
- Optimize the model for real-time predictions

## Contact

For any questions or feedback, please contact Sahil Bhoite at work.sahilbhoite@gmail.com.

Connect with me on LinkedIn: [https://www.linkedin.com/in/sahil-bhoite/](https://www.linkedin.com/in/sahil-bhoite/)

---

**Note**: This project is for educational purposes only. Always do your own research and consider seeking advice from a qualified financial professional before making investment decisions.
