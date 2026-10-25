# Jornal Imoral

## 1. Nome do projeto
**Jornal Imoral**

## 2. Integrantes
Tallys Rafael Silva de Araújo e 
Martiniano

## 3. Tema escolhido
Jornal satírico de desinformação (notícias falsas, feitas de forma fictícia e humorística). A manchete de exemplo anuncia que "Romerito Campos de Andrade foi eleito presidente do Brasil com 60% dos votos". Todo o conteúdo é fictício.

## 4. Tipo de layout escolhido
Layout de **portal de notícias**, em uma única página (*one page*), com:
- barra de navegação no topo (navbar) com logo, busca e menu;
- seção de destaque (*hero*) com a manchete principal em duas colunas: texto à esquerda e imagem à direita.

O layout é construído com **Flexbox** e usa a nomenclatura **BEM** nas classes CSS (`navbar__logo`, `hero__titulo`, etc.).

## 5. Objetivo da página
Apresentar a manchete principal do jornal com destaque visual e permitir a navegação pelas seções da página (Manchete Principal, Últimas Notícias e Newsletter). A página funciona como a base (*front-end*) de um jornal online fictício.

## 6. Componentes simples
Elementos únicos, que não dependem de outros para existir:

| Componente | Classe | Descrição |
|---|---|---|
| Logo | `navbar__logo` | Imagem do logo do jornal (150x100 px) |
| Campo de busca | `navbar__search` | `input type="search"` com bordas arredondadas |
| Item de menu | `navbar__item` | Link em formato de botão arredondado, com efeito `:hover` |
| Badge | `badge` / `hero__badge` | Etiqueta "Urgente" sobre a manchete |
| Título da manchete | `hero__titulo` | `h1` com a manchete principal |
| Texto da manchete | `hero__text` | Parágrafo de apoio da notícia |
| Imagem principal | `hero__img` | Imagem ilustrativa da manchete (420 px de altura) |

## 7. Componentes compostos
Componentes formados pela combinação de componentes simples:

| Componente | Classe | Composto por |
|---|---|---|
| Menu de navegação | `navbar__menu` | Lista (`ul`) com vários itens de menu (`navbar__item`) |
| Barra de navegação (Navbar) | `navbar` | Logo + campo de busca + menu de navegação |
| Seção Hero (manchete principal) | `hero` | Coluna de texto (badge + título + texto) + coluna da imagem principal |

## 8. Onde o Flexbox foi utilizado
Arquivo: `trabalho_do_terceiro/style.css`

- **`.navbar`**: `display: flex; justify-content: space-between; align-items: center;`. Coloca logo, busca e menu na mesma linha, com espaço entre eles e alinhados verticalmente ao centro.
- **`.navbar__menu`**: `display: flex; gap: 18px;`. Deixa os itens do menu lado a lado, com espaçamento entre eles.
- **`.hero`**: `display: flex; justify-content: space-between;`. Divide a seção em duas colunas, com o texto de um lado e a imagem do outro.

## 9. Diário de bordo
> **Preencher:** adicione aqui o link ou a descrição do diário de bordo.

Link: _(inserir link do diário de bordo)_

Modelo de descrição, se preferir escrever aqui:
- **Etapa 1:** definição do tema e do nome do jornal.
- **Etapa 2:** estruturação do HTML (navbar e hero).
- **Etapa 3:** estilização com CSS e organização com Flexbox.
- **Etapa 4:** testes e ajustes finais.

## 10. Observações sobre o uso de IA.
Poucas vezes ou nulas ultilizamos a IA.

# 11. Instruções para abrir o projeto
1. Baixe o projeto (**Code > Download ZIP** no GitHub) ou clone o repositório:
   ```bash
   git clone https://github.com/<seu-usuario>/Jornal-Imoral.git
   ```
2. Se baixou o ZIP, extraia a pasta.
3. Abra a pasta `trabalho_do_terceiro`.
4. Dê dois cliques em **`index.html`** para abrir no navegador (Chrome, Edge, Firefox etc.).
   - Alternativa: no VS Code, clique com o botão direito em `index.html` e escolha **Open with Live Server**.

### Estrutura de pastas
```
Jornal-Imoral/
├── README.md
└── trabalho_do_terceiro/
    ├── index.html
    ├── style.css
    └── Imagens/
        ├── IMG_LOGO.png
        └── IMG_PRINCIPAL.png
```
