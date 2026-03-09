# DESAFIO-QA-BEEDOO-2026
Desafio 2026 | Analista de Qualidade de Software Júnior

## 1. Objetivo da aplicação

O módulo tem o objetivo de permitir a criação de cursos para gerenciamento e verificação pela listagem, possibilitando que um usuário registre informações relevantes sobre cada curso e visualize posteriormente os cursos cadastrados. O sistema é voltado para gestão de cursos e treinamentos, permitindo armazenar dados como descrição, instrutor responsável, período de realização, número de vagas disponíveis e uma imagem ilustrativa do curso. 


## 2. Principais fluxos da aplicação

O usuário acessa a aba de cadastro e preenche os seguintes campos:

- Nome do curso
- Descrição
- Instrutor
- URL da imagem
- Data de início
- Data de fim
- Número de vagas
- Tipo de curso

Após o envio do formulário, o curso deve ser registrado no sistema.

### Listagem de cursos
A aplicação possui uma aba onde é possível visualizar os cursos previamente cadastrados.


## 3. Pontos críticos para teste

- Validação dos campos obrigatórios
- Exclusão de cursos da listagem que já terminaram
- Consistência entre data de início e data de fim
- Validação do número de vagas
- Validação de URL da imagem
- Persistência dos dados cadastrados
- Exibição correta das informações na listagem

---

## Criação de cenários e casos de teste

Os cenários e casos de teste foram documentados na planilha abaixo:

https://docs.google.com/spreadsheets/d/1rFYpIAUVHuhKhc3YjC3QGWS5ii6VS99rppHn6NyjWe4/edit?usp=sharing

Os testes incluem:

- Fluxo principal de cadastro de curso
- Listagem de cursos
- Cenários negativos
- Validação de campos
- Comportamentos inesperados


## Execução dos testes

As evidências da execução dos testes podem ser acessadas no link abaixo:

https://drive.google.com/drive/folders/1-Gjmdl2k7ORAEAnjqqBQWS_CSokhEv1M?usp=sharing

As evidências incluem:

- prints do fluxo de cadastro de cursos
- prints da listagem de cursos
- registros visuais dos bugs encontrados durante os testes

## Registro de Bugs

Durante a execução dos testes foram identificados alguns problemas relacionados principalmente à ausência de validação de dados no formulário de cadastro de cursos.

Principais problemas identificados durante os testes:

- Permite cadastrar curso sem nome
- Permite cadastrar curso com todos os campos vazios
- Permite inserir número de vagas negativo
- Permite cadastrar curso com data final anterior à data de início
- Permite cadastro com URL de imagem inválida
- Permite cadastro de cursos duplicados
- Permite valores extremamente altos no número de vagas
- Não remove espaços em branco no nome do curso

Esses problemas podem comprometer a integridade dos dados e a confiabilidade das informações exibidas na aplicação.

## Severidade dos bugs encontrados

Alta severidade
- Cadastro com todos os campos vazios
- Cadastro sem nome
- Datas inconsistentes
- Vagas negativas
- Vagas sem limites

Média severidade
- Cadastro duplicado
- URL inválida

Baixa severidade
- Espaços em branco no nome
