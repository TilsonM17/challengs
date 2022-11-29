## Teste do Filme

Descrição:

Sou uma empresa de aluguel de streaming de filmes e séries, desejo um sistema no qual o usuário possa buscar um filme ou série e poder alugá-lo por 48 horas. Preciso de uma tela em /admin com listagem desse aluguel (não precisa de autenticação, caso queira fazer uma tela de login pode inserir a senha fixa no código se desejar)

Fluxo de navegação:
- Acessar a home e ter um campo de busca somente para buscar filme e série
- Digito o nome que desejo e clico em buscar
- Lista o que encontrou com foto do filme, nome, resumo e ano de lançamento, cambo de busca fica no topo da listagem caso queira buscar novamente.
- Se encontrar muitos resultados a página terá que ter paginação ou infinite scroll (recurso não obrigatório, somente se tiver tempo)
- Junto com cada filme terá um botão Alugar
- Clicando em alugar irá para uma nova página onde no topo mostre o nome do filme e capa que estou alugando e um form para digitar nome e email e um botão para confirmar o aluguel ou voltar.
- Como administrador quero acessar /admin e ver a listagem de todos os aluguéis, com a data de quando foi alugado e a expiração em 48 hrs, a listagem deverá exibir dados do filme e quem alugou. Deverá também estar em ordem decrescente de aluguel.

Definições tecnicas
- Deverá usar essa API: https://www.themoviedb.org/documentation/api?language=pt-BR
- Backend deverá ser em PHP, pode usar qualquer framework.
- Terá que ter o README de como rodar o projeto localmente e caso tenha testes automatizados de como rodá-lo.
- Deverá criar um repositório no github de forma privada e colocar o meu usuario como maintainer (edmargomes), o repositório poderá ficar publico após a entrega se desejar.
- Deverá ter no mínimo 1 branch para cada item do fluxo de navegação acima, você pode ter mais branchs para outras funcionalidades ou mais de 1 para a mesma funcionalidade, mas não menos que 1 para cada item citado em Fluxo de navegação
- Deverá abrir um PR para cada branch para o main e me enviar o link para review
Caso o branch seguinte dependa do anterior, informar no PR que um depende do outro
Caso o branch não tenha dependência ele deverá ser criado diretamente a partir do main.
Ideal que você envie os avanços todos os dias com PR para já podermos ir revisando e dando feedback. Caso deixe para a última hora poderá não ter tempo hábil para fazer alterações.

