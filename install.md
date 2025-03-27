## INSTALL INSTRUCTIONS

### Documenters Project

### Minh Anh Dang, Annie Wilcox, Ryan Hanks, Ryan Flanery, Samuel Corder

### Step 0: Scrape for officials' contact information

1. Clone this notebook into your working directory by using ```git clone https://github.com/minh-msu/CMSE495_Documenters```
2. Navigate to ```Email_Phone_Location_Scraper.ipynb```
3. Run the whole notebook
4. The resulting dataframe will be saved onto ```contact.csv```

### Step 1: Set Up Google Sheets API

Our project is in HTML, because most browsers block opening local files, we stored our data using the Google Sheets API. Google Sheets API is free for 90 days. Here's how you can start using it:

***
**NOTE:** MSU does not allow students to use Google Sheets API on their msu.edu emails. If you are downloading this as a student, you must use your personal email or set up a new Google Account.
***

1. First, we need to create a project

- Go to your [Google Cloud Console](https://console.cloud.google.com)
- On the top of the screen, select **Select a Project > New Project**
- Give your project a name, select **Create**

2. Next, we need to enable Google Sheets API.

- Select the menu on the left, then select **APIs & Services > Library**
- Search for **Google Sheets API** and enable it

3. Now that we have Google Sheets API enabled, we need to generate an API key.

- In **APIs & Services**, select **Credentials**
- Select **Create Credentials > API Key**

We have generated our API key, and now we can access any public Google Sheet!

### Step 2: Downloading and editing the HTML Project

***
**NOTE:** We are using Visual Studio Code to edit our HTML files, any code editing software will work for you. You can even open the files on your computer's built in text editor and still effectively do this tutorial! You do not need any coding knowledge to complete this tutorial!
***

1. On this GitHub repository (https://github.com/minh-msu/CMSE495_Documenters) download ```DetroitFinders.zip```. Unzip the file wherever you like.
2. Select **File > Open File** and open DetroitFinder
3. Open ```index.html```. In line 38, edit the url to include your Google Sheets API key at the end. Only change the part that says ```YOUR_API_KEY_HERE``` to your API key.
4. Open ```about.html```. In line 22, edit the url to include your Google Sheets API key at the end. Only change the part that says ```YOUR_API_KEY_HERE``` to your API key.
5. Select **File > Save All**

You can now close Visual Studio Code.

### Step 3: Running the Project (Demo)

All that's left now is to open ```index.html``` in any browser and starting searching! Simply click the magnifying glass, and start searching for someone in Detroit's local government. Names should appear, and you can select one to find more about them.

![image](https://github.com/user-attachments/assets/ea39c08e-350a-49c8-a078-c5c03dfc43fb)

***
**NOTE:** When following this demo, you should not need to create your own copy of/version of the data. However, if you have interest into converting your own websites into CSVs, and consequenstly Google Sheets in order to display your own data via the HTML demo, please follow the ```HTML_to_df.ipynb``` tutorial.
***

