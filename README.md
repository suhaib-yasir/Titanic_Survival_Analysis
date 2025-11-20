# 🚢 Titanic Survival Analysis

## Project Overview
This project performs an **Exploratory Data Analysis (EDA)** and **Machine Learning** analysis on the famous Titanic dataset to predict and understand the factors that influenced a passenger's survival. The main objective is to clean the data, engineer relevant features, visualize key relationships, and build a classification model to determine who survived the disaster.

## 🎯 Objective
The primary goals of this analysis are:
1.  To conduct a comprehensive EDA to uncover patterns and relationships in the dataset.
2.  To visualize the distribution of key variables (Age, Fare, Class, Sex) and their correlation with survival status.
3.  To preprocess the data, handle missing values, and engineer new features (e.g., family size, title).
4.  To develop a machine learning classification model to predict passenger survival.

## 📂 Project Structure
The repository contains the following files and directories:

| File/Folder | Description |
| :--- | :--- |
| `Titanic_Survival_Analysis_Notebook.ipynb` | The main Jupyter Notebook containing all the EDA, feature engineering, visualization, and machine learning model building steps. |
| `train.csv` | The raw training dataset used for the analysis. |
| `Age Distribution by Survival Status.png` | Visualization showing age distribution segmented by survival status. |
| `Survival Rate by Sex.png` | Visualization highlighting the survival rates for male vs. female passengers. |
| `Survival Rate by Passenger Class.png` | Visualization showing survival rates across Pclass (1st, 2nd, 3rd). |
| `Distribution of Fare.png` | Histogram showing the distribution of passenger fares. |
| `... other *.png files` | Various other plots and visualizations generated during the EDA phase. |

## 🛠 Technology Stack
The analysis is implemented using Python and relies heavily on the following libraries:

* **Python 3.x**
* **Jupyter Notebook**: For interactive coding, analysis, and documentation.
* **Pandas**: For data manipulation and analysis.
* **NumPy**: For numerical operations.
* **Matplotlib / Seaborn**: For data visualization.
* **Scikit-learn**: For machine learning model implementation and evaluation.

## 🚀 Installation and Setup

### Prerequisites
Make sure you have **Python 3.x** installed on your system.

### Steps
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/suhaib-yasir/Titanic_Survival_Analysis.git](https://github.com/suhaib-yasir/Titanic_Survival_Analysis.git)
    cd Titanic_Survival_Analysis
    ```
2.  **Create and activate a virtual environment (Recommended):**
    ```bash
    python -m venv venv
    # On Windows
    .\venv\Scripts\activate
    # On macOS/Linux
    source venv/bin/activate
    ```
3.  **Install the necessary packages:**
    (A detailed `requirements.txt` is recommended, but based on the notebook, the core libraries are below)
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn jupyter
    ```
4.  **Run the analysis:**
    Launch the Jupyter Notebook server and open the main notebook.
    ```bash
    jupyter notebook Titanic_Survival_Analysis_Notebook.ipynb
    ```

## 📊 Key Findings & Results
* **Gender Bias:** **Females** had a significantly higher survival rate than males ("Women and children first" protocol). This is typically the strongest predictor.
* **Socioeconomic Status:** Passengers in **First Class (Pclass=1)** had a much higher chance of survival compared to those in 2nd and 3rd class.
* **Age and Survival:** Children (especially those under 10) had better survival rates than older individuals, particularly men.
* **Feature Importance:** Features like `Sex`, `Pclass`, and engineered features such as `FamilySize` (from SibSp and Parch) are highly correlated with the target variable (`Survived`).

The machine learning model (e.g., Logistic Regression, Decision Tree, or Random Forest) built in the notebook typically achieves an accuracy of **[Insert Model Accuracy Here, e.g., ~80%]** on the test data.

## 🤝 Contribution
Feel free to fork the repository and submit pull requests. Any suggestions for improving the EDA, feature engineering, or model performance are welcome!
