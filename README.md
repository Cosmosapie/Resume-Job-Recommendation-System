# Resume Job Recommendation System 

An automated system that recommends job roles based on resume content using Machine Learning (TF-IDF & KNN).

OverviewThis project solves the "Information Overload" problem in recruitment by automatically screening resumes.

It uses Content-Based Filtering to match candidate profiles with job descriptions based on keyword overlap and similarity. 

DatasetUsed the (https://www.kaggle.com/datasets/gauravduttakiit/resume-dataset) by Gaurav Dutta from Kaggle.Size: 962 ResumesCategories: 25 Job Roles (e.g., Data Science, Java Developer, HR, Testing)Format: CSV with Category and Resume text Tech StackLanguage: Python 3.xML Libraries: Scikit-Learn (TF-IDF, KNN, OneVsRestClassifier)Data Processing: Pandas, NumPyText Cleaning: Regex (re), NLTK MethodologyPreprocessing: Cleaned raw text by removing URLs, Twitter handles, hashtags, and special characters using Regex to prevent noise overfitting. 

1 Feature Extraction: Converted text into numerical vectors using TF-IDF (Term Frequency-Inverse Document Frequency) with a limit of 1500 features. 

2 Modeling: Used K-Nearest Neighbors (KNN) with Cosine Similarity to find the closest job category for a given resume. 

3 Installation & UsageClone the repository:Bashgit clone https://github.com/yourusername/resume-recommendation.git
cd resume-recommendation

## Install dependencies:Bashpip install pandas numpy scikit-learn nltk matplotlib

## Run the Notebook:Bashjupyter notebook Resume_Screening.ipynb

## Future ImprovementsDeep Learning: Integrate BERT/SBERT to capture semantic meaning (e.g., matching "ML" to "Machine Learning"). 
4 Scalability: Implement FAISS (Facebook AI Similarity Search) to handle millions of resumes efficiently. 5 LicenseThis project is open-source and available under the MIT License.
