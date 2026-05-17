# CS215-Portfolio-HilliardJ

### Project Ideas
Project Idea 1:
Google Search History Data 
- How do my google searches change over time?
- What topics seem to occur the most?

Project Idea 2:
Hapo Bank Data
- How does my income and spending change over time, and how does that relate to my seasonal work schedules as a resturant server?
- How has my spending behaviors evolved over time?

Project Idea 3:
Apple Music Replay Data
- Can I cluster my listening data into moods?
- Are there any changes in my music taste over time?

### Week 10 Update
- For my final project, I will be working alone.
- My general topic is analyzing Apple Music Replay data.
- I will be using my own personal data as the source. I listen to a good amount of music, so I am confident I will have enough data for this project. I am worried about being able to collect this data because the previous time I attempted, I failed and received the wrong information.
- I am hoping to explore how my music taste has cahnged thorughout the years, what genres tend to pop up most and if it changes, and if my listening data be grouped into any moods?

### Week 11 Update
- I have decided to analyze my own personal Apple Music Replay data for this project.
- I obtained my data by going to Apple’s Data and Privacy website and submitting a request to have my data sent to me. It took a few days to receive, but the process was fairly easy.
- The data came in multiple zipped files with a large amount of information. I still need to go through each file to understand what data is available and what kinds of analysis I can perform. From the few files I have already explored, the data appears to be fairly clean and well-organized.
- One challenge I anticipate is navigating through the layers of zipped files and figuring out what each file represents, but I am excited to work through this and begin developing meaningful analysis questions.

### Week 12 Update
<iframe 
  src="favorite_vs_nonfavorite_plot.html" 
  width="100%" 
  height="600" 
  style="border:none;">
</iframe>
Narration of Visualiztion: According to the interactive bar graph, comparing all the songs I've listened to, songs I marked as favorite have, on average, higher play counts and higher play duration (in minutes) than songs not marked as favorite. Favorited songs also have a slightly smaller average skip count. This suggests that favorited songs are played more often and listened to for a fuller amount of time. I found it interesting that the average skip count was pretty similar which suggests I skip my favorited songs about the same time as I skip non-favorited songs. The interactive bar graph is designed so one can hover over to see exact values. 

### Week 14 Update
- My project is now complete, I just need to update comments and narration throughout my Google coLab.
- For my new technique, I am using cumulative growth analysis visualized with a Plotly Scatterplot. I am learning it with the assistance of ChatGPT.
- My communication strategy will be a Google Slides presentation and screenshots of my graphs. I might also link my GitHub website so I can showcase the interactive aspect of my graphs. 

# Final Project
### Introduction & Summary
For my project, I chose to analyze my own **Apple Music Replay data**. I decided on this data source because I knew it contained a large amount of information and personally interested me due to my love of music. The data was collected directly from Apple’s Data & Privacy portal and includes information such as song names, artists, timestamps, favorites, rankings, and play activity across many years of my listening history. I cleaned and transformed multiple datasets, merged information across files, and created visualizations to better understand patterns in my listening behavior. I wanted to explore how my music taste has changed over time, how favorited songs compare to non-favorited songs, and which songs quickly dominated my listening history after I first discovered them. In addition to techniques learned throughout the course, I also implemented a new technique called cumulative growth analysis in order to assess how quickly listening activity accumulated for certain songs relative to others over time.

To begin this project, I requested my Apple Music Replay and listening history data directly from Apple’s Data & Privacy portal. After downloading the files, I explored a multitude of Apple iTunes CSV and JSON files, and identified information related to listening history, favorites, play duration, rankings, and timestamps. I used Python and pandas in Google Colab to clean and transform the datasets. This included converting dates into datetime format, calculating play duration hours from milliseconds, grouping and aggregating data, and merging information across multiple files. I then used Plotly to create interactive visualizations to better understand long-term trends, listening behaviors, and song growth patterns within my listening history.

### Main Insights & Visualizations

One of the most useful visualization techniques I implemented throughout this project was the use of Plotly visualizations. The interactive features were so fun to explore in greater detail because I was able to hover over points and view exact values directly within the graphs. I loved the Plotly scatterplots and being able to see each song from my ten years of listening data. I also found that the interactivity made the visualizations more engaging and effective for communicating trends.

The most interesting insight for me was that **“Black Star” by Radiohead** had the highest listening growth rate after first listen, meaning it rapidly became a major part of my listening behavior shortly after I first heard it. This did not surprise me as I love "Black Star". Another surprising finding was that **I listened to over 173 hours of music during the month of November 2021 alone**. Overall, the project revealed that my listening behavior changes dramatically over time and that certain songs can quickly become dominant parts of my listening history. I had a lot of fun creating this project, and in this class in general!

<iframe 
  src="monthly_listening_plot.html" 
  width="100%" 
  height="600" 
  style="border:none;">
</iframe>

Narration of Visualization: The line plot shows my monthly listening activity across the last 10 years. While some periods show relatively steady listening behavior, other periods contain large spikes in total listening hours. I believe these spikes may be due to changes in routines, school workload, or periods where music played a larger role in my daily life. Overall, the line plot suggests that my listening behavior is not constant over time and instead changes substantially across different periods of my life.

<iframe 
  src="favorite_vs_nonfavorite_plot.html" 
  width="100%" 
  height="600" 
  style="border:none;">
</iframe>

Narration of Visualization: According to the interactive bar graph, comparing all the songs I've listened to, songs I marked as favorite have, on average, higher play counts and higher play duration (in minutes) than songs not marked as favorite. Favorited songs also have a slightly smaller average skip count. This suggests that favorited songs are played more often and listened to for a fuller amount of time. I found it interesting that the average skip count was pretty similar which suggests I skip my favorited songs about the same time as I skip non-favorited songs. The interactive bar graph is designed so one can hover over to see exact values. 

<iframe 
  src="growth_plot.html" 
  width="100%" 
  height="600"
  style="border:none;">
</iframe>

Narration of Visualization: The bubble chart displays each song in my listening history and how many total hours I spent listening to each song. The songs with the largest listening growths are represented by the larger yellow bubbles. The number of days since I first discovered each song are on the x-axis, while total listening hours are on the y-axis. Most songs are near the bottom of the graph, indicating relatively low long-term listening accumulation. However, several songs stand out with both large listening totals and high listening growth rates, suggesting that they rapidly became major parts of my listening habits shortly after discovery. This visualization highlights how some songs gradually accumulate listening activity while others quickly dominate listening behavior.

One interesting pattern I noticed is that many of the smallest bubbles appear toward both the bottom and the left side of the graph, while many of the larger bubbles are associated with more recently discovered songs. I think this may suggest that over time I have developed a stronger understanding of my music taste and have become better at finding songs that I strongly connect with. As a result, more recently discovered songs may accumulate listening hours and listening growth more rapidly than songs I discovered in earlier years.

### Future Work

If I had more time or resources, I would be interested in expanding this project by comparing my personal top songs to the most popular songs during the same time periods in order to explore how closely my listening behavior aligns with popular music trends. I would also like to investigate how my listening habits change during stressful periods such as finals week or midterms. In addition, it would be interesting to continue updating this project with more recent listening data in order to observe how my music preferences and listening behaviors continue to evolve over time.
