# Web Scraping Project - Twitter Trends

## 📌 Project Overview
This project automates the process of scraping Twitter trends using **Python, Flask, Selenium**, and **MongoDB**, and updates the results dynamically on a web page.

---

## 🏆 Objective
1. **Scrape Latest Twitter Trends:**  
   - Automate the retrieval of trending topics from Twitter.
   - Store the data in a MongoDB database.
   
2. **Analyze and Display the Data:**  
   - Fetch the latest data from MongoDB.
   - Dynamically display the trends on a Flask web page.

3. **Provide Interactive Web Interface:**  
   - Run the scraping script.
   - Refresh data using buttons on the web page.

---

## ⚙️ Technologies Used
- **Python** (Backend Logic)
- **Flask** (Web Application Framework)
- **Selenium** (Web Automation)
- **MongoDB** (Database)
- **JavaScript (AJAX, jQuery)** (Frontend Updates)
- **HTML/CSS** (Web Page Layout)
- **Chrome WebDriver** (Browser Automation)

---

## 📂 Project Structure

```
FirstName_LastName_SDET/
│-- resume.pdf                        # Your resume
│-- exactspace.har                     # Generated HAR file
│-- status_code_counts.json             # JSON output with status code counts
│-- sdet_script.py                      # Python source code for automation
│-- templates/
│   └── index.html                      # Webpage for displaying trends
│-- static/
│   └── styles.css                       # CSS styles for UI
│-- app.py                              # Flask application for the project
│-- README.md                           # Project documentation
```

---

## 🚀 Setup Instructions

### 1. Prerequisites
Ensure you have the following installed:

- **Python 3.x** → [Download here](https://www.python.org/downloads/)
- **Google Chrome** → [Download here](https://www.google.com/chrome/)
- **ChromeDriver** (matching Chrome version) → [Download here](https://sites.google.com/chromium.org/driver/)
- **MongoDB Atlas** (Cloud Database) → [Set up here](https://www.mongodb.com/cloud/atlas)

### 2. Install Required Python Libraries

```bash
pip install -r requirements.txt
```

If you don't have a `requirements.txt`, install manually:

```bash
pip install flask selenium pymongo certifi flask-socketio
```

---

## 🔧 How to Run the Project

1. **Clone the Repository (If applicable):**
   ```bash
   git clone https://github.com/yourusername/web-scraping-project.git
   cd web-scraping-project
   ```

2. **Set Up ChromeDriver and Proxy Paths:**  
   Edit the `app.py` file and update paths accordingly:

   ```python
   server = Server("/path/to/browsermob-proxy/bin/browsermob-proxy")
   chrome_service = Service("/path/to/chromedriver")
   ```

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

## 🖥️ How the Project Works

1. **Initial Page Load (`/` route):**  
   - Fetches the latest trends from MongoDB and displays them.
   - Starts the scraping process.

2. **Scraping Process:**  
   - Uses Selenium to scrape Twitter trends.
   - Saves the data into MongoDB.

3. **Refreshing the Data:**  
   - Users can click the "Refresh" button to get the latest data.

4. **Running the Scraper Manually:**  
   - Clicking the "Run Scraper" button triggers the Python script.

---

## 📊 Expected Output

The web page displays:

```
Latest Twitter Trends:
- Trend: #Python
- Date: 2025-01-22
- Time: 14:45:10
```

A JSON file (`status_code_counts.json`) will also contain:

```json
{
    "Total Status Codes": 150,
    "2XX Count": 120,
    "4XX Count": 20,
    "5XX Count": 10
}
```

---

## 📝 Deliverables

Submit a zip folder named as:

```
FirstName_LastName_SDET.zip
```

Contents of the folder:

1. **Your resume** - `resume.pdf`
2. **Python script** - `app.py`
3. **Generated HAR file** - `exactspace.har`
4. **Output file** - `status_code_counts.json`

---

## 🛠️ Troubleshooting

### 1. Flask App Not Starting  
   **Error:** `ModuleNotFoundError: No module named 'flask'`  
   **Solution:**  
   - Install Flask using `pip install flask`.

### 2. ChromeDriver Version Mismatch  
   **Error:** `chromedriver executable needs to be in PATH`  
   **Solution:**  
   - Download the correct ChromeDriver version matching your Chrome browser.

### 3. MongoDB Connection Issues  
   **Error:** `ServerSelectionTimeoutError`  
   **Solution:**  
   - Ensure the correct MongoDB Atlas connection string in `app.py`.

---

## 📧 Contact

For any queries, reach out to:

- **Email:** your.email@example.com
- **GitHub:** [yourgithub](https://github.com/yourgithub)

---

### ✅ Happy Coding! 🎯
```

