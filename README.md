# heart_disease_prediction
predicting heart disease possible risk using UCI dataset ,This data set dates from 1988 and consists of four databases: Cleveland, Hungary, Switzerland, and Long Beach V. It contains 76 attributes, including the predicted attribute, but all published experiments refer to using a subset of 14 of them. The "target" field refers to the presence of heart disease in the patient. It is integer valued 0 = no disease and 1 = disease.




observations from the describtion of the dataset 
1-dataset contains 1025 records for the 13 features which will be denoted as X
2-same values for the target column Y- 1025 label which confirms no null or missing values
3-mean of the ages =54.43 over 1025 patients 
where std stands for standard deviation which is equivalent to 

sqrt((x-xp)^2)/n-1

where x is the data point coming from the dataset 
xp is the average/mean of the sample 
n: size of the sample 
First, take the square of the difference between each data point and the sample mean, finding the sum of those values.
Next, divide that sum by the sample size minus one, which is the variance.
Finally, take the square root of the variance to get the SD.



minimum age at the dataset is 29 year-old
maximum age at the dataset is 77 year-old
50% of the patients aged almost 56 years old



4-Gender or sex = average values = 0.69 which will be one / zero for male/female




5-cp refers to chest pain index

average choletroel index is 249 mg/dl

reference : 200 to 239 mg/dL


6-fasting blood sugar which describes the blood sugar test without eating from 6-8 hours

0.149

reference for normal ranges : 
0.100 to 0.125 g/dL



7-resting electrocardiographic results 


0 = normal; 1 = having ST-T; 2 = hypertrophy

normal : referes to normal echo results


ST-T : ST- and T-wave changes may represent cardiac pathology 
or be a normal variant. 
Interpretation of the findings, therefore,
depends on the clinical context and presence of similar findings on prior electrocardiograms.



hypertrophy :  a disease in which the heart muscle becomes thickened (hypertrophied). 
The thickened heart muscle can make it harder for the heart to pump blood.



8-thalach :maximum heart rate achieved

9-exang: exercise induced angina


10-old peak : ST depression induced by exercise relative to rest

11-slope : the slope of the peak exercise ST segment 
(1 = upsloping; 2 = flat; 3 = downsloping)

12-number of major vessels (0-3) colored by flourosopy

13-thal - 3 = normal; 6 = fixed defect; 7 = reversable defect



![uci](https://user-images.githubusercontent.com/37244966/191237072-95cad98b-afb0-414b-9e66-5fe9ce23812a.png)





KNN algorithm notes :-
Training algorithm:

for i = 1, ..., n in the n-dimensional training dataset D (|D| = n):

   -store (x(i),f(x(i))
    
prediction algorithm:


   closest_point=none
   closest_distance= infinity 
    
    
    
 for i=1,.............n:
 current distance := d(x[i], x[q])
 
   #where d is the euclidean distance between x[i] and x[q]
     
     
     
   ![euclie](https://user-images.githubusercontent.com/37244966/191277508-0aec8a87-279c-4433-8bc5-911ae6a01f06.png)
     
     
     
     
   if current_distance <close_distance (d(x[i],x[q])<infinity ? yes 
      closest_distance := current distance
       closest_point := x[i]
       
       
 the prediction h(x[q])-> target value of the closest_point
 
 
      






