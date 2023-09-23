# ML-Academy-Project

Fraud Detection in Electricity and Gas Consumption

The Tunisian Company of Electricity and Gas (STEG) is a public and non-administrative company that is responsible for delivering electricity and gas across Tunisia. The company has suffered tremendous losses in the order of 200 million Tunisian Dinars due to fraudulent manipulations of meters by consumers.

A crucial problem that these companies face is the imbalance between the energy billed and the energy delivered. This problem is called energy losses caused by fraud or technical causes like meter malfunctions, pipes damages and other technical issues.

The dataset contains two tables: The first is about Clients data and whether it has been labelled as fraud or not. The second table shows all invoices for these clients with information.



# Overview

The main goal of this project is to feed data into a machine learning model that will classify transactions as fraudulent or honest.




# Data Preprocessing and Visualization
STEG's data is divided into two files. The first comprises client information, and the second covers billing history from 2005 to 2019.

After doing some preprocessing and visualisation for each dataset, we combined the client and invoice datasets. This produced an imbalanced dataset.

   ![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/ed11d397-3669-4b4f-b298-1b754ffe1ce3)


This can be a concern for machine learning models, as they can be biassed towards the dominant class. Over- or under-sampling strategies can be used to deal with this problem.

   ![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/86ce47a9-2f5b-49a5-a963-720560042dac)


# Inferences
- Exploring


     ![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/020a6cd6-4547-4770-9a2d-c0bfb75b8a20)
 
     ![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/4981c55e-326e-43de-aba8-5c7383ea2c69)


    The plot shows the proportion of counter type (electricity to gas) for the Tunisian Company of Electricity and Gas (STEG). The client prefers counter-type ELEC rather than GAZ. Other than that, the difference between fraud percentages is small.

    --------

     ![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/0771946b-f6ab-417f-8ab4-17dbea084700)

     ![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/2a538199-e428-4dd3-8711-2276c114d45e)
  
    - The majority of clients are from client_catg 11.
    - Most frauds (by percentage) are from client_catg 51, with over 17%..
    - According to the data, client_catg 51 is not safe, and client_catg 12 is probably the safest.


    --------

     ![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/87a04540-4a21-4f43-9dfb-d0ec06bf83ff)

     ![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/53f719b2-a147-4b0c-9d8c-93ef8c2e72f3)

     
     - Counter_statue 0 is used by the majority of clients, and strangely, it does not have the largest percentage of fraud.


    --------

     ![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/2a719056-47bf-4e13-ba01-8e2532d2ef67)

     ![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/96475216-0ae0-4eeb-a273-959727d3a2e7)


     - The majority of clients come from Region 101 and, interestingly, have a low fraud rate.
     - Based on the data, regions 103, 372, and 311 are not safe from fraud, with more than 10% of cases of fraud.
     - Regions 101 and 301 are safe, considering they have a low percentage of fraud with high transactions.
     - Regions 199, 399, and 206 are safe, but they also have only some records of transactions, not as many as the others.


This information can be used to identify areas that may require greater examination or monitoring in order to prevent fraud. It can also aid in spotting trends or patterns in fraudulent activity across multiple locations, which can then be used to inform the creation of future efforts to avoid or reduce fraudulent activities.







# Comparision Models and Results
- K-Neighbors Classifier:

    Model accuracy score: 0.9539

  
- Random-Forest Classifier:

    Model accuracy score: 0.7900

  
- Logistic-Regression Classifier:

    Model accuracy score: 0.5641




  ![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/5d0dfe35-7b34-4d2c-9689-9683f040fc3c)



# Conclusion

- client_catg: 51 have the highest percentage of being fraud, but also have the lowest record, so we need more data on this.
- region: Based on data, regions 103, 372, and 311 are not safe from fraud, with more than 10% of cases of fraud. Regions 101 and 301 are safe, considering they have a low percentage of fraud with high transactions. Regions 199, 399, and 206 are safe, but they also have only some records of transactions, not as many as the others.
- counter_statue: 4 has the highest value (>10%) even though it has a really low transaction record.

  
   # Note
    The data has far too many outliers, particularly in the invoicing dataset. In addition, imbalanced attributes It is advisable to look into it in the future.
