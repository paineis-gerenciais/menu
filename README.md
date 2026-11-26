# menu

Menu geral dos Painéis Gerenciais: a marca no alto e um botão para cada painel (abre em nova aba).

Publicação: GitHub Pages → https://paineis-gerenciais.github.io/menu/

## Arquivos

- `index.html` — menu (HTML + CSS, sem JavaScript). A marca e os botões são feitos em código, não em imagem.
- `em-breve.html` — destino do botão "Outros".
- `favicon.svg` e `assets/icone-180.png` — ícones da aba do navegador e do celular.
- `assets/` — também guarda a arte antiga (`logo.webp`, `fundo.webp` e `btn-*.webp`). Ela não é mais usada pela página e pode ser apagada.

A marca (símbolo, assinaturas, cores e regras de uso) fica no repositório `padroes`, pasta `marca/`.

## Adicionar ou trocar um painel

Cada botão é um `<li>` em `index.html`.

- **Trocar o endereço:** edite o `href` do `<li>`.
- **Adicionar:** copie um `<li>` existente e troque quatro coisas: o endereço (`href`), a descrição lida por leitores de tela (`aria-label`), a linha de cima (`class="linha"`) e o nome (`class="nome"`).
- **Ícone:** é o desenho dentro de `<svg>`. Dá para repetir um ícone existente ou pedir um novo.
- O botão "Outros" deve ser sempre o último: insira novos painéis acima dele.

## Colocar a imagem de fundo (opcional)

Sem imagem, o fundo é marfim liso.

1. Gere a imagem com o prompt do `ARTE.md` (repositório `geral`) e salve em `assets/fundo-sobrio.webp` (1920 px de largura).
2. No alto do `index.html`, troque `--fundo: none;` por `--fundo: url("assets/fundo-sobrio.webp");`.
