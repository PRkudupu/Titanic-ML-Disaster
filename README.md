# Titanic-ML-Disaster
![alt text](stower_titanic.jpg)
## Introduction
The sinking of the RMS Titanic is one of the most infamous shipwrecks in history. On April 15, 1912, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. This sensational tragedy shocked the international community and led to better safety regulations for ships.This data science project will give you introdcution on how to use Python to apply various machine learning techniques to the RMS Titanic dataset and predict which passenger would have survived the tragedy.

#### Data Field details:

The dataset consists of 11 predictor variables and a binary target variable "survived". The features include assengerId
* PassengerId -- A numerical id assigned to each passenger.
* Survived    -- Whether the passenger survived (1), or didn't (0). We'll be making predictions for this column.
* Pclass      -- The class the passenger was in -- first class (1), second class (2), or third class (3).
* Name        -- the name of the passenger.
* Sex         -- The gender of the passenger -- male or female.
* Age         -- The age of the passenger. Fractional.
* SibSp       -- The number of siblings and spouses the passenger had on board.
* Parch       -- The number of parents and children the passenger had on board.
* Ticket      -- The ticket number of the passenger.
* Fare        -- How much the passenger paid for the ticker.
* Cabin       -- Which cabin the passenger was in.
* Embarked    -- Where the passenger boarded the Titanic.
There are 891 records of passengers, out of which 342 survied and 549 who did not survive.

## Steps 
Data Inspection

Data Understanding

Data Preparation (cleaning - treat missing values, treat outliers and other bad data, Normalization)

Split the Data

Visualize

Train the Model

Test the Model <a>(deploy on unseen data)
      
Evaluate the performance of the Model

### Inference
<code>
#The columns we'll use to predict the target
predictors_dim = ["Pclass", "Sex", "Age", "SibSp", "Parch", "Fare", "Embarked"]
y_predictions = nn.predict(titanic_test[predictors_dim])

#Create a new dataframe 
submission = pd.DataFrame({
        "PassengerId": titanic_test["PassengerId"],
        "Survived": y_predictions
    })
print(submission)
</code>
# Titanic-ML-Disaster
![alt text](op.jpg)
### License 
Active Record is released under the MIT license:
 <a href="https://opensource.org/licenses/MIT">opensource.org/licenses/MIT</a>.

