<br id="topo">
 
<h1 align="center"> SPRINT 2 </h1>

<p align="center">
    <a href="#backlog">Backlog da Sprint</a> | 
    <a href="#us">User Stories e Critérios de Aceitação</a> | 
    <a href="#design">Design de Interação</a> | 
    <a href="#dados">Modelo de Dados</a> |
    <a href="#fonte">Fonte de Dados</a> |
    <a href="#entrega">Entrega</a> |
    <a href="#burndown">Burndown</a>
</p>

<span id="backlog">

  ## 🎯 Backlog da Sprint

<div align="center">
 <img src="Imagens/Backlog-2-Sprint.png">
</div>

<br>

→ [Voltar ao topo](#topo)   

<span id="us">

  ## 📑 User Stories e Critérios de Aceitação


#### US #5: Como usuário administrador desejo adicionar e excluir usuários do sistema para ter controle de quem poderá acessar os dados das red zones.

Critérios de aceitação:

 - Cenário 1: O sistema já conta com o cadastro do usuário administrador ativo 

      Dado que:
      - O usuário é responsável pela administração do sistema como um todo
      
      Quando:
      - O usuário acessa a página de cadastro de usuários
      
      Então:
      - O usuário será capaz de adicionar um novo usuário
      - O usuário administrador poderá definir qual o papel do novo usuário dentro do sistema, limitando as ações desse usuário sobre os dados do sistema


#### US #6: Como usuário administrador desejo que o sistema seja dotado de um método de autenticação para que somente pessoas autorizadas possam visualizar os registros relacionados a cada red zone

Critérios de aceitação:

 - Cenário 1: O sistema tem apenas o usuário administrador cadastrado

      Dado que:
      - O usuário é responsável pela administração do sistema como um todo
      
      Quando:  
      - O usuário acessa a página de cadastro de usuários
      
      Então:
      - O usuário será capaz de, ao adicionar um novo usuário, definir uma senha de acesso temporária para autenticá-lo no ambiente

 - Cenário 2: O usuário perdeu as suas credenciais de acesso

      Dado que:
      - O usuário precisa visualizar os dados constantes no sistema
      
      Quando:
      - O usuário acessar a página de login
      
      Então:
      - O usuário terá a opção de recuperar sua senha


#### US #7: Como usuário desejo contar com um painel com recursos visuais para facilitar a visualização e interpretação dos registros de entrada e de saída de cada red zone.

Critérios de aceitação:

 - Cenário 1: O sistema já conta com alguns registros de entrada e de saída de pessoas

      Dado que:
      - O usuário precisará visualizar os dados coletados pelo sistema de monitoramento das câmeras de segurança
      
      Quando:
      - O usuário acessar a tela inicial do sistema
      
      Então:
      - O usuário terá a opção de visualizar os dados em um painel
      - O painel conterá elementos visuais para auxiliar a interpretação dos registros de entrada e de saída capturados pela inteligência artificial a partir das imagens geradas pelas câmeras de segurança

 - Cenário 2: Ainda não há nenhum registro de entrada e de saída de pessoas no sistema

      Dado que:
      - O usuário é responsável pelo monitoramento de determinada red zone
      - A câmera de segurança dessa red zone ainda não registrou nenhuma movimentação na área
      
      Quando:
      - O usuário acessa a página de visualização em tempo real das imagens das câmeras de segurança
      
      Então:
      - O usuário pode constatar que a área segue sem movimentação de pessoas
  

#### US #8: Como usuário administrador desejo contar com uma seção específica de gerenciamento dos demais usuários que acessam o sistema para facilitar a gestão do ambiente.

Critérios de aceitação:

 - Cenário 1: O sistema conta apenas com o usuário administrador cadastrado

      Dado que:
      - O usuário administrador fará a gestão de todos os usuários dentro do sistema
      
      Quando:
      - O usuário administrador acessar a tela de gestão de usuários
      
      Então:
      - O usuário administrador visualizará uma lista de usuários ativos que contém apenas seu próprio usuário e não visualizará a opção de excluir esse usuário do sistema;
      - O usuário administrador terá a opção de adicionar novos usuários.

 - Cenário 2: O sistema conta com mais de um tipo de usuário cadastrado

      Dado que:
      - O usuário administrador é responsável pela gestão de todos os usuários dentro do sistema
      - Outros tipos de usuários já foram adicionados ao sistema
      
      Quando:
      - O usuário administrador acessar a página de gestão de usuários
      
      Então:
      - O usuário administrador poderá visualizar e editar os dados constantes do cadastro de cada um desses usuários;
      - O usuário administrador terá a opção de excluir qualquer outro usuário que não seja o seu;
      - O usuário administrador poderá adicionar novos usuários ao sistema.
  
   <br>

→ [Voltar ao topo](#topo)

<span id="design">

  ## 🎨 Design de Interação

<div align="center">
 <img src="Imagens/Login.png">
</div>

<br>

<div align="center">
 <img src="Imagens/Dashboard.png">
</div>

<br>

<div align="center">
 <img src="Imagens/Gestão-Usuários.png">
</div>

<br>

<div align="center">
 <img src="Imagens/Adicionar-Usuário.png">
</div>

<br>

<div align="center">
 <img src="Imagens/Detalhes.png">
</div>

<br>

→ [Voltar ao topo](#topo)   

<span id="dados">

  ## 📝 Modelo de Dados

<div align="center">
 <img src="Imagens/DiagramaER_2.png">
</div>

<br>

→ [Voltar ao topo](#topo)   

<span id="fonte">

 ## 📖 Fonte de Dados

  O modelo de Machine Learning criado na primeira sprint será aprimorado com imagens e vídeos produzidos pelos próprios integrantes da equipe. Durante o treinamento, também foram usadas imagens do banco público [Pexels](https://www.pexels.com/pt-br/).
  <br>
  <br>
  Esses materiais foram inicialmente associados ao conjunto de dados da biblioteca [TensorFlow](https://www.tensorflow.org/learn?hl=pt-br). Porém, ao longo da sprint, optamos por migrar para o algoritmo de detecção de objetos [YoloV8](https://docs.ultralytics.com/pt). De acordo com a documentação oficial da Ultralytics, esse algoritmo consiste em um modelo de deteção de objetos e segmentação de imagens em tempo real baseado em avanços de ponta em aprendizagem profunda e visão computacional, que oferece um desempenho de destaque em termos de velocidade e precisão.
  <br>

→ [Voltar ao topo](#topo)   

<span id="entrega">

  ## 💻 Entrega

https://github.com/peonia-api/API_6_Semestre/assets/86115352/a175e2b2-02a1-4cf2-bc20-201c1efcecea


https://github.com/peonia-api/API_6_Semestre/assets/86115352/c8d423fd-36c6-4ea6-9597-006214179a96


https://github.com/peonia-api/API_6_Semestre/assets/86115352/75feb3f5-e813-403c-b4c1-d020e18f2e5d


https://github.com/peonia-api/API_6_Semestre/assets/86115352/4086de87-3a39-4e44-b6ed-6a06b6c454ab


https://github.com/peonia-api/API_6_Semestre/assets/86115352/ae022536-0ba7-470d-a872-77c34655e644


https://github.com/peonia-api/API_6_Semestre/assets/86115352/a6ecd396-4c04-4618-9eb7-7e54d73b3ee8


https://github.com/peonia-api/API_6_Semestre/assets/86115352/656a6346-5134-4dbe-b1ed-194862e28308



→ [Voltar ao topo](#topo)   

<span id="burndown">

## 📉 Gráfico de Burndown 

<div align="center">
 <img src="Imagens/burndown-sprint02.png">
</div>

<br>

→ [Voltar ao topo](#topo)  

<h5 align="center"> Aprendizagem por Projetos Integrados - Faculdade de Tecnologia de São José dos Campos - Prof. Jessen Vidal </h5>
