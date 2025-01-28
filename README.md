# Clickbait Detection on YouTube Videos  

### Problem  
Clickbait is everywhere, and it’s frustrating when a video doesn’t match what was promised. The goal was to figure out if a video is clickbait or not. Tried different approaches, from simple models to advanced AI, to see what works best.  

### What Was Done  
1. **Collected Data**  
   Used the YouTube Data API to gather video details like titles, descriptions, tags, likes, views, comments, and thumbnails. Cleaned the data and added extra features like engagement rate and comment density to make it more useful for analysis.  

2. **Testing Traditional Models**  
   Applied simple methods like sentiment analysis on comments (using VADER and TextBlob). Combined these insights with other features to train models like Random Forest and Gradient Boosting.  

   Results showed that these models do a great job, with over 95% accuracy in spotting clickbait when text-based features are available.  

3. **When LLMs Are Useful**  
   Advanced AI like LLMs were brought in to analyze thumbnails or when comments were disabled. They helped in cases where traditional models lacked context.  

### Results  
- Simple models are enough to detect clickbait in most cases.  
- LLMs become important when analyzing thumbnails or handling videos with no comments.  

### Extras  
The project includes visualizations like confusion matrices, sentiment graphs, and ROC curves to show how the models performed.  
