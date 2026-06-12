# 💸 App de Organização de Finanças Pessoais com Vibe Coding

# Finny — Finanças Pessoais Sem Esforço

> **Desafio de Projeto:** Desenvolvido para a plataforma **DIO (Digital Innovation One)**   
> **Status do Projeto:** Concluído  
> **Plataforma de Desenvolvimento:** Lovable (Web App)  
> **Banco de Dados:** Supabase / PostgreSQL  

O **Finny** é um aplicativo web para gestão de finanças pessoais criado de forma ágil durante um desafio prático da **DIO**. O objetivo do projeto foi estruturar um **PRD (Product Requirement Document)** completo para guiar uma Inteligência Artificial (Lovable) na construção de uma ferramenta que elimina a complexidade e a burocracia das planilhas tradicionais.

---

## Sobre o App

O Finny foi desenhado para ser uma ferramenta "anti-planilha". Em vez de tabelas chatas e formulários longos, o usuário interage com o app de forma natural, rápida e visual.

### Diferenciais do Produto
* **Registro em 3 Segundos:** Chega de perder tempo digitando detalhes. O app conta com um motor de Inteligência Artificial que entende o que você escreve e anota seu gasto automaticamente.
* **Mascote Dinâmico:** Uma baleia fofa e simpática acompanha sua evolução financeira, reagindo ao seu saldo com empatia e sem julgamentos.
* **Indicador "Dinheiro Livre":** Mostra direto na tela o quanto você pode gastar na semana ou no mês sem passar sufoco.
* **Lojinha e Gamificação:** Registrar seus gastos com frequência rende moedas virtuais (*Finny Coins*) que servem para comprar roupinhas e acessórios para personalizar o seu mascote!

---

## Demonstração & Interações

Aqui estão os registros visuais do aplicativo funcionando:

### Interface do Aplicativo

<img width="1217" height="740" alt="finny " src="https://github.com/user-attachments/assets/90ead017-101b-4677-b6e3-08c8e13d1639" />
<img width="1221" height="750" alt="finny 2" src="https://github.com/user-attachments/assets/3c564701-1635-4a27-b93f-8aa6da16346f" />

*Tela principal mostrando o Dinheiro Livre, o Termômetro de Gastos e a nossa Baleia Mascote.* 

---

## Documento de Requisitos do Produto (PRD)

Este é o documento completo que serviu de guia e instrução base para a Inteligência Artificial estruturar e programar o aplicativo:

<details>
<summary><b>Clique aqui para abrir o PRD Completo 📄</b></summary>

### 1. Visão Geral do Produto
* **Proposta de valor:** Registro de transações em menos de 3 segundos.
* **Diferencial:** Interface minimalista + motor de IA em linguagem natural.
* **Experiência:** Mascote dinâmico e interativo (baleia fofa, simpática, sem traços infantis) que reduz a culpa e a ansiedade financeira.
* **Design:** Limpo, moderno e minimalista, seguindo a linha do Tailwind CSS.

### 2. Objetivos e Público-Alvo
* **Objetivos:** Reduzir o atrito na digitação, promover clareza visual da saúde financeira e humanizar o processo através de psicologia comportamental.
* **Público-Alvo:** Jovens adultos, estudantes e profissionais em início de carreira que abandonam ferramentas tradicionais por achá-las burocráticas ou punitivas.

### 3. Requisitos Funcionais

#### 3.1 Registro Inteligente por IA
Campo de texto simples onde o usuário digita livremente e a IA processa a frase:
* *“Gastei 45 reais de uber ontem à noite”* → Valor: R$ 45 | Tipo: Despesa | Categoria: Transporte
* *“Recebi 150 reais do freela de design hoje”* → Valor: R$ 150 | Tipo: Receita | Categoria: Renda Extra

#### 3.2 Teclado de Atalho Rápido
Teclado numérico simplificado com botões de categorias predefinidas (Alimentação, Transporte, Moradia, Lazer, Saúde) para salvar com apenas um clique.

#### 3.3 Dashboard Visual (Termômetro de Gastos)
Barra de progresso horizontal que indica a saúde financeira com base no limite de gastos definido.

#### 3.4 Indicador "Dinheiro Livre"
Cálculo em tempo real do valor disponível para uso:
$$D_{livre} = R_{total} - (D_{fixas} + M_{poupanca})$$

### 4. Mascote Dinâmico e Regras de Humor
A baleia reage ao estado do orçamento do usuário de forma empática:

| Status | Expressão Visual | Tom de Voz (Exemplo) |
| :--- | :--- | :--- |
| **Zona Verde** | Feliz, relaxada, com acessórios. | "Tudo sob controle! Você ainda tem R$ X livres para gastar sem culpa." |
| **Zona Amarela**| Atenta, pensativa, olhar curioso. | "Opa, percebi que seus gastos com delivery subiram. Que tal segurar a onda?" |
| **Zona Vermelha**| Determinada, estilo heróica. | "Eita, o orçamento apertou! Mas sem pânico, estou aqui para ajudar." |

### 5. Customização e Temas Visuais
* **Clássico Moderno:** Azul Slate — Profissional e limpo.
* **Menta Conforto:** Verde Sálvia — Tranquilidade e equilíbrio.
* **Terracota Quente:** Tons de Terra — Acolhedor e orgânico.
* **Minimalist Dark:** Preto e Cinza — Elegância e discrição.

### 6. Estrutura Técnica (Banco de Dados e Telas)
* **Tabelas (Supabase):** `Users` (dados e limites do usuário), `Transactions` (histórico de movimentações) e `AI_Insights` (mensagens e humor da baleia).
* **Telas (Lovable):**
    1. Dashboard Inicial (Resumos e Mascote).
    2. Janela de Entrada (Texto da IA ou Teclado Rápido).
    3. Extrato Histórico (Linha do tempo cronológica).
    4. Configurações (Troca de temas e lojinha).

### 7. Sistema de Gamificação (Lojinha e Conquistas)
Os usuários ganham *Finny Coins* ao manterem a consistência e cumprirem metas. Essas moedas podem ser trocadas por itens cosméticos para a baleia (óculos escuros, chapéus, gravatas, etc.).

#### Tabela de Progressão de Recompensas:
* **Primeiro Passo** (Registrar 1ª transação): 50 coins
* **Consistência Semanal** (Registrar por 5 dias seguidos): 100 coins
* **Disciplina Verde** (Fechar a semana na Zona Verde): 150 coins
* **Maratona Financeira** (30 dias seguidos de registro): 500 coins
* **Zero Dívida** (Um mês sem estourar o orçamento): 400 coins
* **Finny Master** (Completar todas as conquistas do app): 1000 coins

</details>

---

## Refinamentos & Evolução com o Lovable

Durante o processo de criação do **Finny**, utilizei prompts de refinamento para evoluir o aplicativo além do escopo inicial, adicionando novas ferramentas comportamentais e corrigindo regras de negócio complexas. Abaixo estão os comandos e lógicas implementados nas interações com a IA:

### 1. Novas Ferramentas e Personalização (Prompt de Expansão)
Solicitei à IA a criação da seção **## 8. Ferramentas Adicionais e Personalização de Dados** para tornar o app mais completo:
*   **Simulador de Sacrifício (*Psychological Budgeting*):** Uma ferramenta onde o usuário insere um gasto supérfluo recorrente (ex: cafezinho ou delivery) e o sistema projeta o acúmulo financeiro em 1 mês, 6 meses e 1 ano, vinculando o valor poupado a metas reais (como viagens ou eletrônicos).
*   **Divisor de Contas Rápido (*Social Share*):** Calculadora integrada para dividir despesas de grupo (churrascos, jantares). O sistema calcula a divisão e abate os reembolsos esperados do extrato para não distorcer o saldo real do usuário.
*   **Perfil Avançado (Calibragem da IA):** Diferenciação de perfis (Fixo/Clássico ou Freelancer) e um cadastro de compromissos fixos recorrentes que já retém o valor do "Dinheiro Livre" logo no início do mês.

### 2. Correção da Lógica de Ciclo Mensal e Receitas Extras
Para ajustar as regras financeiras do app que não estavam funcionando como o esperado no dia a dia, fiz o seguinte pedido de melhoria para a IA:
*   **Dia do Pagamento (Ciclo Dinâmico):** Substituição do reset fixo do dia 1 por um campo configurável de 1 a 31. Se o usuário recebe dia 5, o ciclo do termômetro e do dinheiro livre roda sempre do dia 5 ao dia 4 do próximo mês.
*   **Edição Prática do Orçamento:** Inclusão de um botão/engrenagem para permitir que o usuário altere sua receita fixa e limite de gastos a qualquer momento de forma simples.
*   **Entrada de PIX / Receitas Extras:** Ajuste no modal de registro rápido (`+ Registrar`). Agora, ao digitar *"Recebi um PIX de 50 reais"*, o valor é somado na hora ao Dinheiro Livre do mês atual, sem bagunçar a receita fixa configurada para os meses seguintes.

### 3. Ajustes Cruciais de Banco de Dados e Reset
No último ciclo de refinamento, apliquei alterações para melhorar os testes da aplicação:
*   **Lógica Direta do Dinheiro Livre:** Garantia de que qualquer ganho extra seja injetado direto no saldo disponível para gastar na semana/mês, atualizando a interface em tempo real.
*   **Botão de Reset Completo (*Recomeçar do Zero*):** Criação de uma função segura na aba de configurações que limpa todas as transações, limpa o extrato e apaga o histórico do banco de dados (Supabase) após uma confirmação, permitindo refazer testes do absoluto zero.

*   Resultado final no Lovable: https://finny-whale-buddy.lovable.app

---

## Reflexão sobre o Processo

### O que funcionou bem?
*   **Velocidade e Design Visual:** O Lovable conseguiu interpretar a proposta de uma interface minimalista e "anti-planilha" de forma muito ágil. O visual moderno com Tailwind CSS e a estrutura das telas ficaram excelentes logo de primeira.
*   **Engajamento com o Mascote:** A lógica de comportamento da baleia mascote e o sistema de pontuação por conquistas (Finny Coins) foram mapeados perfeitamente a partir do PRD, criando uma experiência divertida e leve.

### O que não funcionou como o esperado?
Durante os testes práticos da primeira versão gerada pela IA, notei que algumas regras de negócio essenciais de finanças do mundo real não funcionavam de forma fluida e precisaram de intervenção e refinamento:
*   **Ciclo Mensal Engessado:** O aplicativo calculava o orçamento iniciando sempre no dia 1º de cada mês, o que não reflete a realidade de quem recebe o salário em outras datas (como dia 5 ou quinto dia útil).
*   **Lógica de Receitas Extras (PIX):** Inicialmente, quando um ganho extra era registrado (ex: "Recebi um PIX de 50 reais"), o sistema não atualizava o "Dinheiro Livre" para uso imediato ou tentava alterar a receita fixa dos meses seguintes, gerando inconsistência no saldo atual.
*   **Falta de Flexibilidade e Ambiente de Testes:** Não havia uma forma simples de editar o orçamento fixo na tela principal e, durante o desenvolvimento, o banco de dados ficava poluído com transações antigas, pois não existia uma função de "Reset" para limpar o histórico e recomeçar os testes do zero.

### O que aprendi sobre conversar com IAs?
*   **Iteração é a Chave:** Aprendi que o primeiro resultado da IA raramente será o produto final perfeito. O segredo está em testar o app como um usuário real, identificar os gargalos de lógica e usar prompts de refinamento bem direcionados para corrigir os fluxos.
*   **Clareza em Regras de Negócio:** Quanto mais específico eu sou ao descrever o comportamento esperado (como detalhar que o ciclo deve ir do *dia X ao dia Y do próximo mês*), mais assertiva a IA é na hora de reestruturar o código e o banco de dados.
  
---
