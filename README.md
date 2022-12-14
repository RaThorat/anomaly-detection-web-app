# anomaly-detection-web-app

This is a web app that displays different types of graphs and figures based on uploaded data. It allows users to upload a file and then displays various graphs and figures based on the data in that file. The app is built using the Python library Dash and makes use of various other libraries such as numpy, pandas, and plotly.

To run this app, use the command python app.py and visit http://127.0.0.1:8050/ in your web browser. The app is built using external stylesheets and the Bootstrap theme, which can be customized by the user.

The app layout is made up of a series of rows and columns that display different types of graphs and figures. There is a section for uploading files, as well as sections for displaying the most common and largest applicants and the top 5 matches in the register data. The app also has a function for removing empty rows in the uploaded data for better readability.

The app is built using Dash's interactive components, allowing users to interact with the displayed figures and graphs. It makes use of various Dash dependencies such as Input, Output, and State to handle user interactions and update the displayed figures and graphs accordingly.

## files info

Repository contains app.py, a python file to run the script, example_input_data.xlsx as an example file to upload in the web app, example_register_data.xlsx as an example file which is saved in pythonanywhere website for checking whether the Chamber of Commerce number is present in the anomaly registry. The repository also contains a file of the image after uploading the input data for showing results.

A web app is built to detect anomalies in a set of grant application. 


 # The anomalies detected are:

 whether the name of applicant appears several times in the datasheet or

 whether the name of the company appears several times in the datasheet or

 whether the bank account number of the company appears several times in the datasheet or

 whether more than 100,000 euros was requested or

 whether the Chamber of Commerce number is present in the anomaly registry

# Input data:

The data (example_input_data.xlsx) is encrypted with Python hash codes. A fake anomaly registry (example_register_data.xlsx) contains applicant information that have abused the grant in the past.

# Python code: 

The code is written in Python with Dash plotly. I used following file to start:

https://github.com/RaThorat/proposal_info_Elsevier_Expert_Lookup_02/blob/main/Dashapp_Proposals_info_for_Expert_Lookup.py

I followed instruction videos from charming data for style, bootstrap, decorators etc.:

https://www.youtube.com/watch?v=0mfIK8zxUds&t=13s

https://www.youtube.com/watch?v=vqVwpL4bGKY&list=RDCMUCqBFsuAz41sqWcFjZkqmJqQ&index=4

https://www.youtube.com/watch?v=mTsZL-VmRVE&list=RDCMUCqBFsuAz41sqWcFjZkqmJqQ&index=5

# Deployment: 

I tried first with Azure to deploy the web app, however there was problem with the connection between github repository and the Azure. I switched to pythonanywhere.com for deploying the web-app on following instruction video from charming data:

https://www.youtube.com/watch?v=WOWVat5BgM4

I highly recommend this video.

# Handeling intructions:

You can either open the code in you IDE, run it and visit http://127.0.0.1:8050/ in your web browser or
visit the webapp on the following website

# https://rathorat.pythonanywhere.com/ 
 
Once in the web browser, you will see the possibility to upload Excel example_input_data.xlsx. As soon as you upload the excel sheet, the analysis starts. On the screen you can see an output file with the reference numbers that meet the criteria. You will also see a number of summary graphs.
You can download the output file by clicking the 'Export' button.
