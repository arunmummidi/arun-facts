Alexa interface code is in alexa/ directory

Lambda backend code is in lambda directory

Build locally:
================
1) Download contents of lambda/py
2) setup virtualenvironmetn
  $ virtualenv skill_env
3) Install dependencies
$ cd lambda/
$ pip install -r py/requirements.txt -t skill_env
$ cp -r py/* skill_env/
$ cd skill_env && zip -r package.zip *
$ cp package.zip ~/Desktop

Upload the package.zip file to Lambda
