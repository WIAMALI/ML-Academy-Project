# ML-Academy-Project

Fraud Detection in Electricity and Gas Consumption

The Tunisian Company of Electricity and Gas (STEG) is a public and non-administrative company that is responsible for delivering electricity and gas across Tunisia. The company has suffered tremendous losses in the order of 200 million Tunisian Dinars due to fraudulent manipulations of meters by consumers.

A crucial problem that these companies face is the imbalance between the energy billed and the energy delivered. This problem is called energy losses caused by fraud or technical causes like meter malfunctions, pipes damages and other technical issues.

The dataset contains two tables: The first is about Clients data and whether it has been labelled as fraud or not. The second table shows all invoices for these clients with information.


# Data Preprocessing and Visualization
STEG's data is divided into two files. The first comprises client information, and the second covers billing history from 2005 to 2019.

After doing some preprocessing and visualisation for each dataset, we combined the client and invoice datasets. This produced an imbalanced dataset.

![image](https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/70214242-fa97-4135-9696-d931e2f8180f)

# Extracting insights
- Distribution of variables

    <img width="560" alt="image" src="https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/de71f8b2-48ee-4fa3-b180-447f90d247e0">
  
    The majority of clients are from client_catg 11.


    <img width="574" alt="image" src="https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/2942e430-7f44-4775-8c4d-338ea4f52c12">

    The majority of clients are from Region 101.


    <img width="1000" alt="image" src="https://github.com/WIAMALI/ML-Academy-Project/assets/104154401/a3e1107f-69d4-483d-ab9f-eb65b8018d61">

    The highest fraud percentage occurs at counter_statue 4.



# Models and Results
- K-Neighbors Classifier:

    Model accuracy score: 0.9817

  
- Random-Forest Classifier:

    Model accuracy score: 0.6065
