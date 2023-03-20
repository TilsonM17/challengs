
# Desafio da  Enquete

Uma enquete é uma pesquisa, na qual as pessoas respondem uma pergunta escolhendo
dentre algumas alternativas pré-definidas.

**O seu objetivo é criar uma `API RESTful` para a utilização de uma enquete.**.

**NOTA:** Sinta-se avontade para recriar ele na linguagem ou framework  de sua preferencia.


## Endpoints


Os seguintes endpoints são necessários no seu projeto. Todos os endpoints
deverão ser RESTful com `Content-Type: application/json`.

 #### Get `/poll/:id` 
Deve retornar os dados de uma enquete:

    {
    "data": {
        "poll_id": 1,
        "poll_description": "Teste",
        "options": [
                {"option_id": 1,"option_description": "First option"},
                 {"option_id": 2,"option_description": "Second option"},
                 {"option_id": 3,"option_description": "Third option"},
             ]
    }
}


***Caso o id não exista no sistema, o retorno deve ser um 404 Not Found***.

---

#### Post  `/poll`
Deve criar uma nova enquete.

    {
       
        "poll_description": "Voçe é bonito?" 
        "options": [
             "Sim"
             "Não"
             "Talvez"
             ]
    }

E o retorno:

       {
        "poll_id": 103,
       }

---

#### Post `/poll/:id/vote/:id` 

Deve registrar um novo voto para uma opção.

     {
        "poll_id": 1,
     }


**Caso o id não exista no sistema, o retorno deverá ser um 404 Not Found.**

---

#### Get `/poll/:id/stats`


Vai retornar estatísticas sobre a enquete. As views de uma enquete devem ser
incrementadas sempre que uma requisição `Get /poll/:id` seja feita.
    
    {
        "views": 125    
        "votes": [
            {"option_id": 1,"qty": 10},
            {"option_id": 2,"qty": 25},
            {"option_id": 3,"qty": 1},
             ]
    }
