# Acolhe\Material_2°Ano\DOA

Para esse projeto, foi realizado práticas DEVOPS:

Para uma colaboração entre todos os membros do grupo, foi criado a Organização "Acolhe" no GitHub com todos os integrantes. 

Nessa organização, fizemos a utilização de branches, sendo elas:
1. Entregaveis: Ambiente para avaliação de notas dos professores.
2. PROD: Ambiente em que já foi feito a validação do projeto e a parte em que o projeto é hospedado. Só é aceito PR vindos da DEV;
3. DEV: Ambiente para desenvolvedores, aonde os integrantes juntam suas partes. Só é aceito PR vindos das branches externas;
4. [Outras]: Ambiente "pessoal", 1+ integrante(s) criam a branch para a feature específica, com o objetivo de realizar o Merge em DEV.

Nessa organização, fizemos a utilização de repositórios, sendo eles:
1. Acolhe: repositório principal, armazenar submódulos e informações do escopo inteiro do projeto;
2. front-end: submódulo, parte externa/visual do projeto, App Mobile;
3. back-end: submódulo, parte interna do projeto, API Spring;
4. primeiro-ano: submódulo, repositório para o 1° ano compartilhar informações entre si;

Algumas regras e boas práticas foram implementadas nessa organização, dentre os quais se destacam:
1. Padrão de nomeação de commits seguindo a Conventional Commits;
2. Não é permitido realizar o push direto nas branches fixas (PROD/DEV), caso deseje realizar alguma implementação deve-se criar uma nova branch e realizar o PR;
3. Não é permitido realizar o PR em PROD, com exceção da DEV;
4. Os Pull-Requests precisam obrigatoriamente de 1 reviewer para autorizar o merge em DEV e 2 reviewers para PROD;
5. Foi definido 2 proprietários (owners) da Organização (André & Rafael);

Foi feita a hospedagem de todos os projetos possíveis, sendo eles:
API: https://api-acolhe.onrender.com

Foi feita pipeline, para realizar o deploy de todos os projetos em Cloud, sendo eles:
API: https://github.com/Acolhe/back-end/blob/Entregaveis/.github/workflows/deploy.yml
