## Comandos Sam

# Usando SAM
### Deploy simples com SAM
zip function.zip lambda_function.py

aws lambda update-function-code --profile boxt --function-name hello --zip-file fileb://function.zip

* sam init
* sam local invoke "HelloWorldFunction"
* sam local invoke "HelloWorldFunction" events/event.json
* sam local start-api



/*******-----

test -d ~/.linuxbrew && eval $(~/.linuxbrew/bin/brew shellenv)
test -d /home/linuxbrew/.linuxbrew && eval $(/home/linuxbrew/.linuxbrew/bin/brew shellenv)
test -r ~/.bash_profile && echo "eval \$($(brew --prefix)/bin/brew shellenv)" >>~/.bash_profile
echo "eval \$($(brew --prefix)/bin/brew shellenv)" >>~/.profile