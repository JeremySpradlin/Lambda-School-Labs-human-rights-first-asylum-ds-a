# Labs DS template
# Asylum Decision Database -- Human Rights First
An application to assist immigration advocates in winning asylum cases

[Docs](https://docs.labs.lambdaschool.com/data-science/)

## Description
We built an application for human rights first, a 501(c)3 organization. Our application uses optical character recognition to scan input court decisions for such values as the name of the presiding judge, the decision, and the asylum seeker's country of origin, and inserts these values into a database. The hope is that advocates for asylum seekers can use these data to better tailor their arguments before a particular judge and maximize their client's chances of receiving asylum. To use the application offline, follow the steps under Installation.


## Process
* We received some foundation documents from Human Rights First to start building the database and then scraped more pdf documents of asylum cases of the internet.

* Each pdf document was read in through optical character recognition (OCR), and converted the corresponding text to plain text which will allow us to search through each document and retrieve the judge’s name.

* Create an API connecting the database to the front end with the result that uploaded case files can be inserted into the database

* After converting the uploaded PDF to text, we will extract relvant entities from the text to store relevant features in a DB to facilitate data recall and analysis


## Tools

 * [Python 3](https://www.python.org/downloads/)
 * [Pytesseract](https://github.com/madmaze/pytesseract)
 * [FastAPI](https://github.com/tiangolo/fastapi)
 * [AWS Elastic Beanstalk](https://aws.amazon.com/elasticbeanstalk/)
 * [SQLAlchemy](https://www.sqlalchemy.org/)
 * [PDF2Image](https://pypi.org/project/pdf2image/)
 * [Pillow](https://pillow.readthedocs.io/en/stable/)
 * [Pandas](https://pandas.pydata.org/)


## Installation

 After cloning the repository, in your command line run the following commands:
 ```
 cd Lambda-School-Labs-human-rights-first-asylum-ds-a/
 pipenv install --dev
 pipenv shell
 uvicorn app.main:app --reload
 ```
 Then open localhost:8000 in your browser. The application should be running. 

 ## Contributors

 [Steven Lee](https://github.com/StevenBryceLee)

 [Tristan Brown](https://github.com/Tristan-Brown1096)

 [Liam Cloud Hogan](https://github.com/liam-cloud-hogan)

 [Edwina Palmer](https://github.com/edwinapalmer)

 [Jeremy Spradlin](https://github.com/JeremySpradlin)
 
 [Mahmoud Fansha](https://github.com/fansha1994)


 ## License

 This project is licensed under the terms of the MIT license.