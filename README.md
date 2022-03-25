# ml-project-2-fmz


# Project description:
The aim of this project was to define a pipeline using machine learning methods in order to identify whether a job
advertisement is green or not. The used database contains one million job vacancies published in Switzerland. Jobs ads are
divided in title and content, can be written in different languages and are non labeled. The first step of the proposed pipeline
is a data preprocessing composed of a language splitting, a cleaning on the entire databse and a tokenization of english
data. Then, considering the english data only, we divided it into train and validation subsets for both titles and contents
separately and into a test subset containing both. A manual or fast labeling process is applied based on the United Nations
Sustainable Development Goals. Finally Ridge logistic regression, Convolutional neural networks (CNN) and Bidirectional
Encoder Representations from Transformer (BERT) were implemented. The best result are obtained using Ridge logistic
regression.

Our final pipeline:
![alt text](https://github.com/CS-433/ml-project-2-fmz/blob/main/pipeline2.png)
# Organisation of repository:
Please note that we ran our code on Colab to have access to free GPU. To reproduce the same code, some change of directories may be needed. We also suggest using GPU in order to the running time shorter.

**Also note that we have signed an NDA stating that the data used is confidential. As a result, our repository does not contain any database. Our notebooks however contain some printings (still at most two lines per cell, as agreed with our hosting lab). If you want to have access to more details, please contact directly gaetan.derassenfosse@epfl.ch from the IIPP lab.**

 * [Code](https://github.com/CS-433/ml-project-2-fmz/tree/main/Code)
   * [Cleaning and Labeling](https://github.com/CS-433/ml-project-2-fmz/tree/main/Code/Cleaning%20and%20Labeling): folder that contains the notebook we used to to clean and fast label our data.
   * [Ridgdelogreg](https://github.com/CS-433/ml-project-2-fmz/tree/main/Code/RidgeLogReg): code to implement Ridge logistic regression for our classification of both the title and the content. 
   * [BERT](https://github.com/CS-433/ml-project-2-fmz/tree/main/Code/BERT): code to implement BERT for our classification of both the title and the content. 
   * [CNN](https://github.com/CS-433/ml-project-2-fmz/tree/main/Code/CNN): code to implement CNN for our classification of both the title and the content. 
   * [Final Binary](https://github.com/CS-433/ml-project-2-fmz/tree/main/Code/FINAL%20BINARY): code to join the results of the classification of both title and content to a single binary classification. 
 * [Datasets](./dir1)
   * [Labeling](https://github.com/CS-433/ml-project-2-fmz/tree/main/Datasets/labeling): contains the list of words we based our fast labeling on. 
 * [README.md](./README.md)
