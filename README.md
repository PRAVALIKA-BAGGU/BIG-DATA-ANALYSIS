# BIG-DATA-ANALYSIS
COMOANY : CODTECH IT SOLUTIONS
NAME : PRAVALIKA BAGGU
INTERN ID : CT04DF836
DOMAIN : DATA ANALYSIS
DURATION : 4 WEEKS
MENTOR : NEELA SANTOSH

DESCRIPTION:
This task focuses on analyzing user behavior through activity logs using PySpark in a cloud-based environment, specifically Google Colab. The primary objective is to simulate and study user interaction patterns such as logins, clicks, and logouts by processing a sample dataset and extracting meaningful insights through visualizations.

To begin, the necessary environment is set up. This involves installing Java and Apache Spark, which are required to run PySpark in Colab. Additionally, Python packages like findspark, matplotlib, and seaborn are installed to enable Spark integration and to support visual data exploration.

Once the environment is prepared, a Spark session is initialized to manage data processing tasks. The dataset used is a small, synthetically generated CSV file representing user activity logs. Each row in the dataset includes a user ID, the type of activity they performed (login, click, logout), and the corresponding timestamp. This structure mimics real-world activity tracking in applications, allowing the analysis to simulate genuine business use cases.

The data is loaded into a Spark DataFrame using PySpark’s CSV reader, with schema inference and header recognition enabled. Basic data cleaning is applied to drop any null values in the essential fields and to convert the timestamp column into a proper datetime format using to_timestamp. This ensures that time-based operations like hourly analysis can be performed accurately.

The first analysis focuses on identifying the most active users. By grouping the data by user_id and counting their actions, we determine which users have the highest activity levels. This provides insights into user engagement and helps identify power users or potential bots. The results are converted to a Pandas DataFrame and visualized using Seaborn’s barplot function.

Next, the dataset is enriched by extracting the hour from each activity timestamp. This allows for an analysis of when users are most active during the day. The hourly activity is aggregated, and a bar chart is generated to show trends. For example, higher activity in the morning might indicate business use, while evening peaks could reflect entertainment-related behavior.

Another key insight is derived from the distribution of activity types. Grouping by activity_type and counting their occurrences reveals whether users are primarily logging in, clicking, or logging out. This distribution helps in understanding what kind of interactions dominate the user experience, which can be valuable for feature prioritization or UX improvements.

Throughout the project, visualizations play an important role in communicating findings clearly. Bar charts created using Matplotlib and Seaborn make it easy to interpret trends at a glance. These visuals support decision-making and help validate assumptions about user behavior.

The project concludes by stopping the Spark session to release system resources. While the dataset used is relatively small and synthetic, the approach is scalable and can be applied to large datasets from real applications, such as web server logs, mobile app usage, or IoT telemetry data. This hands-on experience with PySpark prepares learners to handle big data environments and develop insights that support data-driven strategies in real-world organizations.
