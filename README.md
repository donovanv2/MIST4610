# MIST4610 Group Project 1

Group # 21479_8

# Members:
- Donovan Vanderpool
- [Emma Dolson](https://github.com/eld49325/EmmaDolson_MIST4610GroupProject1)
- [Hannah Kelly](https://github.com/hannahkelly98765/MIST-4610)
- [Shir Kochi](https://github.com/shirkorchi/GroupProject1)
- [Kaden Williams](https://github.com/kadenwilliams1/21479_-8)

# PROBLEM DESCRIPTION

Our data model represents the social media app, Instagram. The model consists of user accounts, which have associated profiles, content, and followers/following relationships. Each post can have multiple associated media, such as images or videos, which users can interact with through likes, comments, and shares. Instagram also supports messaging between users and the creation of stories, which are temporary posts that expire after a set time period. Tracking user activity helps Instagram generate personalized recommendations and trends to improve user experience. Despite being one of the most popular social media platforms in the world, Instagram does not allow its users to schedule posts in advance or to create communities of niche interests. From a backend perspective, our model demonstrates how users would interact with these two features and new insights Instagram could gain from them.

# DATA MODEL

![image](https://user-images.githubusercontent.com/129460719/228989935-6fdb6b22-255a-4931-9141-fa0d99884e57.png)

1:M Relationships: users have many accounts, users can send many messages, users can receive many messages, content schedule can schedule multiple content, accounts can have many shares, content can have many shares, accounts can have many comments, comments can be added to multiple content, accounts can have many likes, likes can be given to multiple content.

M:M Relationships: accounts can belong to many communities and communities can have many accounts, communities can have many community types and community types can have many communities

# DATA DICTIONARY

[Data.Dictionary.pdf](https://github.com/donovanv2/MIST4610/files/11117019/Data.Dictionary.pdf)

# QUERIES

TP_Q1: This query converts the user's date of birth into their age as an integer and then returns the names of users who are younger than the input age. A query like this is helpful for censoring content like rated R movie trailers or explicit music for underage users.

![image](https://user-images.githubusercontent.com/129460719/228990792-3ad14c81-598c-4521-b475-90ddb5a70072.png)


TP_Q2: This query returns the username of accounts that have more followers than the average amount of followers for all accounts. A manager may be interested in this information to improve its algorithm and search engine.

![image](https://user-images.githubusercontent.com/129460719/228990847-9a50728d-7a35-4141-bfb0-48994db87149.png)

TP_Q3: This query returns the number of messages a community has sent if the message was sent during the day (12:00-18:00). A query like this is can be helpful in determining when communities are most active or when messaging servers could potentially reach capacity. 

![image](https://user-images.githubusercontent.com/129460719/229161944-acbf5ff2-66db-4976-a5c7-8bbf8b8b4e45.png)

TP_Q4: This query returns the number of messages each account has sent in descending order given that the account has more than 500 followers. A manager may be interested in this data to gauge how active a particular account is.

![image](https://user-images.githubusercontent.com/129460719/229162104-b7ed3827-d062-480d-bb7a-4d5e41690fda.png)

TP_Q5: This query returns the account handles that start with the letter "c," if any, as well as the name of the corresponding user and the community they belong to. A manager may be interested in this data to view information about accounts with related names quickly (by replacing “c” with whichever letter they choose).

![image](https://user-images.githubusercontent.com/129460719/229162207-a1ffe2e8-16c7-4c60-b6d8-d44b3e5d1825.png)

TP_Q6: This query returns all attributes pertaining to accounts and the community they're a part of if the account uses content scheduling. A query like this may be helpful in determining certain attributes (type of account, number of posts, etc.) that may play a factor in determining whether or not the account uses the content scheduling feature.

![image](https://user-images.githubusercontent.com/129460719/229162311-4271d6ac-1cc7-429e-a6aa-70c7b883f5f6.png)

TP_Q7: This query will list the name and DOB of users that send messages with vanish mode and use content scheduling in order of oldest to youngest. A query like this is useful for tracking the use of some of the new features on Instagram.

![Screenshot (71)](https://user-images.githubusercontent.com/129460719/228991572-ebef94b6-4637-4f4e-9e35-87513edb5a54.png)

TP_Q8: This query will list accounts’ ID, handle, and the user’s name and email address associated with the accounts that have no video content posted. A query like this is useful for being able to identify and contact individuals to promote Instagram’s video functionality.

![Screenshot (72)](https://user-images.githubusercontent.com/129460719/228991659-7a6e298b-14dd-4023-a343-6f4772a1fee3.png)

TP_Q9: This query returns the account type and number of times each account type schedules content. A query like this could be helpful for adding possible features that cater towards account types that are frequent users of the content scheduler (ex. If a sports team has games every Saturday at noon, they can schedule a recurring post for each week of the season).

![image](https://user-images.githubusercontent.com/129460719/229162414-a116c7be-4036-405d-b00e-b2585ed813a4.png)

TP_Q10: This query returns the number of shares for each content type. A manager may be interest in this data to determine what type of content is shared the most among users (could be useful for ad monetization, promotions, etc.).

![image](https://user-images.githubusercontent.com/129460719/229162581-0c6b3c69-814e-4378-a8ea-7805f8de9449.png)

# QUERY MATRIX

![Screenshot (73)](https://user-images.githubusercontent.com/129460719/229194749-404c2315-52e5-4e91-b94c-0162a9dfbd68.png)

# DATABASE INFORMATION

- ns_21479_8
- Procedure format: TP_QX
