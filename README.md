# TweetAnalysisForBloodDonation
A Spark Streaming example to receive twitter data and to identify the urgent blood or plasma requirements

The objective of the project is to identify and collect data from twitter feeds which are related to urgent blood or plasma requirements, analyse the tweet to determine the date, user ID, location and the hashtags used for such requirement.

The project uses scala and spark. Twitter provides a streaming API to stream real time twitter data. This project uses a library named Twitter4j to access Streaming API and download twitter data. There are two sets of filter that gets applied to the incoming twitter data. First set of filter looks for tweets containing "blood","plasma", "#blood", "#bloodrequired","#BloodMatters","#BloodDrive","#DonateBlood","#Blood","#NeedBlood

The second set of filter acts to filtered tweets to look for words like urgent, need, emergency, and required. This is for filtering only those messages where there is a urgent need for blood or plasma. This acts as an effective filter to filter general blood donation related messages like "i donated blood today", "organizing a blood donation drive" etc.

Later, we extract the hashtags used for twitter status related to urgent blood donation requirements.

A complete explanation of my code can be found at my medium page here : <link to be added>
