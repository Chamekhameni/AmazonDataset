# Context
This dataset is part of a thesis conducted at the MIRACL research laboratory, focusing on sentiment analysis within the agricultural sector. Our dataset addresses the gap of datasets in this field.  We offer a method for constructing such datasets by collecting reviews  related to pesticide products from Amazon.

# How was it collected?
- This collection aligns with our paper titled " An agricultural sentiment dataset for pest control and crop diseases"
- The corpus is automatically extracted, based on a list of keywords from the AGROVOC thesaurus, and using a web extension developed with Python using BeautifulSoup and Selectorlib libraries to navigate web pages and extract necessary information.
- The data spans from June 17, 2009, to February 17, 2024.

# Content of "Amazon_Dataset"
- The data gathered is a CSV of 10,181 reviews on anti-parasitic products from Amazon.
- The reviews are categorized by pest and disease types: "Insects: 3824 reviews", "Fungi: 2421 reviews", "Herbs: 3296 reviews", "Bacteria: 133 reviews", "Nematodes: 178 reviews", and "Viruses: 323 reviews".
- The Amazon dataset is represented by the following columns: "class_id", "treatment_type", "product_id", "review_author_name", "review_date", "review_content", "review_rating", and "review_is_verified".
  
# Annotation  
- Based on the "review_rating" column, which represents ratings in stars, each star rating was converted into a specific sentiment (e.g., "5 étoiles" to "very positive").
- The annotation schema categorized the number of star ratings into sentiments as follows: ( 1 = "very negative", 2 = "negative", 3 = "neutral", 4 = "positive", and 5 = "very positive". )
- The annotated dataset includes 6574 reviews with "very positive" sentiments, 1647 reviews with "positive" sentiments, 779 reviews with "very negative" sentiments, 386 reviews with "negative" sentiments, and 795 reviews with "neutral" sentiments.
