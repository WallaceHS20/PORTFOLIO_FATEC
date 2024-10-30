<div class="semestre4">

<div align=center>
<h1>B1NARY TECSUS</h1>
</div>

<h4> 5º Semestre • <a href="https://github.com/B1nary-Devs/Tecsus">Repositório Github</a></h4>
<p align="justify"> Empresa Parceira • <a href="https://jaia.software/blog/">TECSUS</a></p>

<p align="center"><img src="https://github.com/user-attachments/assets/caf66ca0-9d6c-4d57-a555-887bdf05cdb2" widht="20%"></img>

<p align="justify"> A B1nary Tecsus é um sistema de análise e exibição dos dados de faturas de energia, água e gás que inclui a tratativa dos dados para garantir integridade e consistência das informações dos contratos e contas. Adicionalmente com o desenvolvimento de um dashboard interativo que permitirá métricas detalhadas, acompanhamento dos contratos, e aplicação de filtros específicos para análises precisas. A ferramenta também oferecerá relatórios detalhados de consumo em diferentes períodos, ajudando a identificar padrões e apoiar decisões estratégicas. Além disso, serão incluídos alertas automáticos para detectar consumo acima da média, identificando anomalias e oportunidades de otimização.</p></p>

  <h2> <a name="Objetivo">Objetivo</a> </h2>

#### Após a finalização do projeto pela equipe B1naryDevs:
* O sistema analisará dados de consumo de energia, água e gás, garantindo a integridade das informações.
* O sistema fornecerá um dashboard interativo para o cliente acompanhar métricas de consumo, aplicar filtros e gerenciar contratos de forma eficaz.
* O sistema gerará relatórios detalhados para ajudar o cliente a identificar padrões de consumo e tomar decisões estratégicas.
* O cliente receberá alertas automáticos por e-mail sobre consumo anômalo e oportunidades de otimização.
  
<br>

<h2>Tecnologias Utilizadas no Projeto</h2>

<p align="justify"> <strong>Python 3:</strong> linguagem para desenvolvimento da aplicação para back-end.</p>
<p align="justify"> <strong>JavaScript:</strong> linguagem para desenvolvimento da aplicação para front-end.</p>
<p align="justify"> <strong>React:</strong> Framework de desenvolvimento de interfaces de usuário e aplicativos de página única.</p>
<p align="justify"> <strong>Power BI:</strong> Ferramenta de Business Intelligence que permite criar relatórios e dashboards interativos, proporcionando insights valiosos e uma melhor compreensão dos dados.</p>

![Python](https://img.shields.io/badge/python-%233776AB.svg?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/react-%2361DAFB.svg?style=for-the-badge&logo=react&logoColor=black)
![Power BI](https://img.shields.io/badge/powerbi-%23F2C811.svg?style=for-the-badge&logo=powerbi&logoColor=black)

  
<br>
  
<h3>Minhas Contribuições</h3>

 > Contribuí ativamente como desenvolvedor front-end na construção da arquitetura e design da aplicação, colaborando com a equipe para criar uma estrutura escalável e eficiente.

## 1. **Criação de componentes genéricos**
   - Contribuí ativamente com o desenvolvimento de componentes de interface, focando na criação de elementos visuais interativos e responsivos além de serem reutilizáveis.

<details>
  <summary>Detalhes</summary>

  ~~~~javascript
# Criação do componente Title que recebe um texto e um elemento HTML filho

import './title.css'

export default function Title({children, name}){
    return(
        <div className='title' data-testid="title">
            {children}
            <span>{name}</span>
        </div>
    )   
}
~~~~
  
</details>

## 2. **Testes de Unidade**
   - Contribuí ativamente no desenvolvimento de testes de unidade para o client side, garantindo a qualidade e a confiabilidade das funcionalidades implementadas.

<details>
  <summary>Detalhes</summary>

~~~~javascript
// SUITE A SEGUIR IRÁ PERCORRER A COLEÇÃO DE TESTES UNITÁRIOS PERTENCENTES A PÁGINA DE AUTENTICAÇÃO
describe('SUITE DE TESTES DA FUNCAO LOGIN', () => {

    beforeEach(() => {
        render(<Router><Login /></Router>);
    });

    it('isNull_fieldsNull_Expect_toastErrorFieldsNull', () => {

        // CAPTURANDO O BOTÃO
        const buttonLogin = screen.getByTestId('buttonLogin');

        // DISPARANDO A FUNÇÃO CLICK
        fireEvent.click(buttonLogin);

        // RETORNANDO TOAST COM MESSAGEM DE ALERTA
        expect(toast.error).toHaveBeenCalledWith('Preencha os campos vazios!');

    });
}
~~~~

</details>

<h2>Conhecimentos Obtidos</h2>
<p align="justify">Essa experiência me proporcionou habilidades valiosas no desenvolvimento de testes unitários, incluindo a criação de testes robustos para validação de funcionalidades críticas. Além disso, adquiri uma sólida compreensão na criação de componentes genéricos reutilizáveis, garantindo maior eficiência e consistência no desenvolvimento do front-end. Estou comprometido em continuar aplicando essas habilidades técnicas em projetos futuros, contribuindo para a manutenção da qualidade do código e a escalabilidade das soluções.</p>
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
