# assets/

Coloque aqui a foto real da Dra. Gina Montezuma com o nome exato:

```
gina-retrato.jpg
```

O `dra-gina-montezuma.html` já está referenciando esse caminho (`assets/gina-retrato.jpg`)
no hero e na seção de autoridade/credenciais. Assim que o arquivo existir aqui, a foto
aparece automaticamente nos dois lugares — nenhuma edição de código é necessária.

Se preferir outro nome de arquivo ou formato (`.png`, `.webp`), basta trocar o valor do
atributo `src="assets/gina-retrato.jpg"` nas duas tags `<img>` do HTML.

## Por que está vazio
A Dra. Gina enviou uma foto real no chat (retrato, fundo escuro, blusa preta drapeada,
brincos), mas o ambiente onde este site foi montado não tem acesso ao arquivo de imagem
em disco — só recebe a imagem para leitura visual, não para salvar como arquivo. Por isso
o HTML já está pronto para usar a foto, mas o arquivo em si precisa ser adicionado
manualmente (por quem tiver o arquivo original) para a foto passar a aparecer no lugar do
placeholder tracejado.
