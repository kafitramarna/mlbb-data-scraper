## Description
This project is a Python script designed to scrape data from the Mobile Legends website and save it in a CSV file. The script collects information about heroes, including their win rate, pick rate, ban rate, and the best counters for each hero based on the data available on the Mobile Legends site. This data is then saved in the `data_hero_best_counter_for.csv` file.

## Languages or Tools
- Python
- Selenium

## Libraries
- pandas
- selenium
- csv

## How to Use
1. Ensure you have [Chromedriver](https://sites.google.com/chromium.org/driver/) compatible with your Chrome browser version, and place it in an appropriate location.
2. Install the required libraries by running:
    ```bash
    pip install pandas selenium
    ```
3. Download and save the `hero_data.csv` file containing your Mobile Legends hero data in the same directory as the script.
4. Adjust the path to Chromedriver in the script (variable `s`).
5. Run the script with:
    ```bash
    python script_name.py
    ```
   Replace `script_name.py` with the name of your Python file.

6. Once the script completes, the data will be saved in the `data_hero_best_counter_for.csv` file in the same directory.

## Example Output
The resulting CSV file will contain the following columns:
- `Hero`: Name of the hero
- `Pick Rate`: Hero's pick rate percentage
- `Win Rate`: Hero's win rate percentage
- `Ban Rate`: Hero's ban rate percentage
- `Best Counter For`: List of the best counter heroes
- `Role`: Hero's role
- `Best Lane`: Hero's best lane

## Notes
- This script uses Selenium for web scraping, so ensure you have a stable internet connection while running it.
- Adjust the sleep time (`time.sleep`) if needed to accommodate page loading speed.
