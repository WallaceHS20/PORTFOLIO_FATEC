<div class="semestre4">

<div align=center>
<h1>B1NARY CREDI</h1>
</div>

<h4> 5º Semestre • <a href="https://github.com/B1nary-Devs/Tecsus">Repositório Github</a></h4>
<p align="justify"> Empresa Parceira • <a href="https://jaia.software/blog/">SPC GRAFENO</a></p>

<p align="center"><img src="https://github.com/user-attachments/assets/e15dc96e-eaf5-4311-ab25-e5d281bcf1f6" widht="20%"></img>

<p align="justify"> Binary Credi é um sistema inovador de pontuação e painel para ativos financeiros. Utilizamos IA e aprendizagem de máquina para identificar duplicatas fraudulentas, garantindo maior segurança e eficiência operacional. Nossa plataforma fornece insights visuais valiosos que capacitam a tomada de decisões informadas, beneficiando tanto as instituições financeiras quanto seus clientes.</p></p>

<h2> <a name="Objetivo">Visão do Projeto</a> </h2>

<div align=center>
  
![B1nary-Devs-Opera-2024-11-21-16-02-10](https://github.com/user-attachments/assets/aa3a7e4e-cacb-47bd-b7ac-cccfd32cb020)

</div>

<br>

<h2> <a name="Objetivo">Objetivo</a> </h2>

#### Após a finalização do projeto pela equipe B1naryDevs:

* O sistema possibilitou a gestão de perfis de utilizadores com controlo de acesso diferenciado, garantindo segurança e personalização de permissões para Administradores e Cessionárias.  
* O sistema ofereceu funcionalidades CRUD completas para Cessionárias, permitindo o gerenciamento eficaz de dados e relacionamentos no processo financeiro.  
* A Cessionária acompanhou faturas futuras, vencidas e concluídas, além de informações detalhadas sobre os Sacados associados.  
* O sistema forneceu uma funcionalidade de visualização de Locais de Pagamento exclusiva para o Administrador, centralizando a gestão dessas informações.  
* O sistema produziu relatórios mensais de conciliação financeira, complementados com previsões baseadas em dados históricos, otimizando o planejamento e a tomada de decisão estratégica nas operações financeiras.  
 
<br>

<h2>Tecnologias Utilizadas no Projeto</h2>

<p align="justify"><strong>Python 3:</strong> linguagem utilizada para o desenvolvimento da aplicação back-end.</p>
<p align="justify"><strong>Flask:</strong> framework utilizado para construir APIs RESTful e gerenciar a lógica do back-end.</p>
<p align="justify"><strong>JavaScript:</strong> linguagem para desenvolvimento da aplicação front-end.</p>
<p align="justify"><strong>ReactJS:</strong> biblioteca utilizada para criar interfaces de usuário e aplicativos de página única.</p>
<p align="justify"><strong>Redux:</strong> biblioteca usada para gerenciar o estado global da aplicação de forma eficiente.</p>

![Python](https://img.shields.io/badge/python-%233776AB.svg?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/flask-%23000000.svg?style=for-the-badge&logo=flask&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black)
![ReactJS](https://img.shields.io/badge/react-%2361DAFB.svg?style=for-the-badge&logo=react&logoColor=black)
![Redux](https://img.shields.io/badge/redux-%23764ABC.svg?style=for-the-badge&logo=redux&logoColor=white)


  
<br>
  
<h2>Minhas Contribuições</h2>

 > Desempenhei um papel essencial como desenvolvedor front-end, participando do planejamento e implementação da arquitetura e do design da aplicação. Trabalhei em conjunto com a equipe para desenvolver uma estrutura eficiente e com alta capacidade de escalabilidade.

## 1. **Criação de componentes genéricos**
   - Participei diretamente na construção de componentes de interface, priorizando a criação de elementos visuais dinâmicos, adaptáveis a diferentes dispositivos e projetados para uso múltiplo.

<details>
  <summary>Detalhes</summary>

  ~~~~javascript
# Criação do componente SearchInput que recebe um texto e uma função e realiza o filtro de tabelas em seu componente pai

// Importação das dependências necessárias
import * as React from 'react';
import Paper from '@mui/material/Paper'; // Contêiner estilizado do Material-UI
import InputBase from '@mui/material/InputBase'; // Campo de entrada minimalista e customizável
import IconButton from '@mui/material/IconButton'; // Botão interativo
import SearchIcon from '@mui/icons-material/Search'; // Ícone de busca

// Componente funcional que renderiza um campo de busca com ícone
export default function SearchInput({ value, onChange }) {
  return (
    <Paper
      component="form" 
      sx={{ p: '2px 4px', display: 'flex', alignItems: 'center', width: 280 }} // Estilos aplicados ao Paper
    >
      <InputBase
        sx={{ ml: 1, flex: 1 }}
        placeholder="Procurar" // Texto exibido quando o campo está vazio
        inputProps={{ 'aria-label': 'Procurar' }} // Propriedade para acessibilidade
        value={value} // Liga o valor do campo de busca ao estado externo
        onChange={onChange} // Executa a função fornecida ao alterar o texto
      />
      <IconButton
        type="button"
        sx={{ p: '10px' }} // Espaçamento interno para dimensionar o botão
        aria-label="search" // Rotulagem para leitores de tela
      >
        <SearchIcon /> {/* Ícone que representa a ação de busca */}
      </IconButton>
    </Paper>
  );
}

~~~~
  
</details>

## 2. **MUI (Material-UI)**  
   - Implementação de componentes prontos para acelerar o processo de desenvolvimento, garantindo consistência no design e alta personalização.

<details>
  <summary>Detalhes</summary>

~~~~javascript
// Este botão exibe a funcionalidade "Não aceitar" de um modal de termos e condições de uso com um estilo personalizado e interações visuais.

import { Button } from '@mui/material';
<Button
    variant="contained" // Estilo predefinido de botão preenchido
    onClick={notAccept} // Função executada ao clicar no botão
    sx={{
        backgroundColor: '#818181', // Cor inicial do botão
        color: 'white', // Cor do texto do botão
        '&:hover': { 
            backgroundColor: '#555555', // Cor ao passar o mouse sobre o botão
        },
        marginRight: 2, // Espaçamento à direita do botão
    }}
>
    Não aceitar
</Button>
~~~~

</details>


## 3. **React Hoock Forms**  
   - Integração do framework `react-hook-form` para validação de formulários com precisão e performance, simplificando o gerenciamento de estados e validações.

<details>
  <summary>Detalhes</summary>

~~~~javascript
// Abaixo está a implementação de um campo de entrada de e-mail com validação integrada utilizando o `react-hook-form`.

import { Button } from '@mui/material';
<TextField
    {...register('email', { // Registra o campo no react-hook-form
        required: 'E-mail é obrigatório', // Mensagem de erro caso o campo esteja vazio
        pattern: { 
            value: /^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/, // Regex para validar o formato de e-mail
            message: 'Formato de e-mail inválido', // Mensagem de erro caso o formato seja inválido
        },
    })}
    error={!!errors.email} // Exibe erro visual caso o campo de e-mail tenha erro
    helperText={errors.email ? errors.email.message : ''} // Mensagem auxiliar exibida abaixo do campo
    label="E-mail" // Rotulo do campo
    fullWidth // Define que o campo ocupa 100% da largura disponível
    margin="normal" // Adiciona espaçamento padrão
    slotProps={{
        input: {
            startAdornment: (
                <InputAdornment position='start'> {/* Adiciona um ícone no início do campo */}
                    <EmailIcon
                        sx={{
                            color: errors.senha ? 'var(--color-error)' : 'inherit', // Muda a cor do ícone caso haja erro
                        }} 
                    />
                </InputAdornment>
            ),
            style: {
                padding: '5px', // Estilo de espaçamento interno do campo
            },
        },
    }}
/>
~~~~

</details>

## 4. **Redux**  
   - Utilização do Redux para gerenciamento centralizado do estado da aplicação, proporcionando maior controle e previsibilidade das interações.

<details>
  <summary>Detalhes</summary>

~~~~javascript
// Define um slice para gerenciar o estado do usuário

export const userSlice = createSlice({
    name: 'user', // Nome do slice, usado para gerar automaticamente as actions e os types
    initialState, // Estado inicial do slice, que deve ser previamente definido
    reducers: { // Conjunto de funções redutoras que modificam o estado
        logoutUser: (state) => { // Função para realizar o logout do usuário
            state.user = null; // Limpa os dados do usuário no estado
            state.status = 'idle'; // Redefine o status para "idle"
            localStorage.removeItem('UserData'); // Remove os dados do usuário do localStorage
        },
    },
});
~~~~

</details>

<h2>Conhecimentos Obtidos</h2>
<p align="justify">
Durante meu projeto do 6° Semestre, desenvolvi habilidades significativas em diversas áreas essenciais para o desenvolvimento de software. A utilização do <strong>React Hook Forms</strong> aprimorou minha capacidade de validar formulários de forma precisa e performática, garantindo uma experiência do usuário confiável e fluida. Trabalhar com o <strong>Material-UI</strong> me proporcionou conhecimentos avançados na utilização de componentes prontos e estilização personalizada, acelerando o desenvolvimento e garantindo consistência no design. Além disso, aprofundei meu entendimento na criação de <strong>componentes genéricos reutilizáveis</strong>, otimizando o desenvolvimento do front-end com maior escalabilidade.  
Também desenvolvi uma forte expertise no uso do <strong>Redux</strong> para gerenciar estados complexos de maneira centralizada, assegurando previsibilidade e facilidade na manutenção.
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
        <td>JavaScript</td>
        <td>Sei fazer com Ajuda</td>
    </tr>
    <tr>
        <td>React</td>
        <td>Sei fazer com Ajuda</td>
    </tr>
    <tr>
        <td>Redux</td>
        <td>Sei fazer com Ajuda</td>
    </tr>
    <tr>
        <td>Material-UI (MUI)</td>
        <td>Sei fazer com Ajuda</td>
    </tr>
    <tr>
        <td>React Hook Forms</td>
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
        <td style="background-color: #f2f2f2;">Pensamento Analítico</td>
        <td>Capacidade de decompor problemas complexos de desenvolvimento em partes menores e manejáveis, identificando soluções eficazes.</td>
    </tr>
    <tr>
        <td style="background-color: #f2f2f2;">Comunicação Técnica</td>
        <td>Habilidade de explicar conceitos técnicos de maneira clara e acessível, facilitando a colaboração entre membros da equipe.</td>
    </tr>
    <tr>
        <td style="background-color: #f2f2f2;">Atenção aos Detalhes</td>
        <td>Foco em garantir que o código seja limpo, eficiente e esteja em conformidade com as melhores práticas de desenvolvimento.</td>
    </tr>
    <tr>
        <td style="background-color: #f2f2f2;">Colaboração em Equipe</td>
        <td>Trabalho efetivo com colegas, integrando ideias e conhecimentos para alcançar os objetivos de desenvolvimento de software.</td>
    </tr>
    <tr>
        <td style="background-color: #f2f2f2;">Adaptabilidade</td>
        <td>Capacidade de aprender rapidamente novas tecnologias e ferramentas, respondendo às mudanças nos requisitos do projeto.</td>
    </tr>
</table>


</details>

-------------------
[RETORNAR A PÁGINA PRINCIPAL](https://github.com/WallaceHS20/PORTFOLIO_FATEC)
