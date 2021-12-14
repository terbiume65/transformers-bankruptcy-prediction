# Bankruptcy Prediction from text segments of annual reports using Transfer Learning with Transformer Models
Extended Essay, Toby Chung, December 2021
### Abstract
Predicting corporate bankruptcy and default risk is an issue that concerns the interests of investors, financial institutions, and governments. For the purpose of due diligence, it is essential to assess a firm's financial stability and credibility before an investment decision is finalized. Models have been traditionally developed mathematically or statistically to forecast the probability of bankruptcy, using only numerical variables in a firm's accounting documents. However, the emerging focus on sequence models in deep learning has brought new research and approaches to developing predictive models with textual data. With recent advancements in transformer models in the field of natural language processing, this study follows previous research of textual models by investigating the effectiveness of transfer learning using new transformer models and providing the first evidence for their predictive power in the application of binary classification on sequences and bankruptcy prediction. Despite using only a small sample size of training data and very little computational resource, the empirical results showed comparable performance and even improvements over the models of previous large-sample studies, demonstrating the new possibilities where machine intelligence systems could perform language-related human tasks.
### Content
You could find the full training history of most model versions in the "RESULTS" directory. There may not be history for models that fail to converge.

You could find the complete source code of the project in the "CODE" directory. The code comes in three parts, in the form of Jupyter Notebooks. 

The first part is "extraction.ipynb". It reads "sf_hdr.txt" to find a list of bankrupt and healthy companies. It then uses web scraping to download 10-K reports of companies on the list from SEC's EDGAR database. The downloaded forms from the bankrupt list and healthy list would be stored in two local directories.

The second part is "dataset.ipynb". It reads the downloaded forms from the local directories for cleaning and truncating to construct a clean .csv dataset file.

The third part is "model.ipynb". This is the part where we use the .csv dataset to actually compile and train the models. 
