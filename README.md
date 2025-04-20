
#  Exercise Tracker with Nutritionix & Google Sheets Integration

This Python project allows users to input their daily exercise activities in natural language (e.g., "walked 2 miles and ran 4km"). It then uses the Nutritionix API to extract meaningful data such as duration and calories burned, and automatically logs the information into a Google Sheet.

##  Technologies Used

- Python 
- Nutritionix API 
- Google Sheets API via Sheety 
- Environment Variables for secure authentication 

##  Setup & Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Junayed-Bin-Karim/fitness-tracker.git
    ```

2. **Create a `.env` file** with your credentials:
    ```env
    APP_ID=your_nutritionix_app_id
    APP_KEY=your_nutritionix_app_key
    SHEET_URL=your_sheety_endpoint_url
    TOKEN=your_sheety_token
    ```

3. **Install required packages**:
    ```bash
    pip install requests python-dotenv
    ```

4. **Run the script**:
    ```bash
    python your_script.py
    ```

## How It Works

- You enter your workout in plain English.
- Nutritionix API processes the input and returns detailed data (e.g., calories burned, duration).
- The data is sent to your Google Sheet via Sheety API, along with the current date and time.

##  Sample Input

```plaintext
Tell me which exercises you did: 
walked 2 miles and ran 4km
```
## Sample Output Logged to Sheet

Date	Time	Exercise	Duration (min)	Calories
20/04/2025	10:00:00	walked 2 miles	30	150


This python project helps the user in keeping track of his workouts.
After the workout, the user can input his workout in natural language sentence form like "walked 2 miles and ran 4km". 
This data is processed in OpenAI API. The response sent by API i.e duration and calories to program is then sent and stored in goggle sheet using Sheety Api in tabular form.
The table contains: Date, Time, Excercise Type, Duration, Calories Burned fields. Sample sheet is given below:

![alt text](https://github.com/shubham101096/fitness-tracker/blob/master/fitness-tracker-screenshot.png?raw=true)

Author
Md. Junayed Bin Karim

