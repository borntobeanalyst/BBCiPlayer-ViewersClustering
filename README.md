# BBC-ViewersClustering
Figuring out the types of viewers for BBC iPlayer comparing different clustering methods.

Using BBC iPlayer's customer behaviour data, firstly, I cleaned the dataset eliminating the points that seem not to be useful or meaningful for the 
analysis and divided viewrs into different clusters by choosing one of the clustering methods (e.g., K-means, PAM, H-clustering) which fits the best with 
the given dataset. Chose number of clusters evaluating the results with silhouette analysis, PCA (principal component analysis), elbow chart. 
Finally, evaluated the result of clustering by conducting subsample analysis. 

## Variable Description

The column descriptions are as follows.

a)	user_id  -- a unique identifier for the viewer

b)	program_id and series_id -- these identify the program and the series that the program belongs to

c)	genre -- the programme’s genre (e.g., drama, factual, news, sport, comedy, etc)

d)	start_date_time -- the streaming start date/time of the event

e)	Streaming id -- a unique identifier per streaming event

f)	prog_duration_min -- the program duration in minutes

g)	time_viewed_min -- how long the customer watched the program in minutes

h)  duration_more_30s - equals 1 if the program duration is more than 30 seconds, equals 0 otherwise 

i)  time_viewed_more_5s - equals 1 if time_viewed is more than 5 seconds, equals 0 otherwise

j)  percentage_program_viewed -- percentage of the program viewed

k) watched_more_60_percent -- equals 1 if more than 60% of the program is watched, equals 0 otherwise

l) month, day, hour, weekend -- timing of the viewing

m) time_of_day -- equals “Night” if the viewing occurs between 22 and 6AM, "Day" if it occurs between 6AM and 14, “Afternoon” if the it occurs between 14 and 17, “Evening” otherwise

