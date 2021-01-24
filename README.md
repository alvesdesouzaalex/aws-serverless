# aws-serverless


## Configuração Profile
aws configure --profile "nome_profile"


# Usando SAM
### Deploy simples com SAM
zip function.zip lambda_function.py

aws lambda update-function-code --profile boxt --function-name hello --zip-file fileb://function.zip


### Deploy com dependencias com SAM



# Usando Serverless


#### Pre instalar
`
sudo apt-get install python3;
sudo apt-get install python3-pip;
sudo pip3 install virtualenv;
`

mkdir -p hello-word/app && cd hello-word

* Create virual environment
virtualenv -p python3 venv
. venv/bin/activate

* Create user admin in AWS and configure profile

* Installing and Configuring Serverless Framework

npm install -g serverless

* Let’s configure Serverless:
serverless config credentials --provider aws --key <ACCESS KEY ID> --secret <SECRET KEY>

* Configure default deploy
serverless deploy --aws-profile arch-serverless

export AWS_PROFILE="serverless" && export AWS_REGION=us-east-1


> Deploying our Project for first time
export AWS_PROFILE="arch-serverless" &&
serverless deploy
>


* Others deploy
serverless deploy -v

* Invoke the function
sls invoke -f hello

* Tailing logs
sls logs -f hello --tail

* Delete this function
serverless remove or sls remove


**** Reference: https://medium.com/faun/aws-lambda-serverless-framework-python-part-1-a-step-by-step-hello-world-4182202aba4a


