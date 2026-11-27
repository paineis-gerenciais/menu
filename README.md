# menu

Menu geral dos Painéis Gerenciais: a marca no alto e um botão para cada painel (abre em nova aba).

Publicação: GitHub Pages → https://paineis-gerenciais.github.io/menu/

## Arquivos

- `index.html` — menu (HTML + CSS, sem JavaScript). A marca e os botões são feitos em código, não em imagem.
- `em-breve.html` — destino do botão "Outros".
- `favicon.svg` e `assets/icone-180.png` — ícones da aba do navegador e do celular.
- `assets/fundo-sobrio.webp` — imagem de fundo.
- `assets/` — também guarda a arte antiga (`logo.webp`, `fundo.webp` e `btn-*.webp`). Ela não é mais usada pela página e pode ser apagada.

A marca (símbolo, assinaturas, cores e regras de uso) fica no repositório `padroes`, pasta `marca/`.

## Adicionar ou trocar um painel

Cada botão é um `<li>` em `index.html`.

- **Trocar o endereço:** edite o `href` do `<li>`.
- **Adicionar:** copie um `<li>` existente e troque quatro coisas: o endereço (`href`), a descrição lida por leitores de tela (`aria-label`), a linha de cima (`class="linha"`) e o nome (`class="nome"`).
- **Ícone:** é o desenho dentro de `<svg>`. Dá para repetir um ícone existente ou pedir um novo.
- O botão "Outros" deve ser sempre o último: insira novos painéis acima dele.

## Imagem de fundo

O fundo é a imagem `assets/fundo-sobrio.webp`, com um véu marfim por cima para não disputar com os botões. O prompt que gerou a imagem está no `ARTE.md` do repositório `geral`.

- **Trocar a imagem:** salve a nova por cima de `assets/fundo-sobrio.webp` (1920 px de largura, até 300 KB).
- **Clarear ou escurecer:** no alto do `index.html`, mude o último número de `--veu`. Mais perto de `1` clareia; mais perto de `0` mostra mais a imagem.
- **Tirar a imagem:** no alto do `index.html`, troque o valor de `--fundo` por `none`. O fundo volta ao marfim liso.
