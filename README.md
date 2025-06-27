## Overview

We aim to build a multi-modal hybrid recommender system that recommends restaurants on Google Map to users by leveraging collaborative signals, review sentiment, metadata, and visual content. Our project goes beyond simple collaborative filtering by integrating multiple modalities and applying explainable and advanced techniques.

## Dataset 

We choose a subset of the Google Restaurants dataset (Google Restaurants), a multi-modal dataset derived from Google Maps. This dataset contains restaurant-related information, including user-posted images, reviews, and additional metadata. For our study, we will utilize a subset comprising 30K restaurants, 37K users, 108K reviews, and 203K images. The available metadata includes business_id, user_id, rating, review_text, and images. By leveraging the business_id and user_id, we can map ratings to users, facilitating rating prediction.

The dataset is from [Google Restaurants](https://cseweb.ucsd.edu/~jmcauley/datasets.html#google_restaurants). You can download it directly from [here](https://mcauleylab.ucsd.edu/public_datasets/gdrive/googlelocal_restaurants/), or download the required files using the commands below:  
### For macOS / Linux:
```bash
wget https://mcauleylab.ucsd.edu/public_datasets/gdrive/googlelocal_restaurants/filter_all_t.json
wget https://mcauleylab.ucsd.edu/public_datasets/gdrive/googlelocal_restaurants/image_review_all.json
```

### For Windows (Command Prompt):
```cmd
curl -O https://mcauleylab.ucsd.edu/public_datasets/gdrive/googlelocal_restaurants/filter_all_t.json
curl -O https://mcauleylab.ucsd.edu/public_datasets/gdrive/googlelocal_restaurants/image_review_all.json
```

## Project Structure
```plaintext
New_Tasty/
│
│
├── src/                  		 		# Source code Folder
│   ├── Image_Review_DataSet.ipynb       		# Explore the Dataset
│   ├── Matrix_Factorization_SVD.ipynb   		# Matrix Factorization Collaborative Filtering
│   ├── N_MF_CF.ipynb        		 		# Neural Matrix Factorization Collaborative Filtering
│   ├── User_Item_CF.ipynb        	 		# User Item based Collaborative Filtering
│   ├── UI.ipynb        	 	 		# UI for demo
│   ├── N_MF_CF_wTextData.ipynb         	 	# Neural Matrix Factorization Collaborative Filtering with Metadata
│   └── evaluation/         				# Evaluation code Folder
│	├── N_Fold_Matrix_Factorization_SVD.ipynb       # N fold cross validation for matrix factoraztion
│ 	├── N_Fold_N_MF_CF_Evaluation.ipynb   		# N fold cross validation for neural matrix factorization
│ 	├── N_Fold_plot.ipynb   			# Plot results for N fold cross validation 
│   	└── N_Fold_User_Item_CF.ipynb      		# N fold cross validation for User/Item CF
│
└── README.md              		 		# Project documentation and instructions


```

## Contributing
Contributions are welcome! Please fork the repository and create a pull request to contribute to the project.

## License
This project is licensed under the MIT License.
