# Netflix Dataset EDA with PySpark

This project leverages Apache Spark to analyze and explore the Netflix dataset. It demonstrates the usage of PySpark for data ingestion, transformation, and visualization of key insights from the dataset.

## Features

1. **Basic Dataset Information**
   - Prints the schema of the dataset.
   - Displays the total number of records.

2. **Content Type Distribution**
   - Shows the distribution of content types (e.g., Movies, TV Shows).

3. **Yearly Content Production**
   - Analyzes the number of movies and TV shows produced each year.

4. **Top 10 Countries Producing Content**
   - Lists the top 10 countries based on the number of content pieces produced.

5. **Rating Distribution**
   - Displays the distribution of ratings across the dataset.

## Setup and Usage

### Prerequisites
- Python 3.x
- Apache Spark
- PySpark library

### Steps to Run
1. **Set up the environment:**
   Ensure that PySpark is installed and properly configured on your system.

2. **Prepare the dataset:**
   Download the `netflix_titles.csv` dataset and place it in the project directory.

3. **Run the Notebook:**
   - Open the Jupyter Notebook file in your environment.
   - Execute the cells sequentially to perform the analysis.

4. **Output:**
   The results of the analysis will be displayed directly in the notebook.

## Project Structure

- **`create_spark_session`**: Initializes a SparkSession for the project.
- **`load_netflix_dataset`**: Loads the Netflix dataset into a Spark DataFrame.
- **`perform_eda`**: Performs the following analyses:
  - Prints schema and total record count.
  - Aggregates and displays content type distribution.
  - Analyzes yearly content production trends.
  - Identifies the top 10 content-producing countries.
  - Displays the rating distribution.

## Example Output

1. **Schema Overview**  
   The dataset schema includes fields like `show_id`, `type`, `title`, `release_year`, `rating`, and more.

2. **Content Type Distribution**  
   Example:
   ```
   +--------+-----+
   |  Type  |Count|
   +--------+-----+
   | Movie  | 6131|
   |TV Show | 2676|
   +--------+-----+
   ```

3. **Top 10 Content-Producing Countries**  
   Example:
   ```
   +--------------+-------------+
   | Country      | Content Count|
   +--------------+-------------+
   | United States| 2805         |
   | India        | 972          |
   +--------------+-------------+
   ```

## Credits

The project uses the Netflix dataset available from [Kaggle](https://www.kaggle.com/shivamb/netflix-shows).