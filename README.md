# 🎬 Simulador Funcional de Assinaturas (Streaming)

Sistema web desenvolvido em **HTML, CSS e JavaScript**, aplicando os **conceitos de Programação Funcional** exigidos no trabalho da disciplina **Linguagem de Programação e Paradigmas** (Prof. Esp. Ademar Perfoll Junior).

Tema escolhido: **Streaming / Assinaturas (planos, upgrades/downgrades e cálculo pró-rata)**.

---

## 📘 Descrição Geral

A aplicação simula um ambiente de **gestão de assinaturas de streaming**, permitindo:

- Registrar **assinaturas** com datas de início e término.  
- Realizar **mudanças de plano** (upgrade/downgrade).  
- Aplicar **promoções temporárias** com descontos percentuais.  
- Calcular **valores pró-rata** por dias no período selecionado.  
- Exibir **métricas de desempenho** do negócio:
  - **ARPU (Average Revenue Per User)**
  - **Churn Rate (Taxa de Cancelamento)**

---

## 🧠 Conceitos de Programação Funcional Utilizados

O projeto foi implementado **sem classes ou mutação direta de estado**, seguindo os princípios da **Programação Funcional (FP)**.

| Conceito | Aplicação no Projeto |
|-----------|----------------------|
| **Funções puras** | Cálculos de dias, interseção de períodos, pró-rata e métricas (ARPU/Churn). Nenhuma dessas funções altera variáveis externas. |
| **Imutabilidade** | O estado (`state.subscriptions`) é recriado com o operador `spread` (`...`) a cada modificação. |
| **Funções de ordem superior** | Uso de `map`, `filter`, e `reduce` para transformar listas e acumular valores. |
| **Validação pura** | Funções como `validateSubscriptionInput` e `isPositiveNumber` não dependem de variáveis globais. |
| **Separação de efeitos colaterais** | A manipulação da interface (DOM) é feita em funções separadas, isolando os efeitos do restante da lógica. |


---

## ⚙️ Como Executar

1. Baixe ou clone o repositório:
   ```bash
   git clone https://github.com/SeuUsuario/projeto-streaming.git
