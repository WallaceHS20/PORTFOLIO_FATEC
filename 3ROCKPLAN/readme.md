<div class="semestre3">

<div align=center>
<h1>ROCK PLANNING</h1>
</div>
  
<h4> 3º Semestre • <a href="https://github.com/B1nary-Devs/DOM-ROCK">Repositório Github</a></h4>
<p align="justify"> Empresa Parceira • <a href="https://www.domrock.net/">DOM ROCK</a></p>

<p align="center"><img src="https://github.com/WallaceHS20/Bertoti---Engenharia-de-Software/assets/101594950/cede74e7-daaa-454b-ba81-e2775b8713a1" widht="20%"></img>

<p align="justify"> A Rock Planning é uma aplicação web que visa gerenciar as vendas, considerando o histórico do vendedor, o planejamento e as vendas realizadas. Deverá apresentar um comparativo dos dados mencionados anteriormente para que possam ser analisados de forma precisa e detalhada. Além disso, a aplicação será aprimorada com a adição de uma predição gerada por um algoritmo de Inteligência Artificial pré-existente, a fim de proporcionar maior precisão e confiabilidade.</p>

<br>

<details>

<summary align=center> VER MAIS DETALHES :information_source: </summary>

<h2> <a name="Objetivo">Objetivo</a> </h2>

#### Após a finalização do projeto pela equipe B1naryDevs:
* O Administrador é capaz de cadastrar vendedores e a carteira de clientes;
* O Vendedor conseguirá planejar as vendas para seus clientes;
* O Administrador conseguirá monitorar as vendas de todos os vendedores através de um Dashboard;
* O Vendedor conseguirá monitorar suas respectivas vendas através de um dashboard.

<br>

<h2>Tecnologias Utilizadas no Projeto</h2>

<p align="justify"> <strong>Java SE 14:</strong> linguagem para desenvolvimento da aplicação para front-end e back-end.</p>
<p align="justify"><strong>MSQL:</strong> SGBD para desenvolvimento do Banco de Dados.</p>
<p align="justify"><strong>Spring Boot 3:</strong> Framework web responsável pelo gerenciamento de microsserviços. 

<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white" target="_blank"><img src="https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white" target="_blank"><img src="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white">

<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" target="_blank"><img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" target="_blank"><img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" target="_blank"><img src="https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white" target="_blank"><img src="https://img.shields.io/badge/IntelliJ_IDEA-000000.svg?style=for-the-badge&logo=intellij-idea&logoColor=white" target="_blank">

  
<br>
  
<h3>Minhas Contribuições</h3>
  
> Contribuí ativamente como desenvolvedor front-end, desempenhando um papel crucial na arquitetura e estilização das páginas. Minhas contribuições incluíram:

<br>

## 1. **Arquitetura HTML:**
   - Colaborei com a arquitetura e estruturações da página, garantindo a escalabilidade e modularidade do código com HTML.

<details>
<summary>Detalhes</summary>
  
  ~~~~HTML
<!-- Tabela de vendedores com classes para estilização e identificador único para manipulação via scripts -->
<table class="table" id="tabelaVendedores">
  <!-- Cabeçalho da tabela definindo as colunas disponíveis -->
  <thead>
    <tr>
      <th scope="col">ID</th>
      <th scope="col">Nome</th>
      <th scope="col">E-mail</th>
      <th scope="col">Editar</th>
      <th scope="col">Detalhes</th>
    </tr>
  </thead>
  <!-- O corpo da tabela é intencionalmente omitido aqui, provavelmente será preenchido dinamicamente com dados dos vendedores -->
</table>
~~~~

</details>

<br>

## 2. **Estilização de Páginas:**
   - Contribuí para a estilização de páginas, seguindo as melhores práticas de design e garantindo uma interface de usuário atraente e intuitiva.

<details>

<summary>Detalhes</summary>

~~~~CSS
/* Estilo geral para todas as tabelas, definindo largura, colapso de borda para evitar espaços duplos, cor da borda, e centralização na página */
table {
    width: 80%;
    border-collapse: collapse;
    border: 1px solid #bdc3c7;
    margin: auto;
}

/* Estilo para linhas da tabela para melhorar a interação do usuário, com uma transição suave para hover e cursor de ponteiro para indicar clicabilidade */
tr {
    transition: all .2s ease-in;
    cursor: pointer;
}

/* Estilo para células e cabeçalhos de tabela, definindo o espaçamento interno, alinhamento do texto e borda inferior para separar as linhas */
th, td {
    padding: 12px;
    text-align: left;
    border-bottom: 1px solid #ddd;
}

/* Efeito hover para linhas da tabela, com mudança de cor de fundo, leve aumento de escala e sombra para destacar a linha atual sob o mouse */
tr:hover {
    background-color: #f5f5f5;
    transform: scale(1.02);
    box-shadow: 2px 2px 12px rgba(0, 0, 0, 0.2), -1px -1px 8px rgba(0, 0, 0, 0.2);
}

/* Estilo específico para células e cabeçalhos da tabela com a classe 'table', definindo fonte, cor da borda e do texto, tamanho da fonte, alinhamento do texto e espaçamento interno */
.table td, .table th {
    font-family: Arial, Helvetica, sans-serif;
    border-bottom: 1px solid #000000;
    color: #000000;
    font-size: 16px;
    text-align: center;
    padding: 12px 12px; 
}

/* Estilo adicional para cabeçalhos da tabela, definindo cor de fundo, sombra da caixa, cor do texto e peso da fonte para um destaque visual claro */
.table th {
    background-color: #1842ca;
    color: #ffffff;
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
    color: white; 
    font-weight: bold; 
}
~~~~

</details>

<br>

## 3. **Requisições REST:**
   - Colaborei no desenvolvimento de funções dedicadas para realizar requisições, garantindo a integridade e usabilidade dos dados transmitidos e recebidos.

<details>

<summary>Detalhes</summary>

~~~JavaScript

// Esta função realiza uma requisição GET para nossa API Spring Boot e atualiza o valor da constante vendedores

async function buscarVendedores() {
    try {

        /* Utilizando a biblioteca axios para realizar uma requisição GET para a URL especificada que representa um
         um endpoint da nossa API Spring Boot que retorna os dados dos vendedores. */
        
        const response = await axios.get("http://localhost:8080/vendedor");

        // Atribuindo o resultado a constante vendedores
        // A propriedade .data é usada para acessar os dados da resposta (response)
        vendedores.value = resposta.data;

    } catch (ex) {

        // Em caso de erro, exibe um alerta indicando que algo deu errado
        alert('Ocorreu uma falha!');

        // A mensagem de erro é obtida através da propriedade .message do objeto de exceção (ex)
        erro.value = (ex as Error).message;
    }
}

~~~

</details>
  
<br>

> Durante o desenvolvimento do projeto, desempenhei o papel de Scrum Master, assumindo responsabilidades cruciais para garantir a eficiência e qualidade do trabalho da equipe. Como Scrum Master, minhas principais atribuições incluíram:

<br>

## 4. **Elaboração de Tasks e User Stories:**
   - Colaborei ativamente com a equipe na definição e elaboração de tarefas e histórias de usuário.
   - Garanti que as User Stories fossem claras, compreensíveis e atendessem aos critérios de aceitação.

## 5. **Gestão da Produtividade:**
   - Implementei práticas ágeis para melhorar a eficiência da equipe.
   - Removi obstáculos que prejudicavam o progresso da equipe, promovendo um ambiente de trabalho livre de obstáculos.
   - Mantive uma comunicação transparente entre os membros da equipe, promovendo a colaboração e o entendimento mútuo.

<br>

<details>
  <summary>Detalhes</summary>

<img width="907" alt="Captura de tela 2023-09-27 194721" src="https://github.com/WallaceHS20/Bertoti---Engenharia-de-Software/assets/101594950/2d7745b4-4556-497b-abd1-ea40c6b91009">
    
</details>

<br> <br>

<h2>Conhecimentos Obtidos</h2>
<p align="justify">Essa experiência multifacetada me proporcionou uma compreensão abrangente do ciclo de vida do desenvolvimento de software, desde a gestão ágil até a implementação eficaz no front-end. Estou comprometido em continuar trazendo meu conjunto diversificado de habilidades para projetos futuros.</p>
<h3>Hard Skills </h3>
<details>
  <summary><b>Clique para ver a lista de hard skills</b></summary>
  <br>
  <table align="center">
    <tr>
      <th width="300px">Tecnologia/Metodologia</th>
      <th width="300px">Classificação</th>
    </tr>
    <tr>
      <td>Java</td>
      <td>★★★☆☆☆</td>
    </tr>
    <tr>
      <td>HTML</td>
      <td>★★★★★☆</td>
    </tr>
        <tr>
      <td>CSS</td>
      <td>★★★★★☆</td>
    </tr>
        <tr>
      <td>JavaScript</td>
      <td>★★★☆☆☆</td>
    </tr>
    <tr>
      <td>MySQL</td>
      <td>★★★☆☆☆</td>
    </tr>
  </table>
</details>
<h3>Soft Skills </h3>
<details>
<summary><b>Clique para ver a lista de soft skills</b></summary>
  <br>
  <table align="center">
    <tr>
      <th width="300px">Habilidade</th>
      <th width="300px">Classificação</th>
    </tr>
    <tr>
      <td>Proatividade</td>
      <td>★★★☆☆☆</td>
    </tr>
    <tr>
      <td>Visão de Negócio</td>
      <td>★★☆☆☆☆</td>
    </tr>
    <tr>
      <td>Comunicação</td>
      <td>★★★★☆☆</td>
    </tr>
    <tr>
      <td>Empatia</td>
      <td>★★★★★☆</td>
    </tr>
    <tr>
      <td>Organização e Planejamento</td>
      <td>★★★★☆☆</td
    </tr>
  </table>
</details>
</summary>
</details>
