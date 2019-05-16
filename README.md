# Manual Git
As informações deste arquivo se refere à utilização do Git como ferramenta de versionamento de código para projetos que o necessitam.
Há diferença entre usar a ferramenta Git e o site GitHub. A `ferramenta Git` serve para você versionar seu código, ou seja, criar pontos dos arquivos de seu código onde você possa desfazer alterações que fez posteriormente. Já o  `site GitHub` serve para hospedar o seu projeto.

Abaixo encontra-se informações pertinentes que são necessárias para seu uso.

### Instalação do Git

* Windows [Link Download](https://git-scm.com/download/win).
> Faça a instalação normal de um programa do Windows

* Distribuições Linux
-No terminal, digite:
> sudo apt-get install git

* Mac
>  Por padrão, ja vem instalado

### Git Básico

##### Adicionando Git à um projeto existente

-Crie um repositório no GitHub.
-Navegue até a pasta raiz do seu projeto pelo terminal e dê os comandos:
```bash
$ git init
$ git remote add origin LINK # substitua pelo link do seu repositório no GitHub
$ git add .
$ git commit -m "sua mensagem aqui"
$ git push origin master 
```
Para exemplificar um *commit*, vamos pensar que ele é um _pacote._ 
Quando se quer enviar um pacote, primeiro você põe o conteúdo dele, fecha o pacote e depois envia ao destinatário. 
O `commit` é parecido com isso, você adiciona seu código ao pacote e depois fecha ele, ao fechá-lo você *cria um ponto de restauração* para ele, ou seja, qualquer modificação futura que você fizer será possível reverter para este commit.
Agora vamos entender o que estamos fazendo em cada linha.

```bash
Inicia um repositório vazio
Adiciona uma conexão para dizer onde que é seu repositório remoto
Adiciona todos os arquivos da sua pasta para o pacote criado no seu computador
Fecha o pacote, adicionando uma mensagem neste commit e criando um ponto de restauração no seu computador
Envia seu código e commits para seu repositório no GitHub *Esse comando deixará seu código atualizado para outras pessoas que queiram baixá-lo
```

##### Clonando um repositório no GitHub

-Navegue pelo terminal até a pasta onde queira clonar o repositório e dê os seguintes comandos:

```bash
$ git clone LINK # substitua pelo link do repositório que queira clonar
```

*Ao clonar, ele cria um repositório Git na pasta que é referente ao repositório de onde foi tirado


