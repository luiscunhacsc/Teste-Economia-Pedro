# Economia A 11.º Ano — Guia Interativo do Pedro

Guia de estudo interativo, feito numa única página HTML, para rever conteúdos de **Economia A do 11.º ano** com explicações curtas, exemplos, fórmulas, armadilhas típicas, mini-quizzes, flashcards e uma rotina de resposta para testes.

O projeto não precisa de instalação, servidor, bundler, base de dados nem dependências externas. Basta abrir o ficheiro `index.html` num navegador moderno.

## Índice

- [Objetivo](#objetivo)
- [Funcionalidades](#funcionalidades)
- [Conteúdos cobertos](#conteúdos-cobertos)
- [Tecnologias usadas](#tecnologias-usadas)
- [Estrutura do projeto](#estrutura-do-projeto)
- [Como executar](#como-executar)
- [Como usar o guia](#como-usar-o-guia)
- [Persistência de progresso](#persistência-de-progresso)
- [Impressão e modo resumo](#impressão-e-modo-resumo)
- [Responsividade](#responsividade)
- [Acessibilidade e usabilidade](#acessibilidade-e-usabilidade)
- [Como personalizar](#como-personalizar)
- [Como adicionar conteúdos](#como-adicionar-conteúdos)
- [Como adicionar perguntas ao quiz](#como-adicionar-perguntas-ao-quiz)
- [Como adicionar flashcards](#como-adicionar-flashcards)
- [Testes manuais recomendados](#testes-manuais-recomendados)
- [Limitações conhecidas](#limitações-conhecidas)
- [Ideias futuras](#ideias-futuras)
- [Licença](#licença)

## Objetivo

Este projeto transforma uma revisão tradicional de Economia A num material de estudo mais visual e ativo.

O foco principal é ajudar o aluno a:

- organizar a matéria por blocos;
- perceber relações de causa e efeito;
- distinguir conceitos parecidos;
- treinar respostas com linguagem económica;
- rever rapidamente antes de um teste;
- praticar com perguntas simples e flashcards;
- acompanhar o próprio progresso de revisão.

O tom do guia é direto e orientado para exame: menos texto longo, mais regras mentais, exemplos e alertas contra erros comuns.

## Funcionalidades

### Página estática completa

Todo o projeto vive em `index.html`, incluindo:

- HTML da interface;
- CSS do layout e tema visual;
- JavaScript da interação;
- conteúdos pedagógicos;
- quiz;
- flashcards;
- estado de progresso.

Não existem dependências externas.

### Navegação rápida

A página inclui:

- barra superior fixa;
- botões para abrir ou fechar todos os conceitos;
- botão para imprimir resumo;
- índice lateral com ligações internas;
- cartões de mapa mental para saltar entre blocos de matéria.

### Pesquisa integrada

O campo de pesquisa permite encontrar conceitos por texto visível ou por palavras-chave definidas em `data-tags`.

Exemplos de pesquisas úteis:

- `inflação`
- `PIB`
- `procura`
- `moeda`
- `UE`
- `Estado`
- `comércio externo`

Quando há pesquisa ativa, os cartões encontrados abrem automaticamente para facilitar a leitura.

### Filtros rápidos

A zona inicial tem chips de filtro para temas frequentes:

- Mercados
- Estado
- Moeda
- Famílias
- Comércio externo
- União Europeia

Cada filtro escreve automaticamente o termo no campo de pesquisa e mostra os conceitos relacionados.

### Cartões expansíveis

Os conceitos principais estão organizados em cartões expansíveis.

Cada cartão tem:

- título numerado;
- descrição curta;
- explicação;
- exemplos;
- fórmulas;
- caixas de memória;
- armadilhas típicas;
- frases-modelo quando aplicável.

### Progresso de revisão

O painel lateral inclui uma checklist de tópicos essenciais:

- Escassez e custo de oportunidade
- Tipos de consumo
- Procura, oferta e equilíbrio
- Inflação e poder de compra
- Mercado de trabalho
- Integração europeia

À medida que o aluno marca tópicos como dominados, o círculo de progresso atualiza a percentagem.

### Mini-quiz

O guia inclui quatro perguntas de aquecimento sobre:

- inflação e desinflação;
- concorrência perfeita;
- taxa de desemprego;
- consumo intermédio.

Ao escolher uma opção, o sistema:

- marca a resposta correta;
- assinala respostas erradas;
- mostra feedback textual;
- permite rever imediatamente a regra conceptual por trás da resposta.

### Flashcards

A secção de flashcards permite revisão ativa.

Os cartões viram ao clicar e cobrem conceitos como:

- custo de oportunidade;
- moeda escritural;
- Lei de Engel;
- excesso de procura;
- taxa de cobertura;
- mercado comum.

### Rotina de resposta em 5 passos

No fim da página existe uma rotina curta para perguntas com texto, tabela ou gráfico:

1. identificar o tema;
2. verificar a unidade;
3. perceber o período temporal;
4. encontrar a relação de causa e efeito;
5. responder com linguagem económica.

### Estilos de impressão

A folha inclui regras específicas em `@media print`.

Na impressão:

- a navegação é ocultada;
- a zona hero é ocultada;
- o quiz e flashcards são ocultados;
- os conceitos aparecem abertos;
- o fundo passa a branco;
- o texto passa a escuro;
- os cartões evitam quebras internas quando possível.

Isto permite gerar um resumo limpo em papel ou PDF.

## Conteúdos cobertos

O guia inclui 31 blocos principais:

1. O problema económico
2. Agentes económicos
3. Consumo
4. Investimento
5. Capital fixo e capital circulante
6. Produção e produtividade
7. Custos e escala
8. Lei de Engel e coeficientes orçamentais
9. Procura, oferta e equilíbrio
10. Deslocações da procura e da oferta
11. Estruturas de mercado
12. Moeda
13. Inflação, IPC e poder de compra
14. Valores nominais e reais
15. Rendimento disponível, consumo e poupança
16. Mercado de trabalho
17. PIB, VAB e Contabilidade Nacional
18. Setores de atividade económica
19. Estado, orçamento e política económica
20. Externalidades e eficiência económica
21. Pobreza e transferências sociais
22. União Europeia e integração económica
23. BCE e política monetária
24. Comércio externo e balança de bens
25. Balança corrente e de capital
26. Taxas de câmbio
27. Convergência real
28. Como ler tabelas e gráficos
29. Frases-modelo para respostas abertas
30. O essencial para a véspera
31. Estratégia mental para o teste

## Tecnologias usadas

| Tecnologia | Utilização |
| --- | --- |
| HTML5 | Estrutura da página e conteúdos |
| CSS3 | Layout, cartões, grelhas, tema visual, responsividade e impressão |
| JavaScript puro | Interações, pesquisa, filtros, quiz, flashcards e progresso |
| `localStorage` | Guardar progresso de revisão no navegador |

Não há:

- Node.js obrigatório;
- `npm install`;
- frameworks;
- bibliotecas externas;
- chamadas de rede;
- backend;
- base de dados.

## Estrutura do projeto

```text
.
├── index.html
└── README.md
```

### `index.html`

Contém a aplicação completa:

- `<style>` com todo o CSS;
- `<body>` com o conteúdo do guia;
- `<script>` com a lógica interativa.

### `README.md`

Documentação do projeto, instruções de uso e notas de manutenção.

## Como executar

### Opção 1: abrir diretamente

Abra o ficheiro `index.html` no navegador.

No Windows, pode usar:

```powershell
Start-Process .\index.html
```

### Opção 2: usar um servidor estático simples

Não é obrigatório, mas pode ser útil se quiser testar como site local.

Com Python:

```powershell
python -m http.server 8000
```

Depois abra:

```text
http://localhost:8000
```

## Como usar o guia

Fluxo recomendado para estudar:

1. Começar pelo mapa mental para perceber os grandes blocos.
2. Abrir os conceitos de um tema específico.
3. Ler a explicação e tentar reformular em voz alta.
4. Usar a pesquisa para procurar dúvidas concretas.
5. Fazer o mini-quiz sem consultar os cartões.
6. Rever os flashcards.
7. Marcar na checklist os tópicos já dominados.
8. Usar o botão de impressão para criar um resumo de revisão final.

Para revisão rápida, pode usar só:

- filtros rápidos;
- caixas de fórmulas;
- caixas de armadilhas;
- frases-modelo;
- bloco "O essencial para a véspera".

## Persistência de progresso

O progresso da checklist é guardado no navegador através de `localStorage`.

A chave usada é:

```text
ecoPedroProgress
```

Isto significa que:

- o progresso continua guardado depois de fechar a página;
- o progresso fica associado ao navegador e dispositivo usados;
- limpar dados do navegador pode apagar o progresso;
- abrir o ficheiro noutro computador começa com progresso vazio.

## Impressão e modo resumo

O botão **Imprimir resumo** chama:

```javascript
window.print()
```

As regras de impressão estão definidas em:

```css
@media print
```

Durante a impressão, o ficheiro esconde elementos interativos e privilegia o conteúdo de estudo.

Recomendação:

- escolher "Guardar como PDF" no diálogo de impressão;
- verificar se a opção de imprimir fundos está desligada, caso queira um PDF mais limpo;
- confirmar a pré-visualização antes de imprimir em papel.

## Responsividade

O layout adapta-se a vários tamanhos de ecrã.

Principais pontos de quebra:

- até `960px`: grelhas principais passam para uma coluna;
- até `640px`: mapas, flashcards e blocos de duas colunas passam para uma coluna;
- a barra superior reorganiza-se para evitar cortes;
- o índice deixa de ser sticky em ecrãs mais pequenos.

## Acessibilidade e usabilidade

O projeto já inclui algumas decisões úteis:

- estrutura semântica com `header`, `main`, `section`, `article`, `nav`, `aside` e `footer`;
- campo de pesquisa com `type="search"`;
- botões reais para ações interativas;
- navegação por âncoras;
- texto alternativo contextual em `aria-label` para zonas importantes;
- boa separação visual entre blocos;
- versão de impressão com contraste alto.

Possíveis melhorias futuras:

- adicionar `aria-expanded` aos cartões expansíveis;
- permitir abrir e fechar cartões com Enter/Espaço no cabeçalho;
- indicar estado selecionado dos filtros com `aria-pressed`;
- melhorar a experiência de leitores de ecrã nos flashcards;
- adicionar modo claro ou controlo de contraste.

## Como personalizar

### Alterar cores

As cores principais estão em variáveis CSS no topo do `<style>`:

```css
:root {
  --bg: #111827;
  --bg-2: #0b1120;
  --text: #f8fafc;
  --gold: #fbbf24;
  --blue: #38bdf8;
  --green: #34d399;
  --red: #fb7185;
}
```

Altere estas variáveis para mudar o tema global sem editar cada componente individualmente.

### Alterar largura máxima

A largura principal da página é controlada por:

```css
--max: 1180px;
```

### Alterar o nome do aluno

Procure por `Pedro` no `index.html` e substitua pelo nome pretendido.

Locais comuns:

- `<title>`;
- marca na barra superior;
- título principal;
- texto do rodapé;
- frases internas do conteúdo.

### Alterar filtros rápidos

Os filtros estão nesta zona:

```html
<button class="chip" data-filter="mercado">Mercados</button>
```

Para adicionar um filtro:

1. criar novo botão com classe `chip`;
2. definir `data-filter`;
3. garantir que os conceitos relevantes têm esse termo em `data-tags`.

## Como adicionar conteúdos

Cada conceito segue esta estrutura:

```html
<article class="concept" id="novo-conceito" data-tags="palavras chave para pesquisa">
  <div class="concept-header">
    <div class="icon">📘</div>
    <div>
      <h3>32. Título do conceito</h3>
      <p class="mini">Resumo curto do conceito.</p>
    </div>
    <div class="toggle">+</div>
  </div>
  <div class="concept-body">
    <p>Explicação do conceito.</p>
    <div class="formula">Fórmula ou regra importante</div>
    <div class="memory-box"><strong>Memória:</strong> pista para recordar.</div>
    <div class="trap-box"><strong>Armadilha:</strong> erro comum a evitar.</div>
  </div>
</article>
```

Depois de adicionar o artigo:

1. confirmar que está dentro de `<div id="concepts">`;
2. adicionar uma ligação no índice rápido, se fizer sentido;
3. adicionar `data-tags` úteis para pesquisa;
4. testar abrir, fechar e pesquisar.

## Como adicionar perguntas ao quiz

As perguntas do quiz usam `data-answer` no cartão e `data-option` em cada botão.

Exemplo:

```html
<article class="quiz-card" data-answer="b">
  <h3>Pergunta?</h3>
  <div class="quiz-options">
    <button class="option" data-option="a">Opção A</button>
    <button class="option" data-option="b">Opção B correta</button>
    <button class="option" data-option="c">Opção C</button>
  </div>
  <div class="feedback"></div>
</article>
```

O JavaScript deteta automaticamente cartões com `.quiz-card`.

## Como adicionar flashcards

Cada flashcard segue esta estrutura:

```html
<div class="flashcard">
  <div class="flash-inner">
    <div class="flash-face">Frente do cartão</div>
    <div class="flash-face flash-back">Resposta no verso.</div>
  </div>
</div>
```

O JavaScript deteta automaticamente `.flashcard` e alterna a classe `flipped` ao clicar.

## Testes manuais recomendados

Depois de editar o projeto, testar:

- abrir a página no navegador;
- clicar em "Abrir tudo";
- clicar em "Fechar tudo";
- abrir e fechar conceitos individuais;
- pesquisar por `inflação`, `PIB`, `procura`, `UE` e `moeda`;
- clicar em todos os filtros rápidos;
- limpar a pesquisa;
- marcar e desmarcar itens da checklist;
- recarregar a página e confirmar que o progresso persiste;
- responder ao mini-quiz com opções certas e erradas;
- virar todos os flashcards;
- usar o botão de impressão;
- testar em largura de telemóvel;
- testar em largura de desktop.

## Limitações conhecidas

- O progresso é local ao navegador; não sincroniza entre dispositivos.
- Não existe painel de administração para editar conteúdos.
- Não existe sistema de pontuação acumulada no quiz.
- Os conteúdos estão embutidos diretamente no HTML.
- Não há testes automatizados.
- O guia está orientado para o programa e estilo de revisão representados no ficheiro atual; deve ser revisto se o currículo ou critérios de avaliação mudarem.

## Ideias futuras

Possíveis evoluções:

- modo claro/escuro;
- contador de perguntas certas no quiz;
- banco maior de perguntas;
- perguntas aleatórias;
- exportação de progresso;
- separação dos conteúdos para JSON;
- página de edição de conceitos;
- mais flashcards;
- revisão espaçada por datas;
- suporte para várias disciplinas;
- versão PWA para uso offline instalado no telemóvel;
- melhorias de acessibilidade com estados ARIA completos.

## Licença

Este projeto ainda não declara uma licença formal.

Se for partilhado publicamente, recomenda-se adicionar uma licença explícita, por exemplo:

- MIT, se a intenção for permitir reutilização livre;
- Creative Commons, se o foco for o conteúdo pedagógico;
- "Todos os direitos reservados", se o objetivo for uso privado.

