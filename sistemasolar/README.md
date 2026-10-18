# Trabalho 2 - CSS: Conhecendo o Sistema Solar

Site educativo em HTML e CSS puro, sem bibliotecas CSS ou JavaScript.

## Fotografias da NASA

A galeria usa quatro registros reais de missões espaciais, da Terra, Marte, Júpiter e Saturno. Algumas imagens são mosaicos feitos com várias fotografias, não desenhos gerados digitalmente.

**Importante:** por padrão, as fotografias são carregadas dos servidores da NASA, portanto precisam de conexão à internet.

**Para colocar todas as fotos na pasta de imagens antes da entrega**, no Windows:

1. Clique duas vezes no arquivo `baixar-fotos-nasa.bat` estando conectado à internet.
2. Aguarde a mensagem de confirmação: o programa salva as quatro fotos em `docs/imagens` e altera automaticamente o HTML para usar os arquivos locais.
3. Confira que aparecem os arquivos `terra.jpg`, `marte.jpg`, `jupiter.jpg`, `saturno.jpg` na pasta `docs/imagens`.
4. Envie a pasta `docs` já com as fotos baixadas para o GitHub.

Se preferir, pode baixar as imagens manualmente das páginas da NASA listadas em "Referências das fotografias" abaixo e salvar com os nomes acima. Depois troque o `src` de cada imagem no HTML pelo endereço `imagens/nome.jpg`.

## Organização dos arquivos

```text
sistema-solar-simples/
├── README.md
├── baixar-fotos-nasa.bat
├── baixar-fotos-nasa.ps1
└── docs/
    ├── index.html
    ├── css/
    │   ├── modern-normalize.css
    │   └── style.css
    └── imagens/
        ├── logo.svg
        ├── ordem-planetas.svg
        ├── tipos-planetas.svg
        └── terra.jpg, marte.jpg, jupiter.jpg, saturno.jpg  (após executar o .bat)
```

## Como abrir e apresentar

Abra `docs/index.html` no navegador. O menu usa `<details>` e `<summary>` sem JavaScript. O `<nav>` contém quatro opções, sendo duas correspondentes às seções atuais. A galeria usa Flexbox (`display: flex`, `flex-wrap: wrap`) e se ajusta para uma coluna no celular com `@media`. O `<header>` usa `position: sticky`.

## Como publicar no GitHub Pages

1. Antes, execute `baixar-fotos-nasa.bat` para colocar as fotografias na pasta do trabalho.
2. Crie um repositório público no GitHub.
3. Adicione a pasta `docs` e o `README.md`.
4. Vá em **Settings > Pages > Build and deployment** e escolha branch `main`, pasta `/docs`.
5. Acesse o endereço do site disponibilizado pelo GitHub e teste.

## Referências dos textos

- NASA - https://science.nasa.gov/solar-system/solar-system-facts/
- NASA - https://science.nasa.gov/solar-system/planets/
- NASA - https://science.nasa.gov/sun/facts/

## Referências das fotografias

- Terra (PIA18033): NASA - https://science.nasa.gov/photojournal/earth/
- Marte (PIA00407): NASA/JPL/USGS - https://science.nasa.gov/photojournal/global-color-views-of-mars/
- Júpiter (PIA04866): NASA/JPL/Space Science Institute - https://science.nasa.gov/photojournal/cassini-jupiter-portrait/
- Saturno (PIA21345): NASA/JPL-Caltech/Space Science Institute - https://science.nasa.gov/photojournal/so-far-from-home/

## Validadores

- HTML: https://validator.w3.org/
- CSS: https://jigsaw.w3.org/css-validator/
- WAVE: https://wave.webaim.org/
- PageSpeed computador e celular: https://pagespeed.web.dev/

As notas e os testes oficiais só podem ser confirmados depois da publicação. `modern-normalize.css` é baseado no projeto MIT https://github.com/sindresorhus/modern-normalize.
