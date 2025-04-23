## Overview

We aim to build a multi-modal hybrid recommender system that recommends restaurants on Google Map to users by leveraging collaborative signals, review sentiment, metadata, and visual content. Our project goes beyond simple collaborative filtering by integrating multiple modalities and applying explainable and advanced techniques.

## Dataset 

We choose a subset of the Google Restaurants dataset (Google Restaurants), a multi-modal dataset derived from Google Maps. This dataset contains restaurant-related information, including user-posted images, reviews, and additional metadata. For our study, we will utilize a subset comprising 30K restaurants, 37K users, 108K reviews, and 203K images. The available metadata includes business_id, user_id, rating, review_text, and images. By leveraging the business_id and user_id, we can map ratings to users, facilitating rating prediction.


## Project Structure
```plaintext
Question_Answering_LM/
│
│
├── src/                  		 # Source code Folder
│   ├── Image_Review_DataSet.ipynb       # Explore the Dataset
│   ├── Matrix_Factorization_SVD.ipynb   # Matrix Factorization Collaborative Filtering
│   ├── N_MF_CF.ipynb        		 # Neural Matrix Factorization Collaborative Filtering
│   ├── User_Item_CF.ipynb        	 # User Item based Collaborative Filtering
│   └── xxx.ipynb         		 # Code
│
└── README.md              		 # Project documentation and instructions

```

## Requirements
- Python 3.7+
- PyTorch
- Tensorflow
- Jupyter Notebook 	

## Next Steps
- **Feature Engineering:** 
- **Model Tuning:** 
- **Evaluation:** 
- **Model Deploy:** 
- **Data Expansion:** 
- **UI Building**

## Contributing
Contributions are welcome! Please fork the repository and create a pull request to contribute to the project.

## License
This project is licensed under the MIT License.
