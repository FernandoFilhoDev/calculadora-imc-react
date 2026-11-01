# 🧮 Calculadora de IMC

Aplicação web feita com **React** e **Vite** que calcula o Índice de Massa Corporal (IMC), mostra a classificação do resultado e exibe a tabela de referência completa.

![Prévia da calculadora de IMC](./screenshots/preview.png)

## ✨ Funcionalidades

- Cálculo do IMC a partir de altura e peso
- Aceita vírgula como separador decimal (ex.: `1,75` e `70,5`)
- Bloqueia caracteres inválidos nos campos (só números e vírgula)
- Classificação do resultado com cor de acordo com a faixa
- Tabela de referência com todas as classificações
- Botões para limpar o formulário e voltar ao cálculo

## 🛠️ Tecnologias

- [React](https://react.dev/)
- [Vite](https://vitejs.dev/)
- JavaScript (ES6+)
- CSS puro com Flexbox
- ESLint

## 📚 Conceitos praticados

- Hook `useState` para controle de estado
- Componentização e reaproveitamento (`Button`, `ImcCalc`, `ImcTable`)
- Comunicação entre componentes com props
- Renderização condicional (formulário ↔ resultado)
- Renderização de listas com `.map()`
- Dados separados da interface (`src/data/data.js`)

## 📁 Estrutura do projeto

```
src/
├── components/
│   ├── Button.jsx / Button.css
│   ├── ImcCalc.jsx / ImcCalc.css
│   └── ImcTable.jsx / ImcTable.css
├── data/
│   └── data.js
├── App.jsx / App.css
├── index.css
└── main.jsx
```

## 🚀 Como rodar o projeto

Pré-requisito: [Node.js](https://nodejs.org/) instalado.

```bash
# Clone o repositório
git clone https://github.com/FernandoFilhoDev/calculadora-imc-react.git

# Entre na pasta do projeto
cd calculadora-imc-react

# Instale as dependências
npm install

# Inicie o servidor de desenvolvimento
npm run dev
```

Depois, abra no navegador o endereço que aparecer no terminal (normalmente `http://localhost:5173`).

## 📊 Tabela de classificação

| IMC               | Classificação   | Obesidade |
| ----------------- | --------------- | --------- |
| Menor que 18,5    | Magreza         | 0         |
| Entre 18,5 e 24,9 | Normal          | 0         |
| Entre 25 e 29,9   | Sobrepeso       | I         |
| Entre 30 e 39,9   | Obesidade       | II        |
| 40 ou mais        | Obesidade grave | III       |

> Esta aplicação é um projeto de estudo e não substitui a avaliação de um profissional de saúde.

## 👨‍💻 Autor

Feito por **Fernando Filho**.

[![GitHub](https://img.shields.io/badge/GitHub-FernandoFilhoDev-181717?logo=github)](https://github.com/FernandoFilhoDev)
