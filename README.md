# Python Twitter Follower and Following Count App
This is a Python application that allows you to get the follower and following counts for multiple Twitter handles and sends the result as an Excel file via email.

# Prerequisites
Before running the app, you need to:

Have a Twitter account and obtain Twitter API credentials (consumer key, consumer secret, access token, and access token secret) from the Twitter Developer Portal.
Have a Gmail account to send the email from and enter your email credentials (sender email address and password) in the code.
Have a receiver email address to send the email to and enter it in the code.
Install the required libraries using the following command:
```bash
pip install tweepy openpyxl schedule
```
Usage
Clone or download the Python script to your computer.
Open the script and enter your Twitter API credentials, email credentials, and receiver email address in the corresponding variables at the beginning of the script.
Enter the Twitter handles you want to get the follower and following counts for in the twitter_handles list.
Uncomment the line schedule.every(1).minutes.do(get_follower_counts) to test the app by scheduling it to run every minute or leave it commented to run it every day at 11:30 pm.
Run the script and let it run continuously in the background.
The app will create an Excel file named twitter_followers_following_YYYY-MM-DD_HH-MM-SS.xlsx with the current date and time as the filename in the same directory as the script.
The app will send an email with the Excel file as an attachment to the receiver email address.
Note: In order to authenticate with Google SMTP servers, the user must generate a Google app password and enter it in the code.

Contributing
Feel free to fork the repository, make changes, and submit a pull request if you'd like to contribute to this app.

License
This app is licensed under the MIT License.
