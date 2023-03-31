# MIST4610
Group Project 1

Group # 21479_8

Members:
- Donovan Vanderpool (me) https://github.com/donovanv2/MIST4610/ 
- Emma Dolson https://github.com/eld49325/EmmaDolson_MIST4610GroupProject1
- Hannah Kelly https://github.com/hannahkelly98765/MIST-4610
- Shir Kochi https://github.com/shirkorchi/GroupProject1
- Kaden Williams (insert link)

PROBLEM DESCRIPTION

Our data model represents the social media app, Instagram. The model consists of user accounts, which have associated profiles, content, and followers/following relationships. Each post can have multiple associated media, such as images or videos, which users can interact with through likes, comments, and shares. Instagram also supports messaging between users and the creation of stories, which are temporary posts that expire after a set time period. Tracking user activity helps Instagram generate personalized recommendations and trends to improve user experience. Despite being one of the most popular social media platforms in the world, Instagram does not allow its users to schedule posts in advance or to create communities of niche interests. From a backend perspective, our model demonstrates how users would interact with these two features and new insights Instagram could gain from them.

DATA MODEL

![image](https://user-images.githubusercontent.com/129460719/228989935-6fdb6b22-255a-4931-9141-fa0d99884e57.png)

1:M Relationships: users have many accounts, users can send many messages, users can receive many messages, content schedule can schedule multiple content, accounts can have many shares, content can have many shares, accounts can have many comments, comments can be added to multiple content, accounts can have many likes, likes can be given to multiple content.

M:M Relationships: accounts can belong to many communities and communities can have many accounts, communities can have many community types and community types can have many communities

DATA DICTIONARY

[Data.Dictionary.pdf](https://github.com/donovanv2/MIST4610/files/11117019/Data.Dictionary.pdf)

QUERIES

TP_Q1: This query converts the user's date of birth into their age as an integer and then returns the names of users who are younger than the input age. A query like this is helpful for censoring content like rated R movie trailers or explicit music for underage users.

![image](https://user-images.githubusercontent.com/129460719/228990792-3ad14c81-598c-4521-b475-90ddb5a70072.png)


TP_Q2: This query returns the username of accounts that have more followers than the average amount of followers for all accounts. A manager may be interested in this information to improve its algorithm and search engine.

![image](https://user-images.githubusercontent.com/129460719/228990847-9a50728d-7a35-4141-bfb0-48994db87149.png)

TP_Q3

TP_Q4

TP_Q5

TP_Q6

TP_Q7: This query will list the name and DOB of users that send messages with vanish mode and use content scheduling in order of oldest to youngest. A query like this is useful for tracking the use of some of the new features on Instagram.

![Screenshot (71)](https://user-images.githubusercontent.com/129460719/228991572-ebef94b6-4637-4f4e-9e35-87513edb5a54.png)

TP_Q8: This query will list accounts’ ID, handle, and the user’s name and email address associated with the accounts that have no video content posted. A query like this is useful for being able to identify and contact individuals to promote Instagram’s video functionality.

![Screenshot (72)](https://user-images.githubusercontent.com/129460719/228991659-7a6e298b-14dd-4023-a343-6f4772a1fee3.png)

TP_Q9: This query returns the account type and number of times each account type schedules content. A query like this could be helpful for adding possible features that cater towards account types that are frequent users of the content scheduler (ex. If a sports team has games every Saturday at noon, they can schedule a recurring post for each week of the season).

TP_Q10

