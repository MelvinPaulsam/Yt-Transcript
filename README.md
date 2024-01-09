# Installation
## 1. Clone the repository
`git clone https://github.com/MelvinPaulsam/Yt-Transcript.git`
## 2. Create a Python environment
Python 3.6 or higher using venv or conda. Using venv:

`cd langchain-experiments`<br>
`python3 -m venv env`<br>
`source env/bin/activate`<br>

Using conda:

`cd langchain-experiments`<br>
`conda create -n langchain-env python=3.8`<br>
`conda activate langchain-env`<br>
## 3. Install the required dependencies
`pip install -r requirements.txt`
## 4. Set up the keys in a .env file
First, create a .env file in the root directory of the project. Inside the file, add your OpenAI API key:

`OPENAI_API_KEY="your_api_key_here"`
Save the file and close it. In your Python script or Jupyter notebook, load the .env file using the following code:

`from dotenv import load_dotenv, find_dotenv
load_dotenv(find_dotenv())`
By using the right naming convention for the environment variable, you don't have to manually store the key in a separate variable and pass it to the function. The library or package that requires the API key will automatically recognize the OPENAI_API_KEY environment variable and use its value.

When needed, you can access the OPENAI_API_KEY as an environment variable:

`import os
api_key = os.environ['OPENAI_API_KEY']`
Now your Python environment is set up, and you can proceed with running the experiments.

