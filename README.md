# Instructions for Zack Novak's data-exercise test

1. Run `docker-compose up --build`
2. Open the jupyter notebook `data-exercise`.
3. Adjust the variable `results_wanted` for the number of fake API calls to make. Default is 1000.
4. Left click `Cell` and select `Run all`. 
5. View data visualizations / statistics at bottom of notebook. 

## APIS USED!

1. Random, fake user data from randomuser.me/api
2. Random quotes from all over from https://quote-garden.herokuapp.com/api
3. Kanye West quotes from https://kanye.rest/
4. Taylor Swift quotes from https://taylor.rest/
5. Game of Thrones quotes from https://gameofthronesquotes.xyz/

### Example problem

I am a data engineer working for a local bank trying to assist service reps with our new online chat service. In order to understand the current environment, I've recorded quotes from customer's chats with our service reps to establish a base line for the chatbot to compare against in the future.

### My dev setup

- Developed in VS Code on Windows 10 using WSL 2.

### Time log
- 3/19/21 5:57 PM EDT: debugged rusty Windows environment and got example up and running. Logged off and called it a day! Total dev time: ~1 minute
- 3/20/21 11:15 AM - 11:45 AM EDT: While getting ready to start, I noticed my kernel in the jupyter noteobook was funky. Went down a fix-it rabbithole, and ended up having to make some changes in WSL2, and was able to get it running by adding:  `ENV JUPYTER_ALLOW_INSECURE_WRITES=true` to the dockerfile. Called it a day after that. I did play around the the problem locally in another shell, so calling total dev time: ~30 minutes. [GitHub Link](https://github.com/jupyter/notebook/issues/5058) for issue I had. No changes to deployment structure.
- 3/21/21 11:20 PM - 12:00 AM EDT: Added code from flask with random user data api. Cleaned it up and expiremented with an idea of using cryptocurrency data, but ultimately decided not to pursue it. Total dev time: ~1 hr 10 min.
- 3/22/21 5:00 PM - ~ 6:00 PM EDT: Added a few other API calls regarding quotes, a profanity API, and a text analysis. Total dev time: ~2 hrs 10 min.
- 3/22/21 11:00 PM - 11:50 PM EDT: Finished all api calls / creation of final df. Got killed by a Spectrum outage in my area, so unable to continue further / push. Total dev time: ~ 3 hrs.
- 3/23/21 11:30 AM - 12:30 PM EDT: Final touches with stats, data visualizations, and struggling with loading the dataframe into neo4j. Added some pseudocode to show what I would have done after resolving the error of loading. Total dev time: 4 hrs. FINAL COMMIT! 