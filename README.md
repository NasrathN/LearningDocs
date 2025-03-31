# LearningDocs

Learning-1 : Was having issue during git push due to two github accounts . I got to know that , for each repository we can set git user and git email id 
Steps 
- go to that directory in local
- git config user.name "NasrathN"
- git config user.email "nasrath.n@outlook.com"

I could do git push after this.

If i come out of that directory , and check the value of user and email - I get the actual values stored in config file .
To check username and email id :
git config user.name
git config user.email

Learning-2 : FASTAPI Course

1. For a particular project of python in local machine , we can select a specific python interpreter if there are more than one version of python installed
- On VS code : View --> Command Palette --> Python: Select Interpreter
- Select python.exe from the scripts folder in virtual environment folder

2. async keyword in any methods defined in fast api is optional . It tells the method to behave asynchronously .

3. Fast API installation : pip install fastapi[all]

4. Basic code section :

from fastapi import FastAPI
app = FastAPI() ------> Creating an instance of FastAPI
@app.get('/')
async def root():
    return {"Message":"Hello world"}

5. Command to run local server : uvicorn main:app ---> uvicorn is built in server of fastapi ; Command is - uvicorn <filename>:<instanc_name>

6. To avoid restarting the server everytime there is change in code , make use of the command uvicorn main:app --reload

7. Pydantic library has nothing to do with fastapi . It can be used with any other python code . Pydantic is used for data schema validation.

