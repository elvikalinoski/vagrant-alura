# vagrant-alura
Curso de Vagrant na Alura

---
**Download**
 ```https://www.vagrantup.com/```

**Instalando**
 ```sudo dpkg -i vagrant_2.2.14_x86_64.deb```

**Verificando a versão da instalação**
 ```vagrant --version```

**Clone do projeto criado no GitHub para a aula**
 ```git clone git@github.com:elvikalinoski/vagrant-alura.git```

**Criando uma VM com o Vagrant**
 ```vagrant init hashicorp/bionic64```

**Inicializando a VM**
 ```vagrant up```

**Verificando o status da VM**
 ```vagrant status```

**Conecta a máquina via SSH**
 ```vagrant ssh```

**Desliga a máquina**
 ```vagrant halt```

**Gere um par de chaves com a ferramenta keygen:**
 ```ssh-keygen -t rsa```

**Acesse a máquina virtual:**
 ```vagrant ssh```

**Dentro da máquina virtual, visualize a pasta vagrant que é um compartilhamento da pasta em seu computador local:**
 ```ls /vagrant```

**Agora, copie a chave pública da pasta local vagrant para a máquina virtual:**
 ```cp /vagrant/id_bionic.pub .```

**Adicione a chave pública na máquina virtual, no arquivo .ssh/authorized_keys**
 ```cat id_bionic.pub >> .ssh/authorized_keys```

**Teste a conexão SSH com as chaves geradas:**
 ```ssh -i sua_chave_privada vagrant@seu-ip```

**Executa o provision**
 ```vagrant provision```


**Valida arquivo de configuração**
 ```vagrant validate```