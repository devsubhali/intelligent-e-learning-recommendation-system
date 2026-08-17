# Intelligent E-Learning Recommendation System

## Overview

The Intelligent E-Learning Recommendation System is a content-based course recommendation system that suggests relevant online courses based on a user's learning interests.

The system analyzes information such as course descriptions, categories, and tags, and compares them with the user's input to recommend the most relevant courses.

## Objective

The main objective of this project is to help learners discover suitable e-learning courses without having to manually search through a large number of courses.

The system takes a user's learning interest as input and provides a list of the top five courses that are most relevant to that interest.

## How It Works

The recommendation process follows these steps:

1. The course dataset is loaded using Pandas.
2. Course descriptions, categories, and tags are combined into a single text representation.
3. TF-IDF (Term Frequency-Inverse Document Frequency) is used to convert the course text into numerical vectors.
4. The user's learning interest is converted into the same vector format.
5. Cosine similarity is calculated between the user's interest and the available courses.
6. Courses are ranked according to their similarity scores.
7. The system displays the top five recommended courses.

## Techniques Used

- Content-Based Recommendation
- TF-IDF Vectorization
- Cosine Similarity
- Natural Language Processing (NLP)

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn 
- Google Colab
- Jupyter Notebook

## Dataset

The project uses an online course recommendation dataset containing information about courses such as:

- Course ID
- Course description
- Category
- Tags

The dataset contains 300 course records.

## Example

### User Input

```text
Machine learning
```
### Example Recommendations

The system returns courses related to the entered learning interests and displays their similarity scores.

Example:

1. course_27
   Category: Business
   Tags: machine learning, design
   Similarity Score: 68.82%

2. course_35
   Category: Design
   Tags: machine learning, business
   Similarity Score: 68.82%

## Handling Irrelevant Queries

If the entered topic does not match any terms present in the available course data, the system informs the user that no relevant courses were found and suggests trying another topic.

For example:

Enter your learning interest: AI

Sorry, no relevant courses were found for that interest.
Try another topic such as Python, Design, Business, or Machine Learning.

## Project Files

Intelligent_E_Learning_Recommendation_System_Final.ipynb
online_course_recommendation.csv
README.md

## Future Scope

The current system is a basic content-based recommendation system. It can be further improved by:

- Adding course ratings and reviews
- Considering the learner's previous course history
- Adding user profiles and personalized learning preferences
- Using collaborative filtering
- Combining content-based and collaborative filtering
- Adding a web-based user interface
- Increasing the size and variety of the course dataset

## Project Status

This project was developed as an academic mini project to demonstrate the basic concepts of recommendation systems and machine learning using Python.

## References

- Scikit-learn documentation
- Pandas documentation
- NumPy documentation
