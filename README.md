# YouTube-Data-Harvesting-and-Warehousing-using-SQL-MongoDB-and-Streamlit

This project aims to develop a user-friendly Streamlit application that utilizes the Google API to extract information on a YouTube channel, stores it in a MongoDB database, migrates it to a SQL data warehouse, and enables users to search for channel details and join tables to view data in the Streamlit app.

API Reference
Get all items
  GET /api/items
Parameter	Type	Description
api_key	string	AIzaSyDY1V7Solq7mGGX1yCVB2TV-bJiQq9hoVE
Get item
  GET /api/items/${id}
Parameter	Type	Description
id	string	channel_id
Acknowledgements
I would like to express my sincere thanks to the following individuals

Mr. Mohammed Hassan (@guvi) :Special thanks for providing guidance and reviewing the project documentation.
Mr. Suriya Prakash N (@guvi) :Thank you for your valuable code contributions and bug fixes.
Data source: The data used in this project was sourced from developers.google.com. We appreciate their data availability.
Your contributions and support have been instrumental in the success of this project.

Installation
1.Install the required packages:

import streamlit as st
from streamlit_option_menu import option_menu
from googleapiclient.discovery import build
import pymongo
from pymongo import MongoClient
import pandas as pd
import pymysql
from pprint import pprint
import datetime
import re
2.Set up your MongoDB and MySQL databases and update the connection configurations in the code.

3.Obtain a YouTube API key and replace 'your-api-key' with your actual API key in the code.

Usage
Data Collection:

To collect data from a YouTube channel, run the application and select the "DATA COLLECTION" option. Enter the channel ID when prompted and click "Extract." The collected data will be displayed and stored in MongoDB.

Select and Store :

This option allows you to select a channel from the stored data in MongoDB and push it into a MySQL database. Choose "SELECT AND STORE," select a channel, and click "Push into SQL" to migrate the data.

Migration of Data :

Choose the "MIGRATION OF DATA" option to push data from MongoDB to MySQL. You can select a channel and migrate its data to the MySQL database.

Data Analysis:

Select the "DATA ANALYSIS" option to perform various data analysis queries, such as finding the most viewed videos, channels with the most videos, and more.

Environment Variables
Environment variables are dynamic-named values that affect the way processes run on a computer.
They are part of the environment in which a process runs.
Each environment variable is typically composed of a name and a value, e.g., DATABASE_URL with a value like .


LINK
LINKEDIN
www.linkedin.com/in/g-rakesh01
