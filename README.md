# Realtime Speech-To-Image

How to build a real time Speech-To-Image Web App using AssemblyAI and DALL.E by OpenAI

## Step 1: Obtain the API Keys

1. Obtain the AssemblyAI API key

   Obtaining the AssemblyAI API key
   Getting access to the AssemblyAI API is extremely simple and starts with a free registration with AssemblyAI.
   Next, after logging in to your account, you will find the `API key` on the right hand panel. Copy and Save it somewhere

   Note: YOU WILL HAVE TO UPGRADE YOUR AssemblyAI ACCOUNT TO BE ABLE TO USE THE REAL-TIME TRANSCRIPTON FEATURE. MAKE SURE YOU HAVE AT LEAST $5 TO SPARE
   
2. Obtain the OpenAI API Key


## Step 2: Create a new python environment and then download the Github Repo

Open Your terminal and create a virtual environment named `myproject`

`python3.9 -m venv myproject`

Activate the virtual environment with the following command

```
cd myproject
source bin/activate
```

Next we will have to download the Github Repo

```
git clone https://github.com/Yingi/Real-time-STI.git
cd Real-time-STI
```

Next, we will download the required python packages to enable us run the web app.

`pip install -r requirements.txt`

## Step 3: Paste your API Keys you copied from AssemblyAI and OpenAI.

For AssemblyAI API Key, open `secrets.toml` file located in a folder called `.streamlit`

`api_key = ‘xxxxxxxxx’`     #Paste your AssemblyAI API Keys here

Next, For OpenAI, open `streamlit_app.py` file search for:
`ai.api_key = “xxxxxxxxxx” `   #Paste your OpenAI API Keys here


## Step 4: Launch the App

You can now launch the app with the below command

`streamlit run streamlit_app.py`

When the app is launched on your browser, To start using the speech to image functionality, click on `Start` button

Start speaking by describing the image you want. Example say `“A white car”`. Then click on the `Stop` button

After some few seconds, VOILÀ, you will see the image of a white car displayed.




`Congratulations!!!!!`, You have successfully launched a Speech-To-Image web app.

In the future, we will be truncating the speech so as not to overwhelm the trancsription algorithm

Thanks!!


