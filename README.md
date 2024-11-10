# WhatsApp Chat Analysis Project

## Project Overview
This project analyzes WhatsApp chat data to extract insights, statistics, and trends. It processes raw WhatsApp exported chat data, structures it, and generates a variety of visualizations and metrics to help understand user activity, message frequency, common words, and more. The project aims to offer an interactive and insightful analysis of a WhatsApp group or individual chat.

## Features
- **Message Analysis**: Shows key statistics like total messages, words, media shared, and links sent.
- **Timeline Visualization**: Analyzes the chat's activity over time, including monthly and daily message trends.
- **Activity Heatmap**: Displays the activity levels of users during different times of the day and week.
- **WordCloud**: Generates a word cloud based on the most frequent words used in the chat.
- **Emoji Analysis**: Provides insights into the emojis most commonly used in the chat.
- **Most Active Users**: Identifies the users who send the most messages in a group or with an individual.
- **Interactive Dashboard**: The user can select individual users or view overall group activity. The project uses Streamlit for a simple and interactive interface.

## Project Components

### 1. Preprocessing the Data
The raw WhatsApp chat data is preprocessed using Python to extract meaningful components such as date, user, message, and media. The data is then structured into a Pandas DataFrame, which allows for easy manipulation and analysis. Various date and time-related columns like day, month, year, and time of day are derived to facilitate activity analysis.

### 2. Helper Functions
- **fetch_stats**: Calculates basic statistics like total messages, total words, media messages, and links shared.
- **most_busy_users**: Identifies the busiest users based on message count.
- **create_wordcloud**: Generates a word cloud of the most frequent words.
- **most_common_words**: Displays the most common words used in the chat (excluding stop words).
- **emoji_helper**: Analyzes and counts the emojis used in the chat.
- **monthly_timeline**: Creates a monthly timeline of the chat activity.
- **daily_timeline**: Analyzes and visualizes the daily message frequency.
- **week_activity_map**: Provides a bar chart of activity levels by day of the week.
- **month_activity_map**: Displays a bar chart of activity by month.
- **activity_heatmap**: Creates a heatmap showing activity levels across different times of the day.

### 3. Streamlit Interface
A simple and user-friendly dashboard is created using Streamlit, allowing users to:
- Upload their WhatsApp chat file.
- Select specific users or view overall group activity.
- View key statistics and visualizations that are dynamically updated based on user selection.

## Detailed Description of the Main Functionality

### 1. Data Preprocessing
The `preprocess` function is responsible for cleaning and structuring the raw chat data into a usable format:
- **Message Extraction**: It extracts the user, message, and timestamp from each chat entry.
- **Date and Time**: The function creates multiple columns to break down the date and time information into components such as year, month, day, hour, and minute.
- **Handling Group Notifications**: Group notifications, such as when someone joins or leaves, are tagged separately.

### 2. Statistics Calculation
The `fetch_stats` function calculates basic statistics like:
- **Total number of messages**: Counts the total number of messages sent.
- **Total number of words**: Counts the total number of words in the chat.
- **Number of media messages**: Counts the number of media messages (e.g., photos, videos) sent.
- **Number of links shared**: Counts the total number of links shared in the chat.

### 3. Message and Activity Visualization
The app generates several interactive visualizations:
- **Monthly and Daily Timeline**: Line charts show trends in the number of messages over time.
- **Activity Heatmap**: A heatmap shows the activity levels by day and time period, indicating when users are most active.
- **User Activity Maps**: Bar charts display the most active days and months, as well as the busiest users in the chat.

### 4. Text Analysis
- **Word Cloud**: The most frequent words used in the chat are visualized using a word cloud, allowing users to easily identify key topics.
- **Most Common Words**: A bar chart shows the most commonly used words, excluding stop words, to give a clearer view of popular terms.
- **Emoji Analysis**: A pie chart visualizes the most commonly used emojis in the chat, giving insights into the emoji usage patterns.

### 5. Interactive Streamlit Dashboard
The Streamlit app provides a sidebar where users can select different analysis options:
- View group-level statistics or filter by individual users to view their specific activity.

## Visualizations
- **Message Trends**: Line charts showing the frequency of messages over time.
- **Activity Heatmaps**: Heatmaps to analyze the time of day and day of the week when users are most active.
- **WordCloud**: Visual representation of the most frequent words in the chat.
- **Emoji Usage**: A pie chart visualizing the most popular emojis used by the group.

## Technologies Used
- **Python**: The core programming language.
- **Streamlit**: Used to build the interactive web application.
- **Pandas**: Used for data manipulation and analysis.
- **Matplotlib & Seaborn**: Used for generating charts and graphs.
- **WordCloud**: Used to generate a word cloud visualization of chat data.
- **URLExtract**: Used to extract URLs shared in the chat.
- **Emoji**: Used to analyze emoji usage.

## Conclusion
This WhatsApp Chat Analysis project helps visualize and analyze chat data, offering insights into user behavior, message patterns, common words, and emoji usage. It can be used to analyze individual conversations or group chats, making it useful for personal data analysis or group communication insights.

## Video Demonstration
[Video Demonstration.webm](https://github.com/user-attachments/assets/034c7687-2d2e-49f7-b3f6-efdeaf8024f8)
