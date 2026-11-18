# meusaldo-financas
# MeuSaldo — Gestão Patrimonial & Finanças Pessoais

Aplicação web responsiva de controle financeiro pessoal desenvolvida para a disciplina de **Desenvolvimento de Interfaces (2/2026)** — CEUB. O projeto tem como objetivo oferecer uma interface clássica, intuitiva e acessível para o gerenciamento mensal de receitas, despesas individuais e reserva de emergência, aplicando boas práticas de UI/UX, psicologia das cores, heurísticas de Nielsen e diretrizes de acessibilidade WCAG 2.1.

---

## 📋 Funcionalidades e Componentes Implementados

- **Barra de Acessibilidade (WCAG 2.1):** Controles no topo da interface para redimensionamento tipográfico (`A-`, `A`, `A+`) e alternância dinâmica entre **Modo Claro** e **Modo Escuro** com contrastes validados (AA/AAA).
- **Painel Consolidado (Dashboard):** Exibição de cartões de indicadores-chave (*Receitas Totais*, *Despesas Totais*, *Reserva de Emergência* e *Saldo Livre*) com alinhamento numérico tabular (`tabular-nums`).
- **Alerta Inteligente de Saldo Negativo:** Banner de aviso automático acionado sempre que as despesas e reservas superam as receitas registradas no período.
- **Lançamento Único em Lote:** Tela dedicada ao preenchimento simultâneo de entradas, categorias de despesas e reserva, acompanhada de uma barra fixa inferior que calcula a prévia do saldo em tempo real.
- **Proteção de Reserva de Emergência:** Os valores destinados à reserva são descontados do saldo livre e destacados visualmente, prevenindo gastos acidentais.
- **Gráfico de Alocação Proporcional:** Gráfico de rosca (*Donut Chart* via Chart.js) com legenda dinâmica e cálculo percentual de cada categoria de saída.
- **Extrato com Abas de Pesquisa e Filtro:** Tabela interativa equipada com campo de busca textual em tempo real e botões de filtragem por tipo (`Todos`, `Receitas`, `Despesas`, `Reserva`).
- **Carrossel de Imagens e Cartões Explicativos:** Slider interativo com dicas financeiras e cartões metodológicos (*Pague-se Primeiro*, *Regra 50-30-20* e *Diagnóstico Visual*) para promover o engajamento do usuário.
- **Área de Login e Contato:** Páginas dedicadas à autenticação do usuário e ao envio de mensagens de suporte com validação de formulário.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

- **HTML5 Semântico:** Estruturação acessível com tags `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>` e atributos ARIA (`role`, `aria-label`, `aria-pressed`).
- **CSS3 Moderno:** Uso de variáveis CSS (`:root`) para troca instantânea de temas, layouts responsivos com **CSS Grid** e **Flexbox**, e media queries para adaptação em dispositivos móveis.
- **JavaScript (ES6+):** Manipulação dinâmica do DOM, cálculos financeiros em tempo real, filtragem combinada (texto + categoria), controle do carrossel e validação de formulários.
- **Chart.js (v4.4.1):** Biblioteca JavaScript utilizada para renderizar o gráfico de rosca interativo.
- **Google Fonts:** Combinação tipográfica entre *Playfair Display* (títulos clássicos) e *Inter* (leitura clara de dados e valores monetários).

---

## 🚀 Passo a Passo da Construção do Projeto

1. **Planejamento Visual e Definição da Paleta:** Escolha das cores institucionais (Azul-Marinho `#14274E`, Dourado `#B8964F` e Off-White `#F8F7F4`) combinadas às cores semânticas (Verde Esmeralda `#1E6B4B` e Vermelho Carmim `#A61C14`), validando as taxas de contraste no padrão WCAG.
2. **Estruturação Base em HTML5:** Criação do esqueleto semântico em página única (*Single Page Application* leve), dividindo a navegação nas abas *Painel Financeiro*, *Lançamentos*, *Contato* e *Login*.
3. **Estilização e Design System em CSS3:** Implementação dos cartões de KPI, tabelas responsivas, formulários em grade e definição das variáveis cromáticas para o tema escuro (`body.dark-mode`).
4. **Lógica Financeira e Gráficos em JavaScript:** Desenvolvimento das funções de cálculo consolidado, prévia em tempo real na barra de lançamentos, disparo do alerta de saldo negativo e integração com o Chart.js.
5. **Implementação de Acessibilidade e Engajamento:** Inclusão da barra superior de acessibilidade (fonte e tema), do carrossel de imagens automático/manual e dos cartões explicativos de educação financeira.
6. **Versionamento e Publicação no GitHub:** Criação do repositório, organização do histórico de commits por funcionalidade e ativação do GitHub Pages para disponibilização online.

---

## 📂 Estrutura de Arquivos

```text
meusaldo-financas/
├── index.html      # Estrutura HTML, estilos CSS e lógica JavaScript consolidados
└── README.md       # Documentação técnica e guia do projeto
