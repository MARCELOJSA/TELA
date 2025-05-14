# Sistema de Gerenciamento de Hotel

## Alunos Participantes

- **Marcelo Jorge Souza Amancio**  
  Matrícula: 2404716

- **Raphael Teixeira Lacerda**  
  Matrícula: 2403900

- **Vinicius Daniel Silva Souza**  
  Matrícula: 2407900

---

## Sobre o Sistema

Este sistema foi desenvolvido em Java utilizando **Swing** para criar uma interface gráfica de gerenciamento de reservas de hotel. A aplicação permite ao usuário preencher dados de uma reserva, selecionar o status da mesma e visualizar um resumo com todas as informações preenchidas.

---

## Funcionalidades Principais

### 1. **Menu Principal**
- Interface gráfica inicial com um menu no topo.
- Contém três menus:
  - **Arquivo** → opção para sair do sistema.
  - **Opções** → acesso ao preenchimento dos dados da reserva, status da reserva e opção para salvar os dados.
  - **Ajuda** → exibe informações sobre o sistema.

### 2. **Preenchimento dos Dados**
- Ao clicar em **Preencher Campos**, é aberta uma nova janela (`Tela6Campos`) com 6 campos para preencher:
  - Nome do hóspede
  - Tipo de quarto
  - Data de check-in
  - Data de check-out
  - Número de hóspedes
  - Preferências adicionais

- Os dados são armazenados em um vetor estático chamado `dados` na classe `MainApp`.

### 3. **Status da Reserva**
- Ao clicar em **Status da Reserva**, uma nova janela (`TelaComboBox`) é exibida com uma `JComboBox` para selecionar o status:
  - Confirmada
  - Cancelada
  - Pendente

- O status escolhido é salvo no índice 6 do vetor `dados`.

### 4. **Salvar Dados**
- Ao clicar em **Salvar Dados**, o sistema verifica se todos os campos foram preenchidos.
- Caso positivo, exibe um resumo da reserva em uma janela com todos os dados inseridos.
- Caso algum campo esteja vazio, exibe uma mensagem pedindo o preenchimento completo.

---

## Tecnologias Utilizadas

- **Java**
- **Swing (javax.swing)**: biblioteca para interfaces gráficas
- **AWT (java.awt)**: utilizada para layout e manipulação de componentes gráficos

---

## Observações

- A imagem central da tela principal é carregada a partir de um arquivo local (`hotel.png`). Certifique-se de que esse arquivo exista no mesmo diretório do projeto ou forneça o caminho correto.
- O código utiliza uma abordagem simples com variáveis estáticas, ideal para protótipos ou sistemas pequenos. Para sistemas maiores, seria recomendado o uso de orientação a objetos mais estruturada e persistência de dados com banco de dados.

---

## Versão

**1.0 – Protótipo inicial**
