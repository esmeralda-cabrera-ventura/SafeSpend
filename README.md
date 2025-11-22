***Attention***

Please read carefully before using the app. 

* Friendly Transparency and Disclaimer Notice – Please Read

This application was designed, built and deployed by James Cao, Esmeralda C. Cabrera Ventura and Tristan Stovall and it is designed to be used by individuals and in one-time/single sessions only. You may temporarily save your data of several months to generate financial trends graphs, but must reset all data before ending a session. This app is not designed for organizational use. Please click on the URL shared above to explore this web app and play with it. We hope you enjoy engaging with our app. 

SafeSpend AI Money Coach is a simple learning project built to demonstrate how Streamlit apps, CSV storage, and GPT-4 can work together to give quick, personalized financial tips. It’s meant to be lightweight, fun, and used for short, single-session financial check-ins, not as a full-scale financial software tool.

To keep the app easy to use, SafeSpend stores information in a temporary shared file behind the scenes. This helps the app remember your inputs during your session, but it also means data isn’t tied to individual accounts.

To keep your information private, we recommend using SafeSpend for quick financial snapshots, and then simply pressing the “Reset Data” button before closing the app. This clears your entries and keeps your information from being accessible to others who might use the link later.

* Why We Mention This

We want to be open about how the app works so you can use it comfortably and confidently. Since this project was designed for personal education and experimentation, it doesn’t include features like logins or private storage. As long as you reset your data at the end of your session, your information stays private and won’t remain in the shared file.

* Your Part (Simple + Quick)

Before exiting your session, just press “Reset Data.”
That’s it — and nothing is stored afterward.

By continuing, you understand how the app works and agree to reset your data when you’re done.

* Our Goal

To give you a simple, intuitive way to get quick, AI-generated financial guidance without any complicated setup — just transparent, friendly use.
Web based product - Link is below

https://safespend-gjwg7qt47fcwuzszcft9kk.streamlit.app/

STEPS TO RECIEVE FINANCIAL ADVICE FROM SAFESPEND AI MONEY COACH

1. User Opens the App
The app is loaded via Streamlit either locally or through Streamlit Cloud.

A sidebar prompts the user to enter their financial details.

2. User Inputs Monthly Financial Data
The sidebar contains fields for:

Monthly Income

Monthly Expenses

Current Savings

Total Debt

Financial Goal (text input)

The user can also enter prior months’ data via a dropdown (optional).

3. User Saves Financial Data
By clicking "Save This Month's Data" or "Save Prior Month's Data", the app:

Writes the entered data into a local CSV file (financial_data.csv)

Ensures data is not duplicated for the same month

4. User Clicks "Get AI Financial Advice"
When clicked, the app checks if a financial goal is entered

It also:

Pulls the most recent saved data from the CSV file

Uses both the new inputs and historical data to form the prompt

5. Prompt Sent to OpenAI API
The app builds a detailed prompt like:

As of April 2025, the user earns $3000 and spends $2200, has $1000 in savings, and owes $5000 in debt. 
The financial goal is: Save for a house.
This prompt is sent to OpenAI’s GPT-4 model via the openai Python SDK.

6. AI Generates Personalized Financial Plan
The model returns a structured response including:

Budgeting tips

Debt repayment strategies

Goal-aligned savings recommendations

The raw output is cleaned up (removing markdown characters, fixing spacing)

7. AI Advice Displayed to User

8. User Can Reuse Advice or Change Inputs
The user can:

Modify inputs and get updated advice

Reset data entirely using the "Reset Data" button

Continue using the app over time to track monthly trends

Technologies Used
Python 3.8+

Streamlit

Pandas

OpenAI GPT-4

Matplotlib (via Streamlit charting)


