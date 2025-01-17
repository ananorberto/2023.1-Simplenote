# First things First (FTF)
## Introdução

Este é o documento de Frist things Frist do projeto de requisitos do grupo 5 referente ao Simplenote. A princípio, o documento tem a finalidade de definir quais requisitos serão priorizados pela equipe de desenvolvimento através de reuniões e uma planilha.

## Definição

First things First ou FTF é uma técnica de priorização que busca entender os riscos, custos e o valor de cada requisito para um produto, avaliando-os através de pesos para chegar em uma lista de prioridade.


## Passo a passo

1. Listar todos os requisitos, se um requisito A se liga com um requisito B, deve-se levar em conta apenas o A.
2. Estimar o valor de cada requisito para o cliente com uma escala de 1 a 9, em que 1 é pouco valoroso e 9 é muito valoroso, é importante a participação do cliente.
3. Estimar uma penalidade que o negócio sofreria na falta daquele requisito seguindo a mesma escala anterior.
4. Criar uma coluna valor total, na qual Vtotal = (Beneficio relativo * Peso relativo) + (Penalidade relativa * Peso relativo).
5. Estimar o custo relativo de implementação seguindo a escala já conhecida, este custo deve levar em conta: a complexidade de implementação, UI necessária, reúso de telas, etc
6. Estimar o risco da implementação de um requisito.
7. Calcular a prioridade dos requisitos com: prioridade = valor % / (custo % * peso_custo + risco % * peso_risco)
8. Ordenar a lista de forma decrescente de prioridade. Os requisitos do topo tem maior prioridade de implementação. Os stakeholders devem ter acesso a mesma.

## Métodos

Para realizar a análise de priorização, foram utilizados os seguintes métodos: Introspecção, Brainstorming, Entrevista, Glossário, Questionário e Storytelling. A participação do usuário ([personas](../personas.md)) foi essencial nos passos 2 e 3, contribuindo para a definição do valor e da penalidade de cada requisito.

- Data: 28 de abril de 2023 e 29 de abril de 2023
- Horário: 10:00 e 20:30
- Local: Campus FGA - UnB e Discord

## Resultados

A tabela a seguir mostra os resultados alcançados após a priorização dos requisitos: </br>
Obs: A todos os pesos foi atribuido o valor 1, exceto ao peso relativo de benefício, no qual foi atribuido o valor 2.

| **Codigo** | **Req** | **valor** | **penalidade** | **valor total** | **valor(%)** | **custo relativo** | **custo (%)** | **Dificuldade imp** | **Difi(%)** | **Prioridade** |
|---|---|---|---|---|---|---|---|---|---|---|
| **INT01** | O usúario deve poder fazer anotação | 9 | 9 | 27 | 2,55% | 1 | 0,40% | 1 | 0,42% | 3,10 |
| **INT06** | O usúario deve poder vizualizar Anotação | 9 | 9 | 27 | 2,55% | 1 | 0,40% | 1 | 0,42% | 3,10 |
| **INT10** | O usúario deveria poder fazer notas sem internet | 9 | 9 | 27 | 2,55% | 1 | 0,40% | 1 | 0,42% | 3,10 |
| **INT13** | O usúario deve poder editar Anotação | 9 | 9 | 27 | 2,55% | 1 | 0,40% | 1 | 0,42% | 3,10 |
| **B01** | O aplicativo deve permitir ao usuário criar uma nova nota com título e conteúdo. | 9 | 9 | 19 | 1,79% | 1 | 0,40% | 1 | 0,42% | 2,18 |
| **B02** | O usuário deve ser capaz de editar o título e o conteúdo de uma nota existente. | 9 | 9 | 19 | 1,79% | 1 | 0,40% | 1 | 0,42% | 2,18 |
| **B03** | O aplicativo deve permitir ao usuário excluir notas existentes. | 9 | 9 | 19 | 1,79% | 1 | 0,40% | 1 | 0,42% | 2,18 |
| **B25** | O aplicativo deve estar disponível para uso sempre que o usuário precisar, sem interrupções ou indisponibilidades não planejadas. | 9 | 9 | 19 | 1,79% | 1 | 0,40% | 1 | 0,42% | 2,18 |
| **INT02** | O usúario deve poder excluir anotação | 9 | 8 | 26 | 2,45% | 2 | 0,81% | 1 | 0,42% | 2,00 |
| **INT07** | O aplicativo salvará a nota em até 1 segundo | 8 | 9 | 25 | 2,36% | 2 | 0,81% | 1 | 0,42% | 1,92 |
| **ST07** | Ser capaz de funcionar sem internet | 9 | 8 | 14 | 1,32% | 1 | 0,40% | 1 | 0,42% | 1,61 |
| **INT11** | O usuario poderia separar suas notas em pastas | 6 | 7 | 19 | 1,79% | 1 | 0,40% | 2 | 0,83% | 1,45 |
| **ENT07** | O aplicativo deve permitir a criação de backups automáticos ou manuais das notas para evitar perda de informação | 9 | 6 | 22 | 2,08% | 2 | 0,81% | 2 | 0,83% | 1,26 |
| **GLO01** | Possibilidade de usar marcação de texto (negrito, itálico, etc) | 5 | 4 | 22 | 2,08% | 2 | 0,81% | 2 | 0,83% | 1,26 |
| **ENT03** | O aplicativo deve permitir a adição de etiquetas nas notas para facilitar a organização | 6 | 4 | 22 | 2,08% | 1 | 0,40% | 3 | 1,25% | 1,25 |
| **INT09** | O aplicativo abrirá em um tempo limite de até 2 segundos | 8 | 8 | 24 | 2,26% | 3 | 1,21% | 2 | 0,83% | 1,11 |
| **B20** | O aplicativo deve ser intuitivo e fácil de usar, com uma interface clara e simples. | 9 | 9 | 19 | 1,79% | 2 | 0,81% | 2 | 0,83% | 1,09 |
| **ST02** | Criar _checklists_ nas notas | 4 | 2 | 14 | 1,32% | 1 | 0,40% | 2 | 0,83% | 1,07 |
| **INT05** | O usúario deve poder usar Markdown | 7 | 4 | 18 | 1,70% | 2 | 0,81% | 2 | 0,83% | 1,03 |
| **INT14** | O usúario deve poder buscar notas por palavras-chave | 7 | 2 | 16 | 1,51% | 2 | 0,81% | 2 | 0,83% | 0,92 |
| **INT15** | O usúario deveria poder pesquisar por suas anotações | 7 | 2 | 16 | 1,51% | 2 | 0,81% | 2 | 0,83% | 0,92 |
| **GLO04** | Possibilidade de criar checklists dentro das notas | 4 | 3 | 15 | 1,42% | 2 | 0,81% | 2 | 0,83% | 0,86 |
| **B27** | O aplicativo deve ser facilmente mantido e atualizado, com um código limpo e bem documentado. | 5 | 5 | 15 | 1,42% | 2 | 0,81% | 2 | 0,83% | 0,86 |
| **ST06** | Poder baixar uma cópia da nota no dispositivo | 6 | 4 | 14 | 1,32% | 2 | 0,81% | 2 | 0,83% | 0,80 |
| **ENT08** | O aplicativo deve ter uma interface simples e fácil de usar, sem muitas opções desnecessárias | 8 | 7 | 23 | 2,17% | 5 | 2,02% | 3 | 1,25% | 0,66 |
| **INT18** | A interface deve ser simples e intuitivo | 7 | 8 | 20 | 1,89% | 5 | 2,02% | 2 | 0,83% | 0,66 |
| **GLO05** | Salvamento automático das notas | 9 | 8 | 20 | 1,89% | 3 | 1,21% | 4 | 1,67% | 0,65 |
| **INT16** | O usuario poderia ver informações sobre sua nota | 6 | 5 | 17 | 1,60% | 4 | 1,62% | 2 | 0,83% | 0,65 |
| **B09** | O aplicativo deve permitir ao usuário formatar o texto das notas, como fonte, tamanho, cor, estilo e alinhamento. | 6 | 7 | 17 | 1,60% | 3 | 1,21% | 3 | 1,25% | 0,65 |
| **INT04** | O usuário poderá compartilhar suas anotações com outras pessoas atraves de um link | 6 | 5 | 17 | 1,60% | 2 | 0,81% | 4 | 1,67% | 0,65 |
| **GLO06** | Capacidade de criar no dispositivo um arquivo cópia de uma nota | 3 | 2 | 14 | 1,32% | 3 | 1,21% | 2 | 0,83% | 0,64 |
| **ENT01** | O aplicativo deve permitir a criação de notas de forma fácil e rápida, sem muitas etapas | 9 | 8 | 16 | 1,51% | 4 | 1,62% | 2 | 0,83% | 0,62 |
| **B21** | O aplicativo deve ser responsivo e rápido, permitindo que os usuários criem e acessem suas notas rapidamente. | 9 | 9 | 19 | 1,79% | 5 | 2,02% | 3 | 1,25% | 0,55 |
| **INT08** | Para o primeiro acesso do usuário, deve ter uma breve explicação sobre o aplicativo e as suas funcionalidades | 3 | 1 | 7 | 0,66% | 1 | 0,40% | 2 | 0,83% | 0,53 |
| **B23** | O aplicativo deve ser acessível para usuários com deficiências visuais ou motoras, com recursos como suporte a leitores de tela e opções de zoom. | 6 | 8 | 18 | 1,70% | 4 | 1,62% | 4 | 1,67% | 0,52 |
| **B16** | O aplicativo deve permitir que os usuários criem notas com lembretes de data e hora para ajudá-los a acompanhar compromissos ou tarefas importantes. | 4 | 3 | 13 | 1,23% | 3 | 1,21% | 3 | 1,25% | 0,50 |
| **QUE01** | O sistema deve ser simples e intuitivo | 8 | 9 | 19 | 1,79% | 6 | 2,43% | 3 | 1,25% | 0,49 |
| **ENT09** | O aplicativo deve permitir o login com diferentes opções, como e-mail, Google ou Facebook, para facilitar o acesso ao aplicativo após formatação ou troca de dispositivo | 7 | 6 | 22 | 2,08% | 4 | 1,62% | 7 | 2,92% | 0,46 |
| **B19** | O aplicativo deve ser confiável e estável, evitando falhas ou perda de dados. | 9 | 9 | 19 | 1,79% | 5 | 2,02% | 5 | 2,08% | 0,44 |
| **GLO03** | Ser capaz de ler e editar arquivos de texto de outras fontes | 4 | 5 | 23 | 2,17% | 5 | 2,02% | 7 | 2,92% | 0,44 |
| **B24** | O aplicativo deve estar disponível em várias plataformas, como iOS, Android, Windows e Mac, para garantir que os usuários possam acessar suas notas em qualquer dispositivo. | 6 | 7 | 17 | 1,60% | 6 | 2,43% | 3 | 1,25% | 0,44 |
| **B08** | O aplicativo deve fornecer opções de segurança, como senha ou autenticação biométrica, para proteger as notas do usuário. | 6 | 7 | 17 | 1,60% | 5 | 2,02% | 4 | 1,67% | 0,43 |
| **B07** | O usuário deve ser capaz de compartilhar notas com outras pessoas por meio de diferentes plataformas. | 5 | 7 | 17 | 1,60% | 4 | 1,62% | 5 | 2,08% | 0,43 |
| **ST03** | Compartilhar publicamente as notas | 5 | 3 | 15 | 1,42% | 4 | 1,62% | 4 | 1,67% | 0,43 |
| **B04** | O usuário deve ser capaz de organizar suas notas em ordem data de criação, alfabética, etc. | 5 | 3 | 13 | 1,23% | 3 | 1,21% | 4 | 1,67% | 0,43 |
| **B13** | O aplicativo deve ser capaz de enviar notificações aos usuários para lembrá-los de tarefas ou compromissos importantes. | 3 | 3 | 13 | 1,23% | 3 | 1,21% | 4 | 1,67% | 0,43 |
| **B26** | O aplicativo deve ser otimizado para usar recursos do dispositivo de forma eficiente, como CPU, memória e bateria. | 5 | 8 | 18 | 1,70% | 5 | 2,02% | 5 | 2,08% | 0,41 |
| **B05** | O usuário deve ser capaz de pesquisar notas por palavra-chave ou tag. | 5 | 4 | 14 | 1,32% | 4 | 1,62% | 4 | 1,67% | 0,40 |
| **B10** | O usuário deve ser capaz de anexar arquivos, imagens, áudios ou vídeos às notas. | 5 | 7 | 17 | 1,60% | 6 | 2,43% | 4 | 1,67% | 0,39 |
| **B11** | O aplicativo deve fornecer uma opção de modo escuro para reduzir o cansaço visual em ambientes com pouca iluminação. | 7 | 7 | 17 | 1,60% | 5 | 2,02% | 5 | 2,08% | 0,39 |
| **INT03** | O usúario deve poder recuperar anotação excluida | 6 | 3 | 15 | 1,42% | 5 | 2,02% | 4 | 1,67% | 0,38 |
| **B18** | O aplicativo deve manter um histórico de versão de notas, permitindo que os usuários voltem para versões anteriores de suas notas. | 4 | 6 | 16 | 1,51% | 6 | 2,43% | 4 | 1,67% | 0,37 |
| **B12** | Os usuários devem poder exportar suas notas em diferentes formatos, como PDF ou Word, para uso posterior fora do aplicativo. | 5 | 6 | 16 | 1,51% | 5 | 2,02% | 5 | 2,08% | 0,37 |
| **B22** | O aplicativo deve garantir a segurança e privacidade das notas dos usuários, protegendo-as contra acesso não autorizado ou perda de dados. | 9 | 9 | 19 | 1,79% | 6 | 2,43% | 6 | 2,50% | 0,36 |
| **ST01** | Escrever notas em conjunto com outros usuários | 7 | 4 | 22 | 2,08% | 7 | 2,83% | 8 | 3,33% | 0,34 |
| **GLO02** | Estar disponível em diversos dispositivos (celulares, laptops, tablets, etc) | 8 | 8 | 24 | 2,26% | 9 | 3,64% | 9 | 3,75% | 0,31 |
| **ENT05** | O aplicativo deve permitir o compartilhamento de notas com outras pessoas, por meio de um link ou por e-mail | 3 | 3 | 15 | 1,42% | 6 | 2,43% | 5 | 2,08% | 0,31 |
| **ST04** | Desenhar nas notas | 5 | 3 | 13 | 1,23% | 4 | 1,62% | 6 | 2,50% | 0,30 |
| **B15** | O aplicativo deve permitir que os usuários trabalhem em notas simultaneamente, com alterações sendo exibidas em tempo real. | 5 | 4 | 14 | 1,32% | 6 | 2,43% | 5 | 2,08% | 0,29 |
| **B06** | O aplicativo deve permitir a sincronização de notas entre diferentes dispositivos do usuário. | 3 | 6 | 16 | 1,51% | 6 | 2,43% | 7 | 2,92% | 0,28 |
| **INT12** | O usuario poderia definir templates para suas notas | 4 | 3 | 11 | 1,04% | 5 | 2,02% | 4 | 1,67% | 0,28 |
| **B17** | O usuário deve ser notificado de tarefas ou compromissos importantes ou quando há alterações em notas compartilhadas. | 2 | 1 | 11 | 1,04% | 5 | 2,02% | 4 | 1,67% | 0,28 |
| **ST05** | Ser capaz de usar a aplicação em dispositivos _mobile_ (celulares e tablets) | 9 | 9 | 19 | 1,79% | 9 | 3,64% | 8 | 3,33% | 0,26 |
| **ENT04** | O aplicativo deve possuir um editor de texto avançado para permitir a utilização da função `toggle` | 2 | 1 | 7 | 0,66% | 3 | 1,21% | 4 | 1,67% | 0,23 |
| **ENT06** | O aplicativo deve ser acessível em diferentes plataformas, como computadores, tablets e smartphones | 9 | 9 | 17 | 1,60% | 9 | 3,64% | 9 | 3,75% | 0,22 |
| **ENT02** | O aplicativo deve permitir a sincronização das notas em tempo real em diferentes dispositivos | 3 | 3 | 9 | 0,85% | 3 | 1,21% | 8 | 3,33% | 0,19 |
| **B14** | O aplicativo deve ser capaz de reconhecer e transcrever a voz dos usuários em notas. | 1 | 1 | 11 | 1,04% | 7 | 2,83% | 8 | 3,33% | 0,17 |
| **INT17** | O usuario poderia importar ou exportar modelos de layout | 2 | 1 | 5 | 0,47% | 7 | 2,83% | 5 | 2,08% | 0,10 | 
| Total | *** | 379 | 348 | 1060 | 100,00% | 247 | 100,00% | 240 |100,00%|48.28|
<p align="center"> Tabela 1: Tabela de priorização FTF <br> Fonte: autores <br> Autores: João e Kauã </p>

### Legenda:
- INT: Introspecção
- B: Brainstorming
- ENT: Entrevista
- GLO: Glossário
- QUE: Questionário
- ST: Storytelling


## Bibliografia

[1] https://aprender3.unb.br/pluginfile.php/2580553/mod_resource/content/2/Requisitos%20-%20Aula%2007.pdf

## Histórico de versão

| Versão |    Data    |                         Descrição                          |    Autor    | Revisor |
| :----: | :--------: | :--------------------------------------------------------: | :---------: | :-----: |
|  `1.0` | 28/04/2023 |                 Inicialização do documento                 | Kauã e João | Mylena  |
|  `1.1` | 29/04/2023 | Confecção da tabela e preenchimento inicial dos requisitos | João e Kauã | Mylena  |
|  `1.2` | 01/05/2023 |   Finalizando o documento e adicionando tabela ordenada    | Kauã e João | Mylena  |
|  `1.3` | 15/05/2023 |                Ajustes Feedbacks entrega 2                 | Ana Beatriz | Mylena  |














      - Verificação - Simplenote:
          - Elicitação:
            - Técnicas Planejadas:
              - StoryTelling: analise/analise-Grupo5/elicitacao/StoryTelling.md
              - Personas: analise/analise-Grupo5/elicitacao/Personas.md
              - Questionário: analise/analise-Grupo5/elicitacao/Questionário.md
              - Introspecção: analise/analise-Grupo5/elicitacao/Introspecção.md
              - Glossário: analise/analise-Grupo5/elicitacao/glossario.md
              - Entrevista: analise/analise-Grupo5/elicitacao/entrevista.md
              - Brainstorm: analise/analise-Grupo5/elicitacao/brainstorming.md
            - Priorização:
              - MosCoW: analise/analise-Grupo5/elicitacao/Priorização/moscow.md
              - First Things First (FTF): analise/analise-Grupo5/elicitacao/Priorização/FTF.md
              - Escala de Três Níveis: analise/analise-Grupo5/elicitacao/Priorização/TLS.md
          - Modelagem:
            - Modelagem Ágil:
              - História de Usuário: analise/analise-Grupo5/modelagem/agil/HistoriasDeUsario.md
              - Backlog: analise/analise-Grupo5/modelagem/agil/backlog.md
              - NFR: analise/analise-Grupo5/modelagem/nfr.md
            - Léxicos: analise/analise-Grupo5/modelagem/lexico.md
            - Cenários: analise/analise-Grupo5/modelagem/Cenarios.md
            - Casos de Uso: analise/analise-Grupo5/modelagem/CasosDeUso.md
            - Especificação Suplementar: analise/analise-Grupo5/modelagem/especificacao_suplementar.md
          - Planejamento:
            - Cronograma pretendido: analise/analise-Grupo5/planejamento/cronograma.md
            - Cronograma realizado: analise/analise-Grupo5/planejamento/cronograma_realizado.md
            - Ferramentas: analise/analise-Grupo5/planejamento/ferramentas.md
            - Metodologias: analise/analise-Grupo5/planejamento/metodologias.md
          - Aplicativo Selecionado: analise/analise-Grupo5/planejamento/app.md
          - Rich Picture: analise/analise-Grupo5/planejamento/rich_picture.md



          ___________________________



            - Análises (V&V):
    - Verificação:
      - Verificação Grupo 6:
        - Verificação geral: analise/analise-grupo6/verificacao_grupo6.md
        - Elicitação:
          - Perfil do usuário: analise/analise-grupo6/elicitacao/PerfilDeUsuario.md
          - Análise de documento: analise/analise-grupo6/elicitacao/analise_documentos.md
          - Entrevista: analise/analise-grupo6/elicitacao/entrevista.md
          - Introspecção: analise/analise-grupo6/elicitacao/instrospecção.md
          - Personas: analise/analise-grupo6/elicitacao/personas.md
          - Priorização: analise/analise-grupo6/elicitacao/priorizacao.md
          - Questionário: analise/analise-grupo6/elicitacao/questionario.md
          - Priorização: analise/analise-grupo6/elicitacao/priorizacao.md
          - Storytelling: analise/analise-grupo6/elicitacao/storytelling.md
        - Modelagem:
          - Modelagem Ágil:
            - História de Usuário: analise/analise-grupo6/modelagem/Agil/Historias_de_usuario.md
            - Backlog: analise/analise-grupo6/modelagem/Agil/backlog.md
          - NFR: analise/analise-grupo6/modelagem/NFR.md
          - Léxicos: analise/analise-grupo6/modelagem/lexicos.md
          - Casos de Uso: analise/analise-grupo6/modelagem/casos_de_uso.md
          - Cenários: analise/analise-grupo6/modelagem/cenarios.md
          - Especificação Suplementar: analise/analise-grupo6/modelagem/especificacao_suplementar.md
          - Léxicos: analise/analise-grupo6/modelagem/lexicos.md
        - Planejamento:
          - Cronograma: analise/analise-grupo6/planejamento/cronograma.md
          - Ferramentas: analise/analise-grupo6/planejamento/ferramentas.md
          - Metodologias: analise/analise-grupo6/planejamento/metodologia.md
          - Aplicativo Selecionado: analise/analise-grupo6/planejamento/app.md
          - Rich Picture: analise/analise-grupo6/planejamento/RichPicture.md
        - Extra:
          - GitPage: analise/analise-grupo6/extras/gitpage.md
          - Atas: analise/analise-grupo6/extras/atas.md
        - Template: analise/analise-grupo6/template.md
      - Verificação - Simplenote:
          - Elicitação:
            - Técnicas Planejadas:
              - StoryTelling: analise/verificacao-Grupo5/elicitacao/StoryTelling.md
              - Personas: analise/verificacao-Grupo5/elicitacao/Personas.md
              - Questionário: analise/verificacao-Grupo5/elicitacao/Questionário.md
              - Introspecção: analise/verificacao-Grupo5/elicitacao/Introspecção.md
              - Glossário: analise/verificacao-Grupo5/elicitacao/glossario.md
              - Entrevista: analise/verificacao-Grupo5/elicitacao/entrevista.md
              - Brainstorm: analise/verificacao-Grupo5/elicitacao/brainstorming.md
            - Priorização:
              - MosCoW: analise/verificacao-Grupo5/elicitacao/Priorização/moscow.md
              - First Things First (FTF): analise/verificacao-Grupo5/elicitacao/Priorização/FTF.md
              - Escala de Três Níveis: analise/verificacao-Grupo5/elicitacao/Priorização/TLS.md
          - Modelagem:
            - Modelagem Ágil:
              - História de Usuário: analise/verificacao-Grupo5/modelagem/agil/HistoriasDeUsario.md
              - Backlog: analise/verificacao-Grupo5/modelagem/agil/backlog.md
              - NFR: analise/verificacao-Grupo5/modelagem/nfr.md
            - Léxicos: analise/verificacao-Grupo5/modelagem/lexico.md
            - Cenários: analise/verificacao-Grupo5/modelagem/Cenarios.md
            - Casos de Uso: analise/verificacao-Grupo5/modelagem/CasosDeUso.md
            - Especificação Suplementar: analise/verificacao-Grupo5/modelagem/especificacao_suplementar.md
          - Planejamento:
            - Cronograma pretendido: analise/verificacao-Grupo5/planejamento/cronograma.md
            - Cronograma realizado: analise/verificacao-Grupo5/planejamento/cronograma_realizado.md
            - Ferramentas: analise/verificacao-Grupo5/planejamento/ferramentas.md
            - Metodologias: analise/verificacao-Grupo5/planejamento/metodologias.md
          - Aplicativo Selecionado: analise/verificacao-Grupo5/planejamento/app.md
          - Rich Picture: analise/verificacao-Grupo5/planejamento/rich_picture.md
    - Validação: 
      - Protótipo: analise/validacao/prototipo.md
      - Comprovação informal: analise/validacao/comprovacao_informal.md
