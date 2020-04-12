# insta-trends
 Trend detector for Instagram stories with Tensorflow


## Usage

### Obtain list of usernames to scrape:

You'll need a *usernames.txt* file with a list of users to scrape stories from. If you want a list of users that follow an user, you can use **usernames_finder** script to do this. Put your IG login and the target profile. The script will create a usernames.txt file with all the followers of the target profile. We will use this list to scrape the stories. 

### Scrape stories with PyInstaStories

Use the **pyinstastories** script to do this. 

>```elm
>python3 pyinstastories.py --batch-file usernames.txt --username [YOUR USERNAME] --password [YOUR PASSWORD]
>```

Note that the above command will scrape stories only from public users and private users that your account follows. It's recommended to use a bot to follow all the targets.