
# Graph-Autoencoder-Drug-Recommender-GADR
 
GARD (Graph Autoencoder Recommender for Drugs) is a medication recommendation model based on graph autoencoders. This project utilizes dimensionality reduction and graph representation learning techniques to predict drug response. By incorporating clinical data and information on drug interactions, GARD aims to provide personalized recommendations for patients in healthcare settings.

For further inquiries, please contact Mongi Kourchid at: mongi.kourchid@gmail.com.

Ce référentiel fournit l'implémentation officielle de PyTorch du document suivant :
![image](https://github.com/user-attachments/assets/31f5badd-acee-4777-8936-3eb8df591cb4)
### Features and Benefits
- **Graph Autoencoder (GCN AE)**: Leverages advanced graph neural networks to create high-quality embeddings, enhancing the model's ability to capture complex relationships within clinical and drug interaction data.
- **Accurate Drug Response Prediction**: Uses learned embeddings to provide precise predictions for drug response, enabling more effective patient care and minimizing the risk of adverse reactions.
- **Advanced Medication Recommendation System**: Employs convolutional neural networks and deep learning methods to generate personalized drug recommendations, tailored to individual patient profiles and health conditions.
## Installation
To set up and run GARD, follow these steps:

#### 1  Clone the Repository:
git clone https://github.com/mongikourchid/Graph-Autoencoder-Drug-Recommender-GADR.git
cd Graph-Autoencoder-Drug-Recommender-GADR
#### 2 Create and Activate a Virtual Environment (Recommended):

#### .For macOS/Linux:
python3 -m venv venv
source venv/bin/activate
#### . For Windows:
python -m venv venv
venv\Scripts\activate
 #### 3 Install Dependencies: Ensure Python 3.7 or higher is installed. Then install the required packages from the requirements.txt file:
 pip install -r requirements.txt
####  4 Run the Main Script: Once the dependencies are installed, execute the main script:
python main.py
 ####  5 Run Tests (Optional): To check that everything is working correctly, you can run the test suite:
 python -m unittest discover tests/
 # Input Data
The GARD model requires specific input data to train and make predictions for drug recommendations. Below is a description of the expected data formats and the steps to prepare them.
### 1. Graph Data Format:
GARD uses graph-based data, where each drug is represented as a node, and interactions between drugs are represented as edges. The input data must be in a graph format.

 ### Node Features:
 Each drug is represented by a feature vector. These features could include molecular descriptors, drug-target interactions, or any other relevant chemical or biological features.
 ### Edge Features:
 The relationships between drugs are represented as edges, where the edge features can include interactions like binding affinity, chemical similarity, or other types of drug-drug relationships.
 ### Graph Construction:
 A graph construction method needs to be defined, such as creating a drug interaction graph or a molecular similarity graph.
###  2. Data Format:
The model expects input in the form of:

 ### Drug feature matrix (e.g., a CSV or numpy array of shape (num_drugs, num_features)).
 ###  Graph adjacency matrix (e.g., a sparse matrix or a dictionary representing edges between drugs).
