# Student Performance Prediction

## Project Overview

This project aims to predict student performance based on various features such as reading score, writing score, gender, ethnicity, parental education level, lunch type, and test preparation course. By analyzing these factors, the model provides insights that can help educators and policymakers enhance educational outcomes.

## Dataset Description

This dataset contains information on the performance of high school students in mathematics, including their grades and demographic information. The data was collected from three high schools in the United States.

## Columns:

- **Gender:** The gender of the student (male/female)

- **Race/ethnicity:** The student's racial or ethnic background (Asian, African-American, Hispanic, etc.)

- **Parental level of education:** The highest level of education attained by the student's parent(s) or guardian(s)

- **Lunch:** Whether the student receives free or reduced-price lunch (yes/no)

- **Test preparation course:** Whether the student completed a test preparation course (yes/no)

- **Math score:** The student's score on a standardized mathematics test

- **Reading score:** The student's score on a standardized reading test

- **Writing score:** The student's score on a standardized writing test

This dataset could be used for various research questions related to education, such as examining the impact of parental education or test preparation courses on student performance. It could also be used to develop machine learning models to predict student performance based on demographic and other factors.

## Table of Contents

- [Project Overview](#project-overview)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Project Structure

The repository is organized as follows:

```
mlproject/
├── artifacts/               # Model artifacts and outputs
├── src/                     # Source code for the project
│   ├── components/          # Data ingestion, transformation, and model trainer scripts
│   └── pipeline/            # Prediction pipeline scripts
├── templates/               # HTML templates for the Flask app
├── app.py                   # Flask application script
├── requirements.txt         # Python dependencies
├── setup.py                 # Package setup script
└── README.md                # Project documentation
```

## Installation

To set up the project locally, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/mlproject.git
   cd mlproject
   ```

2. **Create and activate a virtual environment:**

   - For Windows:

     ```bash
     python -m venv venv
     venv\Scripts\activate
     ```

   - For macOS/Linux:

     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```

3. **Install the required packages:**

   ```bash
   pip install -r requirements.txt
   ```

## Usage

To run the Flask application:

```bash
python app.py
```

Access the application by navigating to `http://127.0.0.1:5000/` in your web browser. Here, you can input student data to receive performance predictions.

## Deployment

To deploy the application using Docker:

1. **Build the Docker image:**

   ```bash
   docker build -t student-performance-app .
   ```

2. **Run the Docker container:**

   ```bash
   docker run -p 5000:5000 student-performance-app
   ```

The application will be accessible at `http://localhost:5000/`.

## Contributing

Contributions are welcome! To contribute:

1. **Fork the repository.**
2. **Create a new branch:**

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Commit your changes:**

   ```bash
   git commit -m 'Add some feature'
   ```

4. **Push to the branch:**

   ```bash
   git push origin feature/your-feature-name
   ```

5. **Open a pull request.**

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

