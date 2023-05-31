# Trabalho Individual de Gestao de Configuracao de Software 2023/1
Versao JAVASCRIPT
10 Pontos

## 1 Descri ̧c ̃ao
Os conhecimentos de Gestao de Configuracao de Software sao fundamentais no ciclo de vida de um produto de software. As t ́ecnicas para a gestao vao desde o controle de versao, automacao de build e de configuracao de ambiente, testes automatizados, isolamento do ambiente ate o deploy do sistema. Este ciclo sao atualmente integrados em um pipeline de DevOps com as etapas de Integracao Contınua (CI) e Deploy Contınuo (CD) implementadas e automatizada.
Para exercitar estes conhecimentos, neste trabalho, voce dever ́a aplicar os conceitos estudados ao longo da disciplina no produto de software contido neste repositorio (PUC-GCES-JS).
O sistema se trata de uma aplicacao em Django e React que gerencia uma biblioteca. Para executar a aplica ̧c ̃ao em sua m ́aquina, basta seguir o passo-a-passo descrito nas pastas do Backend e Frontend arquivo. Link do projeto: PUC-GCES-JS

## 2 Sobre a Aplicacao
A aplica ̧c ̃ao  ́e um simples sistema de gerenciamento de uma biblioteca. Por ́em, o foco do trabalho  ́e na automa ̧c ̃ao da build, testes, conteineriza ̧c ̃ao e configura ̧c ̃ao dos pipelines de CI/CD.

## 3 Etapas do Trabalho
O trabalho deve ser elaborado por etapas. Cada uma das etapas deve ser realizada em um commit separado com o resultado funcional desta etapa. As etapas de 1 a 3 (VEJA A TABELA 1) s ̃ao relacionadas ao isolamento do ambiente utilizando a ferramenta Docker e Docker Compose. Neste sentido o tutorial abaixo cobre os conceitos fundamentais para o uso destas tecnologias.


### 3.1 Tutoriais
As etapas de 4 a 6 (VEJA A TABELA 1) s ̃ao relacionadas a configura ̧c ̃ao do pipeline de CI e CD.

## 4 Containeriza ̧c ̃ao do Banco
A vers ̃ao inicial do sistema cont ́em uma aplica ̧c ̃ao Django no backend cujo funcionamento requer uma instala ̧c ̃ao de um banco de dados Postgres. A primeira etapa do trabalho  ́e de configurar um container somente para o banco de dados com as credenciais especificadas na
descri ̧c ̃ao da aplica ̧c ̃ao e testar o funcionamento do mesmo.

## 5 Containeriza ̧c ̃ao da aplica ̧c ̃ao + banco
Nesta segunda etapa, tanto o backend quanto o banco de dados dever ̃ao estar funcionando em containers individuais. Dever ́a ser utilizado um orquestrador (Docker Compose) para gerenciar comunica ̧c ̃ao entre os containers al ́em do uso de credenciais, networks, volumes, entre outras configura ̧c ̃oes necess ́arias para a correta execu ̧c ̃ao da aplica ̧c ̃ao.

## 6 Configura ̧c ̃ao do Frontend
A terceira etapa do trabalho consiste em dockerizar o frontend que  ́e uma aplica ̧c ̃ao em React seguindo as instru ̧c ̃oes do README e incluindo a mesma no Docker Compose.

## 7 Servindo a aplica ̧c ̃ao com o Nginx
A  ́ultima etapa de configura ̧c ̃ao do ambiente  ́e a de servir a aplica ̧c ̃ao atrav ́es do Nginx. Neste caso, ser ́a necess ́ario configurar o Nginx em um container e adicion ́a-lo ao Docker Compose.

## 8 Integra ̧c ̃ao Cont ́ınua (CI)
Para a realiza ̧c ̃ao desta etapa, a aplica ̧c ̃ao j ́a dever ́a ter seu ambiente completamente containerizado. Dever ́a ser utilizada uma ferramenta de Integra ̧c ̃ao Cont ́ınua para garantir o build, os testes e os deploy para o Docker Hub dos servi ̧cos principais. Esta etapa do trabalho poder ́a ser realizada utilizado os ambientes de CI do GitLab-CI ou Github Actions.
Requisitos da configura ̧c ̃ao da Integra ̧c ̃ao Cont ́ınua (Gitlab ou Github) incluem:

• Build
• Test
• Lint

## 9 Deploy Cont ́ınuo (CD)
A etapa final do trabalho dever ́a ser realizada a partir do deploy autom ́atico da aplica ̧c ̃ao
que deve ser realizado ap ́os passar sem erros em todas as etapas de CI.
