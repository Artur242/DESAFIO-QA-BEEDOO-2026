# DESAFIO-QA-BEEDOO-2026
Planilha de testes: https://docs.google.com/spreadsheets/d/1RNeh0wM8U6PAxy56KcrauVLxRbTedMJ3PB9AD6Mezzw/edit?usp=sharing

Evidências: https://drive.google.com/drive/folders/11_j6UzMxpUBDryb0l3Y-11-a1DThhqS0?usp=sharing

Relatório de bugs: https://docs.google.com/document/d/19Si_aVDmssYpiWswJzrUBtAgmXy_dvLCgrJSkr2LtLs/edit?usp=sharing

Acredito que o objetivo da aplicação Beedoo QA Chalenge é disponibilizar para o usuário uma plataforma que possibilite a criação e divulgação de cursos tanto online como presenciais.

Principais fluxos:
-Cadastro completo e válido
  Preencher todos os campos de forma válida
  Clicar em "Cadastrar Curso"
  Curso aparece na tela de listagem de cursos

-Cadastro com campos vazios
  Não preencher campos de nome, instrutor, datas, número de vagas e tipo de curso
  Sistema bloqueia o cadastro de exibe uma mensagem de erro

-Validação de dados
  Data validas e coerentes
  número de vagas inteiro e positivo
  url de imagem válido
  Sitema valida dados e permite apenas os corretos

-Tipo de curso presencial
  Selecionar curso "Presencial"
  Exibe um novo campo para preencher com endereço

-Cadastro de curso online
  Selecionar curso "Online"
  Exibe um novo campo para preencher com link de inscrição


Principais fluxos na tela de listagem de cursos
-Listagem de cursos
  Cursos devem ser exibidos com dados corretos e imagem carregada

-Exclusão de cursos
  Clicar em "Excluir curso"
  Curso removido da lista
  Exibida mensagem de confirmação

-Dados consistentes
  Dados na tela de cadastro devem aparecer na tela de lista de cursos da mesma forma que foram cadastrados


Pontos que considero mais críticos para testes:
Validação do campos de cadastro, verificar se campos obrigatórios podem ser deixados vazios, permitir que a data final selecionada para antes da data incial, possibilidade de números decimais ou negativos
Verificação de cadastro de curso e exclusão de cursos, verificar se é possível criar e excluir cursos
Verificação de consistência de dados
Validação do layout



Decisões para criação dos testes:
Para a criação dos testes, foquei em garantir a consistência dos dados, certificando que as informações inseridas no Cadastro de Cursos fossem exibidas fielmente na Lista de Cursos, sem perda de integridade ou alterações de formato. Identifiquei os campos mais críticos para o negócio e apliquei técnicas de Análise de valores. Isso incluiu a tentativa de cadastros com campos vazios e a inserção de dados inválidos. Avaliei a reação do sistema às interações do usuário, focando na Componentização e no layout. Analisei como a interface se comporta diante de diferentes volumes de dados ou ausência de informações, identificando falhas de alinhamento e renderização. Dada a ausência de documentação oficial, utilizei padrões de mercado, priorizando cenários que garantissem a usabilidade mínima da plataforma.
