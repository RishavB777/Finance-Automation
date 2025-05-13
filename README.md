# Finance Dashboard

A Streamlit application for visualizing and categorizing personal finance transactions.  Upload a CSV, categorize transactions, and visualize your expenses.

## 🌟 Features

* **Transaction Upload:** 📁 Upload transaction data in CSV format.
* **Data Processing:** ⚙️ Reads the CSV, parses dates/amounts, and categorizes transactions.
* **Categorization:** 🏷️ Automatically categorizes transactions using keywords. Manually edit categories as needed.
* **Visualization:** 📊 Provides a pie chart of expenses by category and a summary of payments.
* **Customizable Categories:** ✏️ Add new categories and keywords.
* **Persistent Categories:** 💾 Categories/keywords are saved in `categories.json` between sessions.
* **Expense and Payment Analysis**: 📈 Separate tabs for viewing and analyzing expenses (debits) and payments (credits).
* **Interactive Data Editing**: ✍️ Uses `st.data_editor` to allow users to edit transaction categories directly in the app.
* **Category Management**: ➕ Users can add new categories via a text input.
* **Detailed Expense Summary**: ℹ️ Displays a dataframe of expense totals per category.

## 🚀 How to Use

1.  **Installation**

    * Clone the repository:

        ```bash
        git clone [https://github.com/RishavB777/Finance-Automation.git](https://github.com/RishavB777/Finance-Automation.git)
        cd Finance-Automation
        ```
    * Create a virtual environment:

        ```bash
        python -m venv venv
        ```
    * Activate the virtual environment:
        * Windows:

            ```bash
            venv\Scripts\activate
            ```
        * macOS and Linux:

            ```bash
            source venv/bin/activate
            ```
    * Install dependencies:

        ```bash
        pip install -r requirements.txt
        ```

2.  **Running the App**

    * Run the Streamlit application:

        ```bash
        streamlit run main.py
        ```

3.  **Using the App**

    * Upload your transaction CSV file.
    * View expenses and payments in separate tabs.
    * Add/edit categories and keywords.
    * Interact with the data and visualizations.

## 🗂️ File Descriptions

* `categories.json`: Stores transaction categories and keywords.
* `main.py`: The main Streamlit application code.
* `requirements.txt`: Lists required Python packages.

## 🛠️ Dependencies

* [Streamlit](https://streamlit.io/): Web application framework.
* [Pandas](https://pandas.pydata.org/): Data manipulation library.
* [Plotly](https://plotly.com/): Visualization library.

## 🗄️ `categories.json` Structure

The `categories.json` file is a JSON dictionary. Keys are category names, and values are lists of keywords.

```json
{
    "Uncategorized": [],
    "Shopping": ["NOON.COM", "LULU HYPERMARKET", "AMAZON AE"],
    "Travel": [],
    "Insurance": ["EMIRATES INSURANCE"],
    "Bank Fee": ["ADCB BANK FEE"],
    "Subscriptions": []
}
