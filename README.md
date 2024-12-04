# Project: Non-Negative Matrix Factorization (NMF) vs. BERTopic for Topic Modeling
### Course: DSC 210: Numerical Linear Algebra for Data Science
### Instructor: Dr. Tsui-wei Weng

#### Instructions:
Note: BERTopic's visualizations required the model to be created during the run because saving to a pickle file removed the functionality. Training BERTopic within the notebook will take around 20 minutes (if ran on google colab). More details [here](https://github.com/MaartenGr/BERTopic/issues/1792#issuecomment-1939288767).

* Ensure that the following libraries are installed in python 3.10 environment:
  - pandas
  - numpy
  - seaborn
  - matplotlib
  - nltk
  - collections
  - scikit-learn
  - gensim
  - tqdm
  - plotly
  - wordcloud
  - octis
  - sentence_transformers
  - umap
  - hdbscan
  - bertopic

* Open NMF_vs_BERTopic.ipynb and run all the cells of the notebook.

#### Results:

* **NMF**

Top 10 words for each of the topics:

<img width="679" alt="Screenshot 2024-12-03 at 10 49 52 AM" src="https://github.com/user-attachments/assets/ebe0a336-046b-4152-8c32-ee4057e2a2aa">

Distributions of topics across all documents:
<img width="768" alt="Screenshot 2024-12-03 at 10 50 34 AM" src="https://github.com/user-attachments/assets/fd2c94c4-e20d-449c-bec8-8b2e0c938e55">

Visualized embedding of documents in 2-D space:
<img width="1026" alt="Screenshot 2024-12-03 at 10 51 21 AM" src="https://github.com/user-attachments/assets/6803b064-4fea-45b7-b5a0-97b108e60140">

Visualized distribution of documents per topic based on newsgroup:
You can view the interactive plot [here](./interactive_plot_nmf.html).

Topic Diversity: **0.98**

Residual Score: **0.94**

Coherence Score: **0.46**

* **BERTopic**

Top 6 words for each of the topics:

<img width="701" alt="Screenshot 2024-12-03 at 10 53 39 AM" src="https://github.com/user-attachments/assets/3a24c6e6-8f36-462f-8a79-b41556099e91">

Distributions of topics across all documents:
<img width="883" alt="Screenshot 2024-12-03 at 11 50 16 AM" src="https://github.com/user-attachments/assets/b4580e9f-8478-4934-a5dd-081270fcfb86">

Visualized embedding of documents in 2-D space:
<img width="888" alt="Screenshot 2024-12-03 at 11 32 31 AM" src="https://github.com/user-attachments/assets/e52fb1d4-07bc-4433-b1f4-7373b4e61462">

Topic Diversity: **0.99**

Topic Coherence: **0.51**

* **Metric Comparison**

<img width="301" alt="Screenshot 2024-12-03 at 11 46 31 AM" src="https://github.com/user-attachments/assets/ad30649b-90ed-4896-adb2-e2db1a2de58e">

