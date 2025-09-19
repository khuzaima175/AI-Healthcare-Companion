# 🤖 AI-Powered Smart Calorie Tracker Pro


An advanced, desktop-based calorie and nutrition tracker built with Python and CustomTkinter. This application leverages the power of Google's Gemini AI to understand natural language for effortless food logging, analyze meal photos, and provide intelligent dietary feedback.

## ✨ Key Features

-   **AI Nutrition Analysis**: Simply type what you ate (e.g., *"2 eggs, a slice of toast with butter, and a banana"*) and let the AI calculate the nutritional information.
-   **📷 Image-to-Text Food Logging**: Snap a picture of your meal, and the AI will generate a text description for you to log.
-   **Modern & Animated UI**: A sleek, professional interface built with CustomTkinter, featuring smooth animations for progress bars and state changes.
-   **Comprehensive Dashboard**: The "Daily Log" tab provides an at-a-glance view of your net calories, macronutrients, and hydration with visually appealing progress cards.
-   **📊 Data Visualization**: Interactive charts powered by Matplotlib to track your macro distribution, weekly trends, and more.
-   **🤖 AI Coach & Meal Planner**: Get personalized dietary advice and generate sample meal plans based on your calorie targets and dietary preferences.
-   **Local Database Storage**: All your data is stored locally and privately in a SQLite database (`calorie_tracker.db`).
-   **Full History & Data Export**: Review your nutritional history over any date range and export your daily logs to a CSV file.

## 🛠️ Technology Stack

-   **Frontend**: Python with [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)
-   **AI & Language Model**: [Google Gemini API](https://ai.google.dev/) (via `google-generativeai`)
-   **Data Visualization**: [Matplotlib](https://matplotlib.org/)
-   **Image Handling**: [Pillow (PIL)](https://python-pillow.org/)
-   **Database**: SQLite3 (built-in)

## 🚀 Getting Started

Follow these steps to set up and run the project on your local machine.

### 1. Prerequisites

-   Python 3.10 or newer
-   A Google Gemini API Key. You can get one for free from [Google AI Studio](https://aistudio.google.com/app/apikey).

### 2. Installation & Setup

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name
    ```

2.  **Create a virtual environment (recommended):**
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required packages:**
    ```sh
    pip install -r requirements.txt
    ```
    *(Note: If you don't have a `requirements.txt` file, create one with `pip freeze > requirements.txt` after installing the packages listed below)*
    ```sh
    pip install customtkinter google-generativeai matplotlib pillow
    ```

4.  **Add your API Key:**
    Open the `main.py` file and find this line (around line 21):
    ```python
    api_key = "AIzaSyARiMM-cfeVHABE0q47hb14RBh0Z7mImV4"  # Replace with a valid key
    ```
    Replace the placeholder key with your own Google Gemini API key.

5.  **Add UI Icons:**
    -   Create a folder named `assets` in the root of the project directory.
    -   Download and place the required `.png` icon files into this folder. A suggested list is below:
        -   `logo.png`
        -   `arrow-left.png`, `arrow-right.png`
        -   `droplet.png`, `activity.png`, `download.png`
        -   `camera.png`, `plus.png`
        -   `list.png`, `graph.png`, `robot.png`
        -   `history.png`, `plan.png`, `settings.png`

### 3. Running the Application

Once the setup is complete, run the main script from the project's root directory:

```sh
python main.py

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.
