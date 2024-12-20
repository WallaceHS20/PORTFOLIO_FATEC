<div class="semestre1">

<div align=center>
<h1>OTUS PROJECT</h1>
</div>

<h4> 1º Semestre • <a href="https://github.com/B1nary-Devs/OTUS-PROJECT">Repositório Github</a></h4>
<p align="justify"> Empresa Parceira • <a href="https://fatecsjc-prd.azurewebsites.net">FATEC SJC</a></p>

<p align="center"><img src="https://github.com/WallaceHS20/Bertoti/assets/101594950/2858b006-347d-4796-9a4b-c5edb0c4ea19" widht="20%"></img>

<p align="justify"> A Otus Project é uma assistente virtual acionada por comando de voz, tendo como público alvo alunos de programação que buscam inovar seus métodos de estudo e organizar seus horários.</p>

<h2> <a name="Objetivo">Objetivo</a> </h2>

* O sistema será capaz de responder a comandos de voz ou sons específicos
* O sistema será capaz de auxiliar o aluno em sua rotina de estudos.
* O usuário conseguirá obter artigos com facilidades
  
<br>

<h2> <a name="Objetivo">Visão do Projeto</a> </h2>

![Inserir um título](https://github.com/user-attachments/assets/3c9b2a48-584c-4e73-b91e-ed1d35dee26e)
  
<br>

<h2>Tecnologias Utilizadas no Projeto</h2>

<p align="justify"> <strong>Python 3 </strong> linguagem para desenvolvimento da aplicação para front-end e back-end.</p>

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
  
<br>
  
<h2>Minhas Contribuições</h2>

 > Atuei de forma significativa no desenvolvimento de funcionalidades do sistema, focando na eficiência e na melhoria da experiência de interatividade para o usuário.

## 1. **Desenvolvimento de funcionalidades do sistema**
   - Contribuí ativamente com desenvolvimento de funcionalidades do sistema e interatividade do usuário. 

<details>
  <summary>Detalhes</summary>

~~~~python
# A função seguinte tem como objetivo escutar o usuário e encaminha-lo para uma página de um artigo com seu respectivo assunto escolhido

def consult_art():
    while True:
        falar('DIGA O NÚMERO DO ITEM QUE DESEJA PESQUISAR EM VOZ ALTA:')
        threading.Thread(target=tocar, args=["start.mp3"]).start()
        escolha = ouvir() #variavel escolha recebe valor dito pelo usuario
        threading.Thread(target=tocar, args=["success.mp3"]).start()
        new = 0

            #caso escolha seja verdadeira, executa comando para abrir navegador com url pré-determinada
        if escolha == '1':
            webbrowser.open('https://ftp.unicamp.br/pub/apoio/treinamentos/logica/logica.pdf', new=new)
            webbrowser.open('https://www.seduc.ce.gov.br/wp-content/uploads/sites/37/2012/06/informatica_logica_de_programacao.pdf', new=new)
            webbrowser.open("https://dicasdeprogramacao.com.br/download/ebook-logica-de-programacao-para-iniciantes.pdf", new=new)
            interface.destroy() #após navegador ser aberto, fechará a interface e pausa a repetição
            break

        elif escolha == '2':
            webbrowser.open('http://antigo.scl.ifsp.edu.br/portal/arquivos/2016.05.04_Apostila_Python_-_PET_ADS_S%C3%A3o_Carlos.pdf', new=new)
            webbrowser.open('https://irias.com.br/blog/python-mysql-criando-um-crud-completo/', new=new)
            interface.destroy()
            break

        elif escolha == '3':
            webbrowser.open('https://www.devmedia.com.br/instalando-e-configurando-a-nova-versao-do-mysql/25813', new=new)
            webbrowser.open('http://www.telecentros.sp.gov.br/saber/apostilas/antigas/apostila_sql.pdf', new=new)
            interface.destroy()
            break

        else:
            falar("Diga um valor compatível com a lista!") # caso escolha do usuraio seja incompativel com itens da lista
~~~~
  
</details>

## 2. **Execução de funcionalidades em Thread**
   - Contribuí ativamente para o desenvolvimento de funcionalidades em thread, permitindo a execução simultânea de tarefas e otimizando a interatividade com o usuário.

<details>
  <summary>Detalhes</summary>

~~~~python
# EXECUÇÃO DE DUAS FUNCIONALIDADES SIMULTÂNEAS ( INTERFACE E SISTEMA DE VOZ )
def guia_de_estudo():
    global interface
    interface = Tk()
    image = Image.open("imagens\\fundo_consult.png")
    photo = ImageTk.PhotoImage(image, master=interface)
    fundo = tk.Label(interface, image=photo)
    fundo.image = image
    fundo.pack()
    interface.geometry('800x650+250+5')
    interface.title("Guia de estudo")
    threading.Thread(target=questionario).start() # executar função simultaneamente com interface
    interface.mainloop() #executa a abertura da interface
~~~~
  
</details>

<h2>Conhecimentos Obtidos</h2>
<p align="justify">
  No primeiro semestre, tive a oportunidade de participar pela primeira vez de um grande projeto em equipe, utilizando metodologias ágeis e práticas de versionamento com Git. Essa experiência foi fundamental para desenvolver minhas habilidades em colaboração, organização de tarefas e adaptabilidade dentro de um ambiente de desenvolvimento ágil. Compreendi melhor o ciclo de vida do desenvolvimento de software, desde a divisão de tarefas até a integração e o versionamento do código. 
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
      <td>Python</td>
      <td>Sei fazer com Autonomia</td>
    </tr>
    <tr>
      <td>Git</td>
      <td>Sei fazer com Ajuda</td>
    </tr>
  </table>
</details>
<h3>Soft Skills </h3>
<details>
<summary><b>Clique para ver a lista de soft skills</b></summary>
  <br>
  <table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th style="background-color: #dce6f1;">Habilidade</th>
    <th style="background-color: #dce6f1;">Descrição</th>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2;">Proatividade</td>
    <td>Precisei tomar iniciativas para antecipar problemas e propor soluções antes que surgissem.</td>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2;">Visão de Negócio</td>
    <td>Precisei entender o impacto das minhas ações no negócio e alinhar minhas atividades com os objetivos estratégicos da empresa.</td>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2;">Comunicação</td>
    <td>Precisei comunicar de forma clara e eficaz com a equipe para alinhar expectativas e compartilhar informações importantes.</td>
  </tr>
  <tr>
    <td style="background-color: #f2f2f2;">Organização e Planejamento</td>
    <td>Precisei planejar e organizar minhas tarefas para cumprir prazos e garantir a eficiência no desenvolvimento do projeto.</td>
  </tr>
</table>

</details>

-------------------
[RETORNAR A PÁGINA PRINCIPAL](https://github.com/WallaceHS20/PORTFOLIO_FATEC)
