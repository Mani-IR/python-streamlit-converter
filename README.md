


# Currency Converter

A simple web-based currency converter built with Python and Streamlit. Converts amounts between currencies using real-time exchange rates from [ExchangeRate-API](https://www.exchangerate-api.com/).

## Features
- Real-time currency conversion
- Interactive Streamlit UI
- Caches exchange rates for 3 hours
- Supports multiple currencies

## Project Structure
```
pro-6/
├── env/                        # Virtual environment
├── src/
│   ├── app.py                 # Streamlit app
│   ├── currency_convertor.py  # Conversion logic
│   └── constants.py           # Currency list
└── README.md
```

## Setup
1. Clone the repo:
   ```bash
   git clone <repository-url>
   cd pro-6
   ```
2. Create and activate virtual environment:
   ```bash
   python -m venv env
   source env/bin/activate  # Linux/Mac
   env\Scripts\activate     # Windows
   ```
3. Install dependencies:
   ```bash
   pip install streamlit requests cachetools
   ```
4. Run the app:
   ```bash
   cd src
   streamlit run app.py
   ```

## Usage
- Select base and target currencies
- Enter amount to convert
- View instant results

## Notes
- Rates cached for 3 hours
- Requires `constants.py` with `CURRENCIES` list
- Shows error if API fails

## Dependencies
- `streamlit`
- `requests`
- `cachetools`

## License
MIT License
