# 🎫 Customer Support Ticket Analyzer

This project is a machine learning pipeline designed to automatically classify customer support tickets. It predicts the **issue type** and **urgency level**, and extracts key **entities** (like product names and dates) from the ticket text. This helps in routing tickets to the correct department and prioritizing critical issues.

## ✨ Features

-   **Data Preprocessing**: Cleans and normalizes raw ticket text for optimal model performance.
-   **Multi-Task Classification**: Trains two separate models to predict:
    1.  **Issue Type** (e.g., "Technical Issue", "Billing", "Shipping")
    2.  **Urgency Level** ("Low", "Medium", "High")
-   **Entity Extraction**: Identifies and extracts key information from the ticket, such as:
    -   Product names
    -   Dates
    -   Complaint-related keywords
-   **Comprehensive Feature Engineering**: Utilizes TF-IDF for text vectorization and incorporates additional features like text length, word count, and sentiment scores.
-   **Model Evaluation**: Includes detailed classification reports and confusion matrices to assess model performance.

## 🛠️ Tech Stack

-   **Language**: Python 3
-   **Core Libraries**: Pandas, NumPy, Scikit-learn, NLTK, TextBlob
-   **Data Visualization**: Matplotlib, Seaborn
-   **Environment**: Jupyter Notebooks or any Python IDE

## 🚀 Getting Started

Follow these steps to set up and run the project locally.

### 1. Prerequisites

-   Python 3.8 or higher
-   `pip` package manager

### 2. Clone the Repository

```bash
git clone [https://github.com/your-username/ticket-analyzer.git](https://github.com/your-username/ticket-analyzer.git)
cd ticket-analyzer
```

### 3. Set Up a Virtual Environment

It is highly recommended to use a virtual environment to manage dependencies.

```bash
# Create the virtual environment
python3 -m venv venv

# Activate it
# On macOS/Linux:
source venv/bin/activate
# On Windows:
.\venv\Scripts\activate
```

### 4. Install Dependencies

Install all the required libraries using the `requirements.txt` file.

```bash
pip install -r requirements.txt
```

### 5. Place the Dataset

Ensure the dataset file `ai_dev_assignment_tickets_complex_1000.xls` is placed in the root directory of the project.

### 6. Run the Script

Execute the main Python script to train the models and see an example prediction.

```bash
python app.py
```

The script will print the model evaluation reports and a JSON output for a sample ticket.

## 📁 Project Structure

```
.
├── ai_dev_assignment_tickets_complex_1000.xls  # The
