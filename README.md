# td-mathamatica-api
A basic project to allow live pricing data from TD Ameritrade API to be imported into a Mathematica notebook. 

# Some benefits of TD's API
I was able to sign up for both a DTD brokerage account and developer portal in a few hours. There was no real paper work to fill out. 
Once you have your token, TD does provide live stock and options data which was the main thing i was looking for.

# Getting your TD Refresh Token
By far the hardest part of this process is getting the refresh token from TD. It took me half a day to find this guide, and from there it was only about one hours work. https://www.reddit.com/r/algotrading/comments/c81vzq/td_ameritrade_api_access_2019_guide/ . Do this first, and come back once you have a refresh token. 

Your client ID is available from the application you register in your TD Developer account, its much simpler to get.


# Inputting your Token and Client ID into the file
The only two variables you need to update her are refresh token and clientid, every thing else you just need to re-evaulate once you have those. 

I have hidden all the outputs with the ; at the end of each line. If it isn't working for you, removing those might give you an idea as to why.

# Using the token to get data from the API

# Extending
This is making use of one endpoint, the main other interesting ones are the options chain, which I will work on next and some of the automatic trading ones.

I am in no way a Mathematica programmer, I have some experince working with API's which is how I figured this out. There may be better methods than URL Fetch, but this worked first for me.


# Contributing
It woudl be great to improve this wrapper to make it cleaner and add more endpoints.  Please make a PR for any changes you make and I will merge it so we can all benefit from it. 

# Other useful notes
A very comprehensive python wrapper exists https://github.com/alexgolec/tda-api. If you are looking to build a a more comperehensive application, Alex's repo would be a great starting point. 
