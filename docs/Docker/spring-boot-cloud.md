# Contêiner do Docker

???+ importante

    Antes de fazer esse procedimento é preciso já ter clonado o Backend e rodado o comando: mvn clean package

O primeiro passo para você testar o nosso projeto é baixar o aplicativo desktop Docker:

[https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/){target="_blank"}

Após a instalação do Docker clone o repositório:

[https://github.com/henrique-sdc/Docker_Valorant.git](https://github.com/henrique-sdc/Docker_Valorant.git){target="_blank"}

Abrindo o Repositório:

Navegue até o diretório do projeto clonado:

    cd Docker_Valorant

Abrir a IDE Visual Studio Code através:

    cd code .

Abra o terminal CMD e execute o comando:

    docker compose up -d --build --force-recreate

Feito isso você terá criado um contêiner no Docker onde estará nosso banco de dados.

???+ importante

    Todo vez que você for usar nosso sistema é preciso verificar se o Docker está ligado.

