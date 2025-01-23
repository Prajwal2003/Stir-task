# Web Scraping Project - Twitter Trends

## Project Overview
This project automates the process of scraping Twitter trends using **Python, Flask, Selenium**, and **MongoDB**, and updates the results dynamically on a web page.

---

## Objective
1. **Scrape Latest Twitter Trends:**  
   - Automate the retrieval of trending topics from Twitter.
   - Store the data in a MongoDB database.
   
2. **Analyze and Display the Data:**  
   - Fetch the latest data from MongoDB.
   - Dynamically display the trends on a Flask web page.

---

## Technologies Used
- **Python** (Backend Logic)
- **Flask** (Web Application Framework)
- **Selenium** (Web Automation)
- **MongoDB** (Database)
- **JavaScript** (Frontend Updates)
- **HTML/CSS** (Web Page Layout)
- **Chrome WebDriver** (Browser Automation)

---

## Setup Instructions

### 1. Prerequisites
Ensure you have the following installed:

- **Python 3.x** → [Download here](https://www.python.org/downloads/)
- **Google Chrome** → [Download here](https://www.google.com/chrome/)
- **MongoDB Atlas** (Cloud Database) → [Set up here](https://www.mongodb.com/cloud/atlas)

### 2. Install Required Python Libraries

```bash
pip install flask selenium pymongo certifi flask-socketio
```

---

## How to Run the Project

1. **Clone the Repository (If applicable):**
   ```bash
   git clone https://github.com/yourusername/web-scraping-project.git
   cd web-scraping-project
   ```

2. **Enter you Credentials**  
   Edit the `creds.yaml` and `filezip.py`(this will generate the proxy setting zip) file and update paths accordingly:
   

3. **Run the Flask Application:**  
   Use the following command to start the Flask web server:

   ```bash
   python app.py
   ```

4. **Access the Web Interface:**  
   Open a browser and visit:

   ```
   http://localhost:5001
   ```

---

## How the Project Works

1. **Initial Page Load (`/` route):**  
   - Fetches the latest trends from MongoDB and displays them.
   - Shows 2 button - Run scraper and Refresh Data

2. **Clicking Run scraper - Scraping python code is run:**  
   - Uses Selenium to scrape Twitter trends.
   - Saves the data into MongoDB.

3. **Clicking on Refresh Data - Refreshes the Data:**  
   - Users can click the "Refresh" button to get the latest data.

---

## Expected Output

The web page displays:

```
        Latest Twitter Trends:

||  Run Scraper  ||  Refresh Data  ||

      Trend: #Trend1 #Trend2 ...
         Date: 2025-01-22
         IP: 142.45.10.5
```

---

## Contact

For any queries, reach out to:

```
- Email: prajwalgh13@gmail.com
- GitHub: https://github.com/Prajwal2003
```

