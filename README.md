# Documentação Técnica de Integração

**Projeto:** Integração de Formulário Front-End com Backend em POO
**Versão:** 1.1
**Data:** Setembro/2025
**Responsável:** Equipe de Desenvolvimento Web

---

## 1. Contexto do Projeto

O projeto conta atualmente com um **front-end pronto** para coleta de dados, desenvolvido em **HTML5, CSS3 com Bootstrap 5.3** e **JavaScript**. Este front-end tem como função principal capturar as informações digitadas pelo usuário e armazená-las em variáveis locais.

O **backend**, já existente, foi construído em **JavaScript com Programação Orientada a Objetos (POO)**, e concentra as regras de negócio e funcionalidades de processamento dos dados.

O próximo passo da equipe é realizar a **integração entre essas duas camadas**, utilizando os recursos já desenvolvidos.

---

## 2. Objetivo

O objetivo desta documentação é:

* Explicar de forma clara o funcionamento do código atual no front-end.
* Destacar suas limitações.
* Definir o que deverá ser realizado pelos desenvolvedores para completar a integração com o backend em POO.

---

## 3. Funcionamento do Código Atual

1. O **formulário** exibe campos de entrada para **nome, e-mail, telefone e senha**.
2. O botão "Salvar Dados" chama a função `salvarDados()`.
3. Essa função coleta os valores digitados pelo usuário através de `document.getElementById("id").value`.
4. Os dados são **armazenados em variáveis locais** (`nome`, `email`, `telefone`, `senha`).
5. Nenhuma ação adicional é executada: os dados não são exibidos, enviados ou persistidos.

Esse design deixa a lógica de integração propositalmente em aberto para que seja desenvolvida no backend.

---

## 4. Limitações do Código Atual

* Os dados coletados não são validados além das restrições básicas do HTML5 (`required`, `type`).
* Não há comunicação com o backend em POO.
* Nenhum dado é persistido em banco de dados ou outro armazenamento.
* Não há feedback ao usuário após a submissão.
* Não existe camada de segurança implementada para proteger as informações sensíveis (ex.: senha).

---

## 5. Responsabilidades de Integração

A partir do estado atual do código, os desenvolvedores deverão:

* **Criar a ligação entre front-end e backend**, aproveitando as classes já existentes no código orientado a objetos.
* **Encaminhar os dados capturados** (nome, e-mail, telefone e senha) para os métodos adequados do backend.
* **Implementar regras de negócio** e validações de acordo com a lógica definida no backend.
* **Definir o retorno esperado** (sucesso, falha, mensagens de erro) e integrar com a interface do formulário.

---

## 6. Considerações Finais

O front-end entregue é uma **base estável e responsiva** para entrada de dados. No entanto, ele é apenas um ponto de partida.

A evolução deste projeto depende da **integração com o backend em POO**, que será responsável por aplicar as regras de negócio, validar as informações, armazenar os dados e fornecer o retorno necessário ao usuário.

Esta documentação não dita como essa integração deve ser feita, justamente para deixar em aberto diferentes abordagens técnicas que poderão ser exploradas pelos desenvolvedores, de acordo com a estrutura do backend já existente.
