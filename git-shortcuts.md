#Instalando o git no servidor
	sudo yum install git
	# Criar chave ssh
	 ssh-keygen -t rsa -b 4096
	nome da chave:{key-name}
	passphrase:{senha}
	ssh-add {key-name} caso nao funcione faça: ssh-agent /bin/sh depois: ssh-add {key-name}
	# Conectando ao git
	ssh -T git@github.com
	# Copiando repositorio
	git clone git@github.com:hospeda/base-docker.git

#Clonar repositório para LOCAL
  [/local-repository]# git clone . #github reconhece a pasta do repositório após fazer o clone .
  
#Puxar repositório remoto descartando alterações locais
  git add *
  git stash
  git pull

  
  
