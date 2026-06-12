# 1. Create Azure Account
  -	Go to the Azure Portal.
  -	Sign up for a new account using your email ID.
  -	Microsoft provides a free trial with 30 days subscription and credits (usually $200).
  -	Verify your identity with a phone number and payment method (no charges during trial unless you upgrade).

# 2. Create Azure SQL Database
-	In the Azure portal, click Create a resource → Databases → SQL Database.
-	Select your Resource Group or create a new one.
-	Provide a Database name and configure a SQL Server (admin login + password).
-	Choose a pricing tier (Basic is fine for testing). Configure the storage. Select “Basic(For less demanding workloads)

<img width="604" height="381" alt="image" src="https://github.com/user-attachments/assets/736df584-8c4c-472c-a11e-60fdb963c13f" />
<img width="940" height="453" alt="image" src="https://github.com/user-attachments/assets/080b4db5-1117-4edd-a5f5-c2e2aaff0563" />
-	Configure Additonal settings. Select Sample, so that it will allow you to use the sample dataset.
<img width="679" height="573" alt="image" src="https://github.com/user-attachments/assets/1c57b4ad-6346-4d7e-807b-7b505758a998" />
-	Click Review + Create to deploy.

# 3. Create Databricks Community Edition
-	Search for databricks on azure portal
-	Click on it and create an account in databricks community edition (use same server that you have created in first step). 
<img width="559" height="354" alt="image" src="https://github.com/user-attachments/assets/30e7dbd3-af4c-420a-afb2-33b85350daac" />
-	Once the account is created , it looks as below.
<img width="940" height="281" alt="image" src="https://github.com/user-attachments/assets/dee35385-3833-4b98-b13e-56782477ca84" />

# Step 4: Export Tables from Azure to Databricks
- After executing the scripts provided in jupyter source file, you will be able to see the tables in databricks.
<img width="103" height="67" alt="image" src="https://github.com/user-attachments/assets/d168a42c-3871-44bf-8f83-d403a7fcf805" />

 <img width="940" height="457" alt="image" src="https://github.com/user-attachments/assets/5569f2c6-6c98-47aa-895c-484eb1017739" />

# How to connect the JDBC_URL to Jupyter notebook in DataBrick :- 
   ```sh
jdbc_url = "Put this your server URL"
   ```
   ```sh
connection_props = {
    "user": "Your user_id",
    "password": "mypassword",
    "driver": "com.mysql.cj.jdbc.Driver"
}
   ```
