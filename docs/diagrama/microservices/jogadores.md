
Esse microserviço é responsável por gerenciar as contas dos usuários do sistema que está sendo desenvolvido. Ele também pode ser utilizado como template para o desenvolvimento de outros microserviços que se utilizem de recuros semelhantes em seu funcionamento.

  1. [Endpoints](#endpoints)

## Endpoints

??? note "Create Account"

    ``` url
    POST /accounts
    ```

    Request
    ``` json
    {
        "username": "Alek",
        "tag": "#top1",
        "playtime": "300"
        ...
    }
    ```
    Response

    | code | body | 
    |--|--|
    | 201 | `{ "id": "1", "username": "Alek", "tag": "#top1" }`{:.json} |
    | 401 | | 


???+ info "Get Account"

    ```
    GET /porcen-vitoria/{uuid}
    ```
    Response

    | code | body | 
    |--|--|
    | 200 | ```{"id": "1", "username": "Alek", "matches": "250", "winPercentage": "42%" }``` |
    | 401 | | 

