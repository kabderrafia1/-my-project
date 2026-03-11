# Smart Cabin Advisor

Final project for the Building AI course

## Summary
Smart Cabin Advisor is an AI tool that predicts cabin rental prices based on size, location, amenities, and reviews. It helps cabin owners and renters make data-driven decisions.  
*Building AI course project*

---

## Background
The project aims to solve these problems:  
* Cabin owners often under- or overprice their cabins due to lack of market insight.  
* Renters cannot easily compare cabins based on both price and qualitative reviews.  
* Manual analysis of cabin features and location is time-consuming.  

**Motivation:** I am interested in using AI to make real estate and rental markets more transparent and fair. Predicting prices accurately benefits both owners and renters, while leveraging natural language from reviews adds depth beyond numerical features.

---

## How is it used?
* Users (cabin owners or renters) input features of a cabin:  
  * Size, number of bathrooms, sauna size, distance to lake, proximity to neighbors.  
  * Text reviews of the cabin (optional).  
* The AI predicts a suggested rental price and highlights features that increase or decrease value.  
* Renters can query “similar cabins in this price range” and get AI-sorted recommendations.  

**Example usage:**  
```python
# Sample input
cabin_features = {
    "size_m2": 120,
    "sauna_m2": 15,
    "distance_to_lake_m": 50,
    "indoor_bathrooms": 2,
    "reviews": [
        "beautiful lake-side view", 
        "quiet and relaxing"
    ]
}

# AI output
predicted_price = 415000
top_factors = ["size", "bathrooms", "lake distance"]

print(f"Predicted price: €{predicted_price}")
print(f"Top 3 factors influencing price: {top_factors}")
