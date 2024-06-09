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

        CREATE TABLE jogadores (
        id SERIAL PRIMARY KEY,
        Username VARCHAR(255),
        Tag VARCHAR(255),
        Url TEXT,
        DpR NUMERIC,
        Kdr NUMERIC,
        Headshot NUMERIC,
        Win NUMERIC,
        Wins NUMERIC,
        KAST NUMERIC,
        DDdeltaR NUMERIC,
        Kills NUMERIC,
        Deaths NUMERIC,
        Assists NUMERIC,
        ACS NUMERIC,
        kad_ratio NUMERIC,
        kills_per_round NUMERIC,
        Clutch1v1s NUMERIC,
        flawless_rounds NUMERIC,
        current_rating NUMERIC,
        peak_rating NUMERIC,
        Playtime NUMERIC,
        Matches NUMERIC,
        Level NUMERIC,
        Losses NUMERIC,
        top_agent1 VARCHAR(255),
        top_agent2 VARCHAR(255),
        top_agent3 VARCHAR(255),
        top_hours_agent1 NUMERIC,
        top_hours_agent2 NUMERIC,
        top_hours_agent3 NUMERIC,
        top_matches_agent1 NUMERIC,
        top_matches_agent2 NUMERIC,
        top_matches_agent3 NUMERIC,
        top_win_agent1 NUMERIC,
        top_win_agent2 NUMERIC,
        top_win_agent3 NUMERIC,
        TopKDAgent1 NUMERIC,
        TopKDAgent2 NUMERIC,
        TopKDAgent3 NUMERIC,
        top_weapon1 VARCHAR(255),
        top_weapon_headshot1 NUMERIC,
        top_weapon_bodyshot1 NUMERIC,
        top_weapon_legshot1 NUMERIC,
        top_weapon_kills1 NUMERIC,
        top_weapon2 VARCHAR(255),
        top_weapon_headshot2 NUMERIC,
        top_weapon_bodyshot2 NUMERIC,
        top_weapon_legshot2 NUMERIC,
        top_weapon_kills2 NUMERIC,
        top_weapon3 VARCHAR(255),
        top_weapon_headshot3 NUMERIC,
        top_weapon_bodyshot3 NUMERIC,
        top_weapon_legshot3 NUMERIC,
        top_weapon_kills3 NUMERIC,
        top_map1 VARCHAR(255),
        top_map_winrate1 NUMERIC,
        top_map_wins1 NUMERIC,
        top_map_losses1 NUMERIC,
        top_map2 VARCHAR(255),
        top_map_winrate2 NUMERIC,
        top_map_wins2 NUMERIC,
        top_map_losses2 NUMERIC,
        top_map3 VARCHAR(255),
        top_map_winrate3 NUMERIC,
        top_map_wins3 NUMERIC,
        top_map_losses3 NUMERIC,
        top_map4 VARCHAR(255),
        top_map_winrate4 NUMERIC,
        top_map_wins4 NUMERIC,
        top_map_losses4 NUMERIC,
        top_map5 VARCHAR(255),
        top_map_winrate5 NUMERIC,
        top_map_wins5 NUMERIC,
        top_map_losses5 NUMERIC,
        top_map6 VARCHAR(255),
        top_map_winrate6 NUMERIC,
        top_map_wins6 NUMERIC,
        top_map_losses6 NUMERIC,
        top_map7 VARCHAR(255),
        top_map_winrate7 NUMERIC,
        top_map_wins7 NUMERIC,
        top_map_losses7 NUMERIC,
        top_map8 VARCHAR(255),
        top_map_winrate8 NUMERIC,
        top_map_wins8 NUMERIC,
        top_map_losses8 NUMERIC,
        top_map9 VARCHAR(255),
        top_map_winrate9 NUMERIC,
        top_map_wins9 NUMERIC,
        top_map_losses9 NUMERIC,
        top_map10 VARCHAR(255),
        top_map_winrate10 NUMERIC,
        top_map_wins10 NUMERIC,
        top_map_losses10 NUMERIC,
        Views NUMERIC,
        rank VARCHAR(255)
        );

???+ importante

    Toda vez que você for usar nosso sistema é preciso verificar se o Docker está ligado.