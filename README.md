# Interface Clara

Site de demonstração de **usabilidade, experiência do usuário (UX), acessibilidade e responsividade**, feito somente com HTML e CSS .

## 1. Acesso ao site

| Item | Endereço |
|---|---|
| Site (GitHub Pages) | `https://camargo-projetos.github.io/Cria-o-de-Interfaces/` |


## 2. Páginas e navegação

| Página | Arquivo | Responsável |
|---|---|---|
| Início | `index.html` | João Manoel |
| Usabilidade | `heuristicas.html` | João Manoel |
| Experiência (UX) | `ux.html` | João Manoel |
| Cores e tipografia | `cores-tipografia.html` | Lucas Samuel |
| Acessibilidade | `acessibilidade.html` | Lucas Samuel |
| Responsividade | `responsividade.html` | Lucas Samuel |

Todas as páginas compartilham o mesmo cabeçalho, menu e rodapé. Cada página interna tem caminho “Você está em”, índice “Nesta página” e botões “Anterior” e “Próxima”.

## 3. Tarefas por integrante

| Integrante | Tarefas |
|---|---|
| João Manoel Camargo | Estrutura do projeto, `css/base.css` (variáveis, menu, rodapé, botões, cartões, tabelas), páginas Início, Usabilidade e Experiência (UX), seções 4.1 e 4.2 deste README |
| Lucas Samuel dos Santos | Páginas Cores e tipografia, Acessibilidade e Responsividade, seções 4.3, 4.4 e 4.5 e instruções de execução deste README |

## 4. Conceitos aplicados e escolhas de design

### 4.1 Usabilidade (heurísticas de Nielsen)

| Heurística | Escolha de design |
|---|---|
| 1. Visibilidade do status | Página atual destacada no menu (fundo branco e sublinhado) e caminho “Você está em” |
| 2. Mundo real | Linguagem simples em português; rótulos como “Enviar mensagem” |
| 3. Controle e liberdade | Menu em todas as páginas, “Anterior/Próxima”, “Voltar ao topo”, botão “Limpar campos” |
| 4. Consistência | Mesmo cabeçalho, rodapé e estilo de botões em todas as páginas |
| 5. Prevenção de erros | Campos `required`, `type="email"` e `maxlength` no formulário |
| 6. Reconhecimento | Menu sempre com nomes claros; símbolos sempre acompanhados de texto |
| 7. Flexibilidade | Link “Pular para o conteúdo”, cartões como atalhos, índice lateral |
| 8. Minimalismo | Poucas cores, espaço em branco e uma ideia por seção |
| 9. Recuperar de erros | Dicas de preenchimento e validação nativa do navegador |
| 10. Ajuda | Seção “Ajuda: como navegar” na página inicial |

### 4.2 Experiência do usuário (UX)

| Conteúdo da aula | Escolha de design |
|---|---|
| Cinco planos (estratégia, escopo, estrutura, esqueleto, superfície) | Cada plano tem uma decisão registrada na página `ux.html` |
| Prototipação baixa e alta fidelidade | O site em HTML/CSS funciona como protótipo de alta fidelidade |
| Signos e engenharia semiótica | Símbolos (←, →, ↑, ›, ✓, ✗) sempre acompanhados de texto |
| Fluxo de navegação | Caminho curto: Início → tema → leitura → “Próxima” |

### 4.3 Cores e tipografia

| Conteúdo da aula | Escolha de design |
|---|---|
| Associar significado às cores | Azul (calma) como cor principal; laranja (dinamismo) só em botões de ação |
| Não usar a mesma cor para funções distintas | Laranja nunca é usado em links ou títulos |
| Manter padrão de cores | Mesmas variáveis CSS (`:root`) em todas as páginas |
| Fonte sem serifa para produtos digitais | Fonte do sistema, sem serifa |
| Evitar caixa alta em textos longos | Todo o texto em caixa baixa; caixa alta aparece só como exemplo do que evitar |
| Legibilidade | Texto de 17 px, entrelinha de 1,65 e linhas de até 48rem |

### 4.4 Acessibilidade

| Princípio (WCAG) | Escolha de design |
|---|---|
| Perceptível | Contraste mínimo de 4,5:1 em todos os pares de texto e fundo; símbolos decorativos com `aria-hidden` |
| Operável | Navegação completa por teclado, contorno de foco visível, link “Pular para o conteúdo”, alvos de 44 px no menu, botões e índice |
| Compreensível | `lang="pt-BR"`, menu igual em todas as páginas, rótulos e dicas nos campos do formulário |
| Robusto | HTML semântico (`header`, `nav`, `main`, `section`, `footer`) e `aria-current` na página atual |

### 4.5 Responsividade

| Técnica | Escolha de design |
|---|---|
| Abordagem mobile-first | CSS base para telas pequenas; regras para telas maiores em `@media (min-width: …)` |
| Pontos de quebra | `40em` (tablet) e `64em` (computador) |
| Layout fluido | `grid` com `repeat(auto-fit, minmax(…, 1fr))` e menu com `flex-wrap` |
| Mídias flexíveis | Tabelas com rolagem horizontal dentro de um contêiner |
| Tipografia fluida | Títulos com `clamp()` |

## 5. Como executar localmente

1. Baixar ou clonar o repositório.
2. Abrir o arquivo `index.html` em um navegador. Não é preciso instalar nada.

## 6. Estrutura de arquivos

```
index.html            heuristicas.html     ux.html
cores-tipografia.html acessibilidade.html  responsividade.html
css/
  base.css            estilos compartilhados
  home.css            heuristicas.css      ux.css
  cores-tipografia.css acessibilidade.css  responsividade.css
```
