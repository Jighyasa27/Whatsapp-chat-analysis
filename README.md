# WhatsApp Chat Analyzer

A Streamlit web application to analyze WhatsApp chat exports. This tool provides insights into chat statistics, user activity, word usage, emoji analysis, and more, with visualizations and interactive controls.

## Features
- Upload and analyze WhatsApp chat export files
- View top statistics: total messages, words, media, and links
- Monthly and daily message timelines
- Activity maps by day and month
- Weekly activity heatmap
- Most active users in group chats
- Word cloud and most common words (with Hinglish stopword removal)
- Emoji usage analysis

### Prerequisites
- Python 3.7+

### Installation
1. **Clone the repository:**
   ```bash
   git clone <repo-url>
   cd whatsapp-chat-miniproject-5th
   ```
2. **Install dependencies:**
   ```bash
   pip install streamlit pandas matplotlib seaborn wordcloud urlextract emoji
   ```

### Files
- `app.py`: Main Streamlit app
- `helper.py`: Helper functions for statistics, word cloud, emoji analysis, etc.
- `preprocessor.py`: Preprocesses WhatsApp chat text into structured data
- `stop_hinglish.txt`: Hinglish stopwords for filtering common words

### Usage
1. **Run the app:**
   ```bash
   streamlit run app.py
   ```
2. **Open the app in your browser** (usually at http://localhost:8501)
3. **Upload your WhatsApp chat export file** (text format)
4. **Explore the analysis and visualizations**

## How it Works
- The app preprocesses the chat file, extracts users, messages, dates, and more
- Provides statistics and visualizations for overall and per-user activity
- Uses a custom Hinglish stopword list for word cloud and common word analysis

## Dependencies
- streamlit
- pandas
- matplotlib
- seaborn
- wordcloud
- urlextract
- emoji

Install all dependencies with the provided pip command above.

## License
MIT License

## Acknowledgements
- Inspired by various open-source WhatsApp analyzers
- Stopword list includes common Hinglish and English words
