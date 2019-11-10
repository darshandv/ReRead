# ReRead
Web application to proofread documents and derive research-oriented insights. 


Install the required dependencies using the below command into a virtual environment

`pip3 install -r requirements.txt`

**OR**

Below are the dependencies required for the application in detail. You can install each of them separately.

### Dependencies

**Sumy Summarizer**

`pip install git+git://github.com/miso-belica/sumy.git`

**PyTorch**

`pip3 install http://download.pytorch.org/whl/cpu/torch-0.4.1-cp36-cp36m-linux_x86_64.whl`

`pip3 install torchvision`

**Django Widget Tweaks**  

`pip3 install django-widget-tweaks`

**Gensim**  
`pip3 install gensim`

**Language-check**  
`pip3 install language-check`


### Instructions to set up server
+ Clone the repository
+ Run `python3 manage.py migrate`
+ Run `python3 manage.py makemigrations`
+ Run server using `python3 manage.py runserver` and navigate to localhost:8000

### Instructions to set up https:// server
To setup a ssl server you need a certificate and a key. Use a certificate from a CA that your browser trusts, for example [Letsencrypt](https://letsencrypt.org/). If you have a certificate/key pair from a certificate authority, you can tell Django SSL Server to use it with the following steps:
+ Clone the repository
+ Run `python3 manage.py makemigrations`
+ Run `python3 manage.py migrate`
+ Run sslserver using `python manage.py runsslserver --certificate /path/to/certificate.crt --key /path/to/key.key` and navigate to https://127.0.0.1:8000/


### Features
+ Grammar Error Correction
+ Keyword Extraction and Associated Literature References
+ Abstract Summarisation
