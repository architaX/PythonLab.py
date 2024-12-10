import pandas as pd
data={'Name':['Alice','Bob','Charlie',None,'Eve'],'Age':[25,None,30,22,None],'City':['New York',None,'Los Angeles','Chicago','Miami']}
df=pd.DataFrame(data)

def analyse_missing_data(df):
    print("DataFrame:")
    print(df)
    print("\nMissing Data Analysis")
    
    missing_data=df.isnull().sum()
    print("Missing values in each column: ")
    print(missing_data[missing_data>0])
    
    missing_percentage=(missing_data/len(df))*100
    print("\nPercentage of missing values in each column:")
    print(missing_percentage[missing_percentage>0])
    return missing_data,missing_percentage

def handle_missing_data(df):
    print("\nChoose a method to handle missing data")
    print("1.Fill missing values with a specifies value")
    print("2.drop rows with missing values")
    print("3.Drop columns with missing values")
    choice=input("Enter your choice(1|2|3):")
    if choice=='1':
        value=input("Enter the value to fill missing data:")
        df_filled=df.fillna(value)
        print("data after filling missing values")
        print(df_filled)
    elif choice=='2':
        df_dropped_rows=df.dropna()
        print("\n Data after dropping rows with missing values")
        print(df_dropped-rows)
    elif choice=='3':
        df_dropped_coloumns=df.dropna(axis=1)
        print("\ndata after dropping columns with missing values: ")
        print(df_dropped_columns)
    else:
        print("Invalid Choice! Please enter 1,2or 3")
        
missing_data,missing_percentage=analyse_missing_data(df)
handle_missing_data(df)
