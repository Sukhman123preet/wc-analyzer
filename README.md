# WhatsApp Chat Analyzer

## Overview
The **WhatsApp Chat Analyzer** is a Streamlit-based application that allows users to upload a WhatsApp chat file and perform various types of analysis, such as message statistics, word cloud generation, emoji frequency analysis, and activity mapping. The app provides insights into user messaging behavior, the most active users, and detailed activity heatmaps.

## Features
- **User Selection**: Choose between analyzing data for all users or a specific user in the chat.
- **Message Statistics**: Displays total messages, words, media, and links shared by the selected user.
- **Active User Analysis**: Visualizes the most active users and their contribution in a pie chart.
- **Word Cloud**: Generates a word cloud based on the most frequently used words, excluding stopwords.
- **Emoji Analysis**: Displays the top 5 most used emojis in the chat.
- **Quarterly Timeline**: Shows the message count over time, broken down by quarters.
- **Activity Map**: Provides insights into the busiest days and months.
- **Heatmap**: Displays an hourly activity heatmap for each day of the week.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-repository/whatsapp-chat-analyzer.git
    cd whatsapp-chat-analyzer
    ```

2. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Streamlit application**:
    ```bash
    streamlit run app.py
    ```

## File Structure

- `app.py`: The main file to run the Streamlit application.
- `helper.py`: Contains helper functions for data processing and analysis.
- `index.py`: Contains the function to parse the uploaded WhatsApp chat file.
- `requirements.txt`: Lists the dependencies required to run the application.

## How It Works

1. **Upload a File**: 
   - Upload a WhatsApp chat file (.txt) via the sidebar.
  
2. **User Selection**:
   - After processing, users can select "overall" (for all users) or a specific user from the sidebar for analysis.

3. **Analysis**:
   - On clicking "Show Analysis", detailed statistics, including message count, word count, media, and links shared, are displayed in the main area.

4. **Most Active Users**:
   - For the "overall" user selection, a pie chart is displayed showing the percentage distribution of messages from the most active users.

5. **Word Cloud**:
   - A word cloud of frequently used words (excluding stopwords) is displayed.

6. **Emoji Frequency Analysis**:
   - The top 5 most frequently used emojis are shown in a bar chart along with their respective frequencies.

7. **Timeline**:
   - A timeline plot showing the number of messages sent per quarter.

8. **Activity Map**:
   - Displays the busiest days and months for message activity.
   
9. **Heatmap**:
   - An hourly activity heatmap showing the messaging patterns for each day of the week.

## Dependencies
- **Python**: Version 3.x
- **Streamlit**: For building the web interface.
- **Pandas**: For data manipulation.
- **Matplotlib**: For plotting graphs and charts.
- **Seaborn**: For advanced data visualizations.
- **WordCloud**: For generating word clouds.
- **NLTK**: For natural language processing, particularly for stopword removal.
- **NumPy**: For array manipulation.
  
## Credits
This project uses open-source libraries, including Streamlit, NLTK, Matplotlib, Seaborn, and others.

## License
This project is licensed under the MIT License.
