<div class="semestre4">

<div align=center>
<h1>B1NARY INSPECT</h1>
</div>

<h4> 4º Semestre • <a href="https://github.com/B1nary-Devs/JAIA-SOFTWARE">Repositório Github</a></h4>
<p align="justify"> Empresa Parceira • <a href="https://jaia.software/blog/">Jaia Software</a></p>

<p align="center"><img src="https://github.com/B1nary-Devs/JAIA-SOFTWARE/assets/102266928/9a081b92-bb7d-4a3f-8b88-f1e68f69848e" widht="20%"></img>

<p align="justify"> A B1 Inspec é uma solução completa para controle e reporte de anomalias detectadas em Laudos de Inspeção Predial. O sistema oferece funcionalidades essenciais, incluindo segmentação precisa de áreas específicas do edifício, cadastro de prestadores de serviço, geração ágil de ordens de serviço e criação de relatórios detalhados, otimizando a gestão e a manutenção predial.</p>

<h2> <a name="Objetivo">Visão do Projeto</a> </h2>

<div align=center>
  
![Publicação _ LinkedIn - Opera 2024-11-21 15-36-47](https://github.com/user-attachments/assets/b8984f6c-0686-4cac-86f6-02d8c5d5fef8)

</div>

<br>

<h2> <a name="Objetivo">Objetivo</a> </h2>

* O sistema realiza a emissão de laudos técnicos prediais, fornecendo análises detalhadas e precisas sobre as condições das estruturas.
* O sistema automatiza tarefas administrativas, agilizando a gestão de contratos empresariais e reduzindo o tempo necessário para cada processo.
* O cliente recebe automaticamente por e-mail os resultados de seus laudos, garantindo praticidade e rapidez na obtenção das informações.
  
<br>

<h2>Tecnologias Utilizadas no Projeto</h2>

<p align="justify"> <strong>Java 14:</strong> linguagem para desenvolvimento da aplicação para back-end.</p>
<p align="justify"> <strong>TypeScript:</strong> linguagem para desenvolvimento da aplicação para front-end.</p>
<p align="justify"> <strong>Vue JS:</strong> Framework de desenvolvimento de interfaces de usuário e aplicativos de página única.</p>
<p align="justify"> <strong>Spring Boot:</strong> Framework Java de desenvolvimento de aplicações Spring, proporcionando configuração automática e um ambiente de execução standalone.</p>


![Vue.js](https://img.shields.io/badge/vuejs-%2335495e.svg?style=for-the-badge&logo=vuedotjs&logoColor=%234FC08D) ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
  
<br>
  
<h2>Minhas Contribuições</h2>

 > Contribuí ativamente como desenvolvedor front-end na construção da arquitetura e design da aplicação, colaborando com a equipe para criar uma estrutura escalável e eficiente.

## 1. **Criação de componentes**
   - Contribuí ativamente com o desenvolvimento de componentes de interface, focando na criação de elementos visuais interativos e responsivos.

<details>
  <summary>Detalhes</summary>

  ~~~~typescript
# Criação do componente popUp quando determinada ação ou processo é finalizada

<template>
    <div v-if="showPopup" class="cover"></div>
    <div class="card" :class="{ active: showPopup }">
        <button @click="ocultarPopup" class="dismiss" type="button">×</button>
        <div class="header">
            <div class="image">
                <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                    <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
                    <g id="SVGRepo_iconCarrier">
                        <path d="M20 7L9.00004 18L3.99994 13" stroke="#000000" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round"></path>
                    </g>
                </svg>
            </div>
            <div class="content">
                <span class="title">{{ title }}</span>
                <p class="message">{{ mensagem }}</p>
            </div>
        </div>
    </div>
</template>
~~~~
  
</details>

## 2. **Criação de Views**
   - Contribuí ativamente com o desenvolvimento de diversas páginas de renderização, garantindo que os formulários e layouts fossem responsivos e de fácil navegação.

<details>
  <summary>Detalhes</summary>

  ~~~~typescript
# Formulário de cadastro de prestador
<template>
  <div class="form-cadastro">
      <div class="form-title">
          <h1>Prestador de Serviço</h1>
          <span>> Cadastro</span>
      </div>
      <div class="form-body">
          <div class="input-group">
              <div class="input-box">
                  <label for="id_nome">Nome</label>
                  <input type="text" id="id_nome" v-model="nome" placeholder="Ex: Encanador">
              </div>

              <div class="input-box">
                  <label for="id_cnpj">CNPJ</label>
                  <input type="number" id="id_cnpj" v-model="cnpj" placeholder="00.000.000/0000-00">
              </div>

              <div class="input-box">
                <label for="id_categoria">Segmento</label>
                <select id="id_categoria" v-model="categoriaSelecionada">
                  <option v-for="ctg in categoria" :key="ctg.id" :value="ctg.id">{{ ctg.nome }}</option>
                </select>
              </div>

              <div class="input-box">
                  <label for="id_email">Email</label>
                  <input type="email" id="id_email" v-model="email" placeholder="Ex: joao@gmail.com">
              </div>

              <div class="input-box">
                  <label for="id_senha">Senha</label>
                  <input v-model="senha" type="password" id="id_senha">
              </div>
          </div>

          <div class="form-submit">
                  <button @click="returnarPag" class="button-return">Voltar</button>
                  <button @click="cadastrarPrestador">Cadastrar</button>
          </div>

      </div>

      <div class="form-footer">
          <p>© B1naryInspec | V.01</p>
      </div>
  </div>
  <ThePopUp></ThePopUp>
</template>

<script setup lang="ts">

import { onMounted, ref } from 'vue';
import ThePopUp from '../components/ThePopUp.vue';
import {exibirPopup} from '../components/ThePopUp.vue'
import axios from 'axios';

 // Capturando os valores dos campos
const categoria = ref([]);
const erro = ref();
const nome = ref("");
const cnpj = ref("");
const email = ref("");
const senha = ref("");
const token = localStorage.getItem('token')

~~~~
  
</details>

## 3. **Criação e configuração de rotas**
   - Contribuí ativamente com o desenvolvimento de rotas de navegação da aplicação front-end.

<details>
  <summary>Detalhes</summary>

  ~~~~typescript
const router = createRouter({
  history: createWebHistory(import.meta.env.BASE_URL),
  routes: [
    {
      path: '/',
      name: 'home',
      component: HomeView
    },
    {
      path: '/login',
      name: 'login',
      component: () => import('../views/Login.vue'),
      beforeEnter (_, __, next) { // Impede usuários não assinados
        if (!verifyTokenAcesso()) {       // de acessar a página Home.
          next();
          return;
        }
        next('/')
      }
    },
...
~~~~

</details>

## 4. **Requisições REST**
   - Contribuí com o desenvolvimento de requisições REST da aplicação.

<details>
  <summary>Detalhes</summary>

~~~~typescript
async function cadastrarPrestador() {
  // Verifique se uma categoria foi selecionada
  if (categoriaSelecionada.value === null) {
    alert('Selecione uma categoria antes de cadastrar.');
    return;
  }
    var usuarioId = await cadastrarUsuario();
  
  // Fazendo a requisição POST com os valores capturados
  try {
    
    await axios.post('http://localhost:8080/prestador', {
  
      prestadorNome: nome.value,
      cnpj: cnpj.value,
      usuarioId: usuarioId,
      segmentoId: categoriaSelecionada.value
  
    }, 
    {
      headers: {
          'Authorization': `Bearer ${token}` 
        }
    }
    );
    
    enviarEmailCredenciais(email.value, senha.value);
  
    // Requisição bem-sucedida, exibir um alerta de confirmação
    exibirPopup('Cadastro Realizado com Sucesso', 'Novo Prestador Registrado.', 123)
    limparCampos();
  
    
  } catch (error) {
    console.error('Ocorreu um erro ao cadastrar o prestador:', error);
    alert('Erro ao cadastrar o prestador.');
  }
}
~~~~

</details>

<h2>Conhecimentos Obtidos</h2>
<p align="justify">
  No quarto semestre, tive meu primeiro contato com o front-end avançado, especialmente na criação de componentes, o que foi uma experiência transformadora para mim. Esse aprendizado permitiu que eu entendesse melhor a modularidade e a reutilização de código, conceitos essenciais para construir interfaces escaláveis e organizadas.
</p>


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
      <td>Typescript</td>
      <td>Sei fazer com Ajuda</td>
    </tr>
    <tr>
      <td>VueJS</td>
      <td>Sei fazer com Ajuda</td>
    </tr>
  </table>
</details>
<h3>Soft Skills </h3>
<details>
<summary><b>Clique para ver a lista de soft skills</b></summary>
  <br>
  <table align="center" border="1" cellspacing="0" cellpadding="8">
    <tr>
      <th width="300px" style="background-color: #dce6f1;">Habilidade</th>
      <th width="300px" style="background-color: #dce6f1;">Descrição</th>
    </tr>
    <tr>
      <td style="background-color: #f2f2f2;">Gestão de Tempo</td>
      <td>Durante os projetos, precisei gerenciar e priorizar tarefas de forma eficaz para cumprir prazos e garantir a produtividade da equipe.</td>
    </tr>
    <tr>
      <td style="background-color: #f2f2f2;">Resolução de Problemas</td>
      <td>Fui desafiado a resolver problemas técnicos e operacionais de maneira criativa, buscando sempre a melhor solução para o andamento do projeto.</td>
    </tr>
    <tr>
      <td style="background-color: #f2f2f2;">Trabalho em Equipe</td>
      <td>Colaborei ativamente com a equipe, garantindo comunicação aberta e eficiente para alcançar os objetivos comuns.</td>
    </tr>
    <tr>
      <td style="background-color: #f2f2f2;">Aprendizagem Contínua</td>
      <td>Estive sempre disposto a aprender novas tecnologias e aprimorar minhas habilidades para me adaptar às demandas do projeto.</td>
    </tr>
</table>

</details>

-------------------
[RETORNAR A PÁGINA PRINCIPAL](https://github.com/WallaceHS20/PORTFOLIO_FATEC)  
