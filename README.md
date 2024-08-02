# Map-Reduce-Algorithm-in-Spark-

Description of task 

This university project was an individual task where I needed to determine the distribution of the most shocking words in an ABC news article data set that consisted of 1048576 headlines.  The proposed method to approach the problem was undefined, so I decided to solve it using a MapReduce algorithm, considering the size of the data at hand. The shocking words in question were also undefined, so I selected the words based on my own personal opinion of shocking news headlines, characterising them into 2 categories: 'horrible shocking words' and 'funny shocking words'. Each step of the solution is annotated accordingly in the uploaded notebook. 


Detailed explanation of task solution

I first defined the shocking words across two categories: 

1) Most shocking words related to horrible/ violent/ upsetting crimes. 
2) Most shocking words related to funny instances - shocking in terms of being surprised to see this in a news headline.

My selection words from these categories  was based on my personal opinions as well as the content of previous news articles that I have read related to these subjects. My word selection is therefore as follows:

1) Horrible Shocking Words Selection:'kill','murder','attack','dead','death','accident','stabbed','stabbing','assault','assaulting','assaulted','killed','killing','manslaughter','fire','kidnap','kidnapping','kidnapped','torture','torturing','tortured','shot','shooting','exploded','explosion'. 

2) Funny Shocking words: 'bamboozled','bamboozle','bamboozled','clown','clowns','flabbergasted','monkey'. 

To determine the distribution of these word selections, I used a map reduce algorithm to count the occurrences of all the words in the entire data set, in the form of key value pairs and using RDD partitioning. After obtaining this RDD word count, I filtered out the respective words and demonstrated their distribution using histograms. As an added conclusion to the analysis, I filtered an rdd of the full headlines related to 'clown' and 'bamboozle' so that we can see what these headlines are and if they are in fact funny. 

