# What Makes a Spotify Song Popular? Exploring the Audio Features Behind Today's Hits
### by Aarushi Khurana

Spotify provides more than just a popularity score for each song -- it also measures a variety of audio characteristics, including danceability, energy, acousticness, and valence. This project explores whether those features are associated with a song's popularity. Through a data exploration of a public Spotify dataset, thousands of tracks were analzyed and compared across different popularity levels and characteristics, examined whether explicit songs tend to receive higher popularity scored, and identified patterns that may help explain why some songs perform better than others. While there were some notable trends in the analyses, it also demonstrates that no single musical characteristic fully explains a song's success

## Dataset

The dataset used for this exploration is the [Spotify Tracks Dataset](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset?resource=download), which was downloaded from Kaggle. The data includes thousands of songs available on Spotify along with their popularity scores and audio features such as danceability, energy, acousticness, valence, tempo, and whether the song is marked as explicit. These audio features are generated using Spotify's audio analysis system, while popularity scors are calculated by Spotify based on streaming activity and other engagement metrics. 

Although Kaggle provides public access to the dataset, it is not the original creator of the data. The underlying information comes from Spotify and reflects the company's own methods for measuring song characteristics and popularity. Because Spotify does not publicly disclose the exact formula used to calculate popularity scores, the results should be interpreted carefully. Additionally, the datasset may not include every song available on Spotify and represents only a snapshot in time. As songs continue to gain streams, popularity scores may change. 

Overall, the dataset is appropriate for exploring relationships between measurable audio characteristics and popularity, but it cannot explain why listeners choose particular songs or determine whether one feature directly causes greater popularity. 

## Data Analysis

The dataset was imported into [Google Sheets](https://docs.google.com/spreadsheets/d/1bPYk069YWhUJBg1NYFa3p1RzconGpvCPPs24vBMgU5k/edit?usp=sharing) for analysis and no major data cleaning was required because the dataset already contained standarzied numerical values for Spotify's audio features. I first calculated summary statistics, including the average, minimum, and maximum popularity scores, along with average values for danceability, energy, valence, and acousticness, to better understand the overall characteristics of the dataset. 

Next, I created a new **Popularity Category** variable by grouping songs into three categories based on their popularity scores: **Low (0-33), Medium (34-66), and High (67-100)**. Using pivot tables, I compared average audio features across these popularity groups. Additional pivot tables were used to compare average popularity by genre and whether a song was marked as explicit.

The analysis found that most audio features remained relatively consistent across popularity categories. However, highly popular songs generally had higher average danceability and lower average acousticness than less popular songs. Songs marked as explicit also had a slightly higher average popularity than non-explicit songs, although the difference was modest. These findings suggest that while some measurable characteristics are associated with popularity, no single audio feature appears to determine whether a song becomes successful. 

## Average Audio Features by Song Popularity

image 

description

## Methods and Limitations

This analysis was conducted using Google Sheets. Pivot tables were used to summarize average values across catefories, and bar charts were created to visualize the findings. Because the porject relies on more descriptive statistics, it identifies associations rather than causal relationships. 

Several limitations should be considered. First, Spotify does not publicly disclose the complete methodology behind its popularity score, making it difficult to determine exactly what contributes to a song's ranking. Secon, the dataset represents a single snapshot of Spotify songs rather than continuously updated streaming data. Finally more important factors that influence popularity, such as artist reputation, playlist placement, marketing, release timing and social media trends, are not included in the dataset. As a result, this project cannot determine why a song becomes popular; it can only identify patterns among the available variables. 

## Conclusion and Ethical Considerations

This project explored whether Spotify's measurable audio features are associated with song popularity. While highly popular songs tended to be more danceable and less acoustic, most other audio characteristics differed only slightly across popularity levels. The most popular genre by far also demonstrated was the pop-film genre in music out of 115 genres listed.  Explicit songs also showed a modest increase in average popularity, although the difference is relatively small. 

These findings suggest that musical characteristics alone cannot fully explain a song's success. Popularity is likely influenced by a combination of audio features, artist recognition, promotion, listener behavior, and broader cultural and geographic trends. 

From an ethical perspective, it is important not to interpret these results as a formula for creating successful music or evidence that certain genres or artistic styles are inherently better than others. The dataset reflects Spotify's platform and ranking system rather than universal musical quality or lsitener preferences. Additional reporting, including interviews with artists, producers, and music industry professionals, would provide valuable context that numerical data alone cannot capture. 

## Sources
