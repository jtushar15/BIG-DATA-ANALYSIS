# BIG-DATA-ANALYSIS

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: TUSHAR RAMDAS JADHAV

*INTERN ID*: CT12KEV

*DOMAIN*: DATA ANALYSIS

*DURATION*: 8 WEEKS(January 5th, 2025 to March 5th, 2025.)

*MENTOR*: NEELA SANTOSH

# BIG DATA ANALYSIS USING PYSPARK

The notebook starts by installing PySpark using !pip install pyspark, ensuring that the required library is available for use. It then initializes a SparkContext (sc), which is the core engine that handles distributed data processing. The version of Spark is printed to verify the setup. After that, a SparkSession (spark) is created using SparkSession.builder.getOrCreate(), which is essential for working with structured data like DataFrames and SQL tables in Spark. The SparkSession acts as the entry point for all DataFrame-based operations.

The next section demonstrates how PySpark integrates with Pandas. It first creates a Pandas DataFrame (pd_temp) with 10 random values using NumPy. This DataFrame is then converted into a Spark DataFrame (spark_temp) using spark.createDataFrame(pd_temp), allowing large-scale processing. The notebook interacts with the Spark catalog, which manages metadata about tables. The command spark.catalog.listTables() is used to check the available tables before and after registering the DataFrame as a temporary table using createOrReplaceTempView("temp"). This allows SQL-style queries on the DataFrame, making it easier to analyze large datasets.

The final part of the notebook reads an external dataset (airports.csv) using spark.read.csv(file_path, header=True). This command loads the CSV file into a Spark DataFrame (airports), treating the first row as column headers. The dataset is then displayed using airports.show(), which prints the first few rows. This step showcases how PySpark can handle structured data from external files, making it suitable for big data analytics, ETL pipelines, and machine learning workflows.

*Combining SQL and DataFrame APIs*

PySpark allows seamless integration of SQL queries with DataFrame transformations.Both methods produce the same result but use different approaches.Both methods produce the same result but use different approaches.

# OUTPUTS:-

Airpots_data:
![Image](https://github.com/user-attachments/assets/bac69899-fb89-4bc3-9a9d-7f72470c9647)

Filghts_data:
![Image](https://github.com/user-attachments/assets/5e9e7261-1ccc-4428-b7a0-667f3fabc8e0)

Planes_data:
![Image](https://github.com/user-attachments/assets/e1edaa5b-d934-416a-9178-70fc8b3ba2c2)

Output of Analysis:
![Image](https://github.com/user-attachments/assets/2af5c805-d450-4b88-a71d-0daf6da779a3)

# Conclusion of the PySpark Project
This PySpark project demonstrates how to efficiently process and analyze large datasets using Apache Spark. By leveraging SparkContext and SparkSession, the project sets up a scalable environment for handling distributed data. The integration of Pandas with PySpark highlights the transition from small-scale data processing to a big data framework, ensuring flexibility in data analysis.

Key operations performed in the project include creating DataFrames, registering temporary SQL tables, and executing SQL queries to filter and transform data. The project also showcases reading structured data from CSV files, applying DataFrame transformations (such as filtering, grouping, and sorting), and using SQL-like operations for efficient data manipulation. These techniques help in real-world applications like ETL (Extract, Transform, Load) pipelines, data warehousing, and machine learning preprocessing.

Overall, the project highlights the advantages of PySpark for big data processing by combining the power of distributed computing, SQL-based querying, and scalable transformations. PySpark’s capabilities make it an essential tool for working with large datasets in industries such as finance, healthcare, retail, and artificial intelligence. Future improvements could include machine learning integration using Spark MLlib or real-time data processing with Spark Streaming. 🚀

Would you like me to add anything, such as next steps, optimization tips, or real-world applications? 😊
