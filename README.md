# Splash Screen com Animação em Flutter

## Descrição do Projeto
Este projeto foi desenvolvido com o objetivo de criar uma **tela de Splash (inicial)** em Flutter contendo uma **animação de movimento**, além de interação com o usuário e persistência de dados.

A aplicação apresenta uma imagem (logo) que se movimenta **de cima para baixo até o centro da tela**, juntamente com campos para inserção de dados e navegação entre telas.

---

## Objetivos

- Criar uma Splash Screen animada
- Implementar animação de movimento (de cima para baixo)
- Coletar dados do usuário (nome e idade)
- Armazenar dados localmente
- Navegar entre telas
- Exibir os dados na tela principal

---

## Tecnologias Utilizadas

- Flutter
- Dart
- SharedPreferences (armazenamento local)

---

## Funcionalidades

### Splash Screen
- Exibe uma imagem (`logo.png`)
- A imagem inicia fora da tela e **desce até o centro**
- Contém:
  - Campo para digitar o nome
  - Campo para digitar a idade
  - Botão para entrar no app

### Armazenamento
- Utiliza **SharedPreferences**
- Salva:
  - Nome
  - Idade

### Tela Home
- Exibe:
  - Nome do usuário
  - Idade do usuário
- Possui botão para voltar à Splash

---

## Animação

A animação foi feita utilizando:

- `AnimationController`
- `Curves.easeOut`

E consiste em:
- Movimento vertical da imagem
- Início fora da tela
- Finalização no centro

---

## Armazenamento de Dados

Os dados são armazenados localmente usando:

```dart
SharedPreferences

