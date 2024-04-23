# Contêiner do Docker

???+ importante

    Antes de fazer esse procedimento é preciso já ter clonado o Backend e rodado o comando: mvn clean package

O primeiro passo para você testar o nosso projeto é baixar o aplicativo desktop Docker:

[https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/){target="_blank"}

Após a instalação do Docker clone o repositório:

    
    https://github.com/henrique-sdc/Docker_Valorant.git

Abrindo o Repositório:

Navegue até o diretório do projeto clonado:

    cd Docker_Valorant

Abrir a IDE Visual Studio Code através:

    cd code .

Abra o terminal CMD e execute o comando:

    docker compose up -d --build --force-recreate

Feito isso você terá criado um contêiner no Docker onde estará nosso banco de dados.

É preciso abrir o pgAdmin caso não tenha instalado instale [PostgreSQL](https://www.postgresql.org/download/) depois de ter instalado abre o pgAdmin crie um banco de dados vava, após isso cole este comando no terminal SQL para criar nosso banco:

        CREATE TABLE IF NOT EXISTS public.jogadores
        (
            id SERIAL PRIMARY KEY,
            username VARCHAR(255),
            tag VARCHAR(100),
            playtime NUMERIC(10,3),
            matches NUMERIC(10,3),
            rating VARCHAR(100),
            level VARCHAR(100),
            loses VARCHAR(100),
            damage_round VARCHAR(100),
            headshot VARCHAR(100),
            win VARCHAR(100),
            wins NUMERIC(10,3),
            kills NUMERIC(10,3),
            deaths NUMERIC(10,3),
            assists NUMERIC(10,3),
            kad_ratio VARCHAR(100),
            kills_round VARCHAR(100),
            clutches VARCHAR(100),
            top_agents_1 VARCHAR(255),
            top_hours_agent_1 VARCHAR(100),
            top_matches_agent_1 VARCHAR(100),
            top_win_agent_1 VARCHAR(100),
            top_kd_agent_1 VARCHAR(100),
            top_weapon_1 VARCHAR(255),
            top_weapon_headshot_1 VARCHAR(100),
            top_weapon_2 VARCHAR(255),
            top_weapon_headshot_2 VARCHAR(100),
            top_maps_1 VARCHAR(255),
            top_porcentagem_map_win_1 VARCHAR(100)
        );

???+ importante

    Toda vez que você for usar nosso sistema é preciso verificar se o Docker está ligado.