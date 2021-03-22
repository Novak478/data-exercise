# Instructions for Zack Novak's data-exercise test



### My dev setup

- Developed in VS Code on Windows 10 using WSL 2.

### Time log
- 3/19/21 5:57 PM EDT: debugged rusty Windows environment and got example up and running. Logged off and called it a day! Total dev time: ~1 minute
- 3/20/21 11:15 AM EDT: While getting ready to start, I noticed my kernel in the jupyter noteobook was funky. Went down a fix-it rabbithole, and ended up having to make some changes in WSL2, and was able to get it running by adding:  `ENV JUPYTER_ALLOW_INSECURE_WRITES=true` to the dockerfile. Called it a day after that. I did play around the the problem locally in another shell, so calling total dev time: ~30 minutes. [GitHub Link](https://github.com/jupyter/notebook/issues/5058) for issue I had. No changes to deployment structure.
- 3/21/21 11:20 PM EDT: 