# HealthCare_Patient_Rating

Data for this can be found at Google Drive Link: https://drive.google.com/open?id=0ByejGgzAgireOG1WNXo5OHBydTA

Business understanding
CMS rates hospitals in the US on a scale of 1-5 with the objective to make it easier for patients and consumers to compare the quality of hospitals.
 
The ratings directly influence the choice of hospital made by consumers and may have a significant impact on the revenue earned by hospitals. Thus, it is extremely important for hospitals to understand the methodology used by CMS for calculating the ratings so that they can work on improving the factors that influence them.
 
This project is focused on developing an approach to calculate hospital ratings and using it to identify areas of improvement for certain hospitals. It will also require a thorough understanding of the rating system developed by CMS.
 
The details of the CMS rating project is available at https://www.cms.gov/medicare/quality-initiatives-patient-assessment-instruments/hospitalqualityinits/hospitalcompare.html
 
In this project, you will approach the ‘CMS rating problem’ from different angles. You can think of it as ‘re-engineering the CMS rating system’.
 


 
Data understanding  
The data can be downloaded from the hospital compare website. You need to download 'Hospital_Revised_FlatFiles_20161110'. 
 
Modelling 
Part 1 - Supervised Learning-Based Rating
Think about the types of supervised models you will choose for predicting the star ratings (1-5, five-class classification). Consider all the practical as well as technical aspects involved. In the report, mention the types of models you will consider, the pros and cons of each, and the reasons for choosing certain models for this problem. Note that you have to build only one type of model (as mentioned in part 2 below). 
Create a random forest to predict the hospital ratings (1-5) using the 64 measures specified by the CMS.
Evaluate your model using relevant techniques. Report the relative importance of measures according to their predictive power; also report unexpected patterns, if any.
 
Part 2 - Clustering-Based Rating (Unsupervised)
The methodology followed by CMS to assign ratings is described in the report here. It is an unsupervised method. Create an unsupervised clustering model to assign hospital ratings (1-5) using the 64 measures specified by the CMS. The main problem is to calculate the 7 group scores for each hospital. Various methods exist to conduct this analysis, two of which are mentioned below. The second method is similar to the one used by CMS. You can choose either of these ways to complete this part of the project.  
 
Method 1: Figure out your own way to assign weights to the measures in respective groups. The method may or may not be similar to the one used by the CMS, though it should be based on sound reasoning. Using the weights, calculate 7 group scores for each hospital. You can then take the weighted average of group scores to calculate a final score of each hospital, perform clustering, and assign a star rating to each cluster.
    
Method 2: This method uses factor analysis (or latent variable analysis) to find the weight of each measure in respective groups. Using factor analysis, find the group score for each hospital. You can then take the weighted average of group scores to calculate the final score of each hospital, perform clustering, and assign a star rating to each cluster.
 
Using the method of your choice, develop a procedure to:
Calculate and report the weights of all the measures within the respective groups
Compare the weights obtained using this method with the ones obtained from the random forest
Report the group score and the final score of each hospital
Report the final star rating of each hospital  
Compare the rating assigned by you with the actual ratings assigned by CMS and report the analysis using relevant evaluation/comparison metrics
Comment on the explanatory power, discriminatory ability and the stability of the method
 
Part 3 - Recommendations for Hospitals
Suppose you work for a healthcare consulting company. The hospital with Provider ID = 140010 (EVANSTON HOSPITAL) is your client. 
 
The hospital’s current star rating is 3 and it wants to improve it to at least 4 next year. 
 
Using your understanding of the star rating system, recommend ways to improve the rating. 
