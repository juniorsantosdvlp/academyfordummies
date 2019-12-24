# Projeto voltado para treinamento de profissionais de TI

comece com o GIT seguindo esses passos, 

1. Crie uma conta no GitHub

2. Faça um [Fork](https://github.com/UNIVALI-LITE/Portugol-Studio/wiki/Fazendo-um-Fork-do-reposit%C3%B3rio) do projeto.

3. [Clone](https://help.github.com/pt/github/creating-cloning-and-archiving-repositories/cloning-a-repository) o repositorio em sua máquina.

4. Crie um branch com o seu nome.

5. Se apresente modificando o arquivo apresentacao e depois envie o Pull Request.

Do clone ao pull request https://blog.da2k.com.br/2015/02/04/git-e-github-do-clone-ao-pull-request/


# -------------------------------------------------------------- #

Dockerfile

Esse arquivo será usado para criar a imagem da aplicação que estiver no repositório. Ele é uma abstração conteinerizada que colocará todas as dependências da aplicação que foram postas no decorrer da criação do app, dentro de uma imagem, ao que será usada em seguida para construir o conteiner de fato.

1. Primeiro vamos buildar a imagem. - > docker build -t <nome_da _imagem> .

2. Vamos verificar se a imagem foi buildada com sucesso. - > docker images -a

3. Agora, vamos rodar nosso conteiner (caso ja tenha a aplicação). -> docker run -it <nome_do_container> -p <porta> <nome_da_imagem>