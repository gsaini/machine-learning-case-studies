# Anime Rating Case Study

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![mlflow](https://img.shields.io/badge/mlflow-%23d9ead3.svg?style=for-the-badge&logo=numpy&logoColor=blue)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)

## 📖 Problem Statement

### Background
Streamist is a global streaming platform that offers a wide variety of web series and movies to its users. Each piece of content is rated by viewers, and additional information such as the number of viewers, number of episodes, episode duration, and more is collected for each title. Recently, Streamist has decided to focus on the anime category to better understand what drives user ratings and to improve content recommendations and acquisition strategies.

### Business Problem
Streamist wants to identify the most significant factors that influence the ratings of anime titles on their platform. By understanding these factors, Streamist aims to:
- Enhance user engagement by recommending highly-rated anime based on user preferences
- Inform content acquisition and production decisions
- Improve the overall user experience by highlighting key features that matter most to viewers

### Data Science Problem
As a data scientist at Streamist, your task is to:
1. Analyze the provided anime dataset to uncover the key factors that impact anime ratings
2. Build a predictive model (using linear regression) to estimate the rating of an anime based on its features
3. Evaluate the model's performance and interpret the results to provide actionable insights for the business

### Key Questions
- What are the most important features that influence the rating of an anime?
- How accurately can we predict the rating of an anime using the available data?
- What recommendations can be made to Streamist based on the analysis and model findings?

### Deliverables
- 📊 Exploratory Data Analysis (EDA) highlighting trends, patterns, and relationships in the data
- 🤖 A linear regression model to predict anime ratings, along with an assessment of its performance
- 💡 Insights and recommendations for Streamist based on the analysis and modeling results

---

## 🗂️ Data Information
Each record in the dataset provides a description of an anime. Below is the data dictionary:

| Column                        | Description                                                      |
|-------------------------------|------------------------------------------------------------------|
| `title`                       | The title of the anime                                           |
| `description`                 | The synopsis of the plot                                         |
| `mediaType`                   | Format of publication                                            |
| `eps`                         | Number of episodes (movies are considered 1 episode)             |
| `duration`                    | Duration of an episode in minutes                                |
| `ongoing`                     | Whether it is ongoing                                            |
| `sznOfRelease`                | The season of release (Winter, Spring, Fall)                     |
| `years_running`               | Number of years the anime ran/is running                         |
| `studio_primary`              | Primary studio of production                                     |
| `studios_colab`               | Whether there was a collaboration between studios                |
| `contentWarn`                 | Whether anime has a content warning                              |
| `watched`                     | Number of users that completed it                                |
| `watching`                    | Number of users that are watching it                             |
| `wantWatch`                   | Number of users that want to watch it                            |
| `dropped`                     | Number of users that dropped it before completion                |
| `rating`                      | Average user rating                                              |
| `votes`                       | Number of votes that contribute to rating                        |
| `tag_Based_on_a_Manga`        | Whether the anime is based on a manga                            |
| `tag_Comedy`                  | Whether the anime is of Comedy genre                             |
| `tag_Action`                  | Whether the anime is of Action genre                             |
| `tag_Fantasy`                 | Whether the anime is of Fantasy genre                            |
| `tag_Sci_Fi`                  | Whether the anime is of Sci-Fi genre                             |
| `tag_Shounen`                 | Whether the anime has a tag Shounen                              |
| `tag_Original_Work`           | Whether the anime is an original work                            |
| `tag_Non_Human_Protagonists`  | Whether the anime has any non-human protagonists                 |
| `tag_Drama`                   | Whether the anime is of Drama genre                              |
| `tag_Adventure`               | Whether the anime is of Adventure genre                          |
| `tag_Family_Friendly`         | Whether the anime is family-friendly                             |
| `tag_Short_Episodes`          | Whether the anime has short episodes                             |
| `tag_School_Life`             | Whether the anime is regarding school life                       |
| `tag_Romance`                 | Whether the anime is of Romance genre                            |
| `tag_Shorts`                  | Whether the anime has a tag Shorts                               |
| `tag_Slice_of_Life`           | Whether the anime has a tag Slice of Life                        |
| `tag_Seinen`                  | Whether the anime has a tag Seinen                               |
| `tag_Supernatural`            | Whether the anime has a tag Supernatural                         |
| `tag_Magic`                   | Whether the anime has a tag Magic                                |
| `tag_Animal_Protagonists`     | Whether the anime has animal protagonists                        |
| `tag_Ecchi`                   | Whether the anime has a tag Ecchi                                |
| `tag_Mecha`                   | Whether the anime has a tag Mecha                                |
| `tag_Based_on_a_Light_Novel`  | Whether the anime is based on a light novel                      |
| `tag_CG_Animation`            | Whether the anime has a tag CG Animation                         |
| `tag_Superpowers`             | Whether the anime has a tag Superpowers                          |
| `tag_Others`                  | Whether the anime has other tags                                 |
| `tag_is_missing`              | Whether tag is missing or not                                    |

---

## 🎯 Learning Outcomes
- Exploratory Data Analysis
- Preparing the data to train a model
- Training a regression model
- Model evaluation
- Forward Feature Selection

---
