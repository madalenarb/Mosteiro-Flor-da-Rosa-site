# Mosteiro de Flor da Rosa: o site como projeto

Versão de 15 de novembro de 2026. É a mesma página publicada em https://claude.ai/artifact/VMvbfvEE7nYunHQFEBnbR3, aqui como projeto com ficheiros separados, e funciona sem internet.

## Abrir

Descomprima a pasta inteira e abra `index.html` no navegador (duplo clique). Não precisa de servidor nem de internet: as fotografias, os mapas e as letras vêm na pasta.

Para pôr o site na web, envie a pasta tal como está para um alojamento de páginas estáticas, por exemplo Netlify Drop ou GitHub Pages. A página de entrada é `index.html`.

## O que está em cada pasta

- `index.html`: a página, com os textos fixos em português, inglês e neerlandês e os desenhos das plantas, guardados como `<template>`.
- `css/estilo.css`: o aspeto. O modo claro é o de origem; o escuro e o automático escolhem-se no menu, em «Aspeto».
- `css/fontes.css` e `fontes/`: as letras Barlow, Barlow Semi Condensed e EB Garamond, com as licenças.
- `js/app.js`: o funcionamento (menu, mapas, linha do tempo, fotografias) e os textos que mudam com a língua, como a linha do tempo, as legendas das fotografias e as etiquetas dos mapas.
- `js/dados.js`: as plantas numeradas de 1980, as notas da planta de 1615 e as histórias com as fontes.
- `photos/` e `thumbs/`: as fotografias, em tamanho grande e em miniatura.
- `maps/`: os mapas da Flor da Rosa e do Crato e da Rota Histórica (PR1). `elev/`: as imagens dos alçados.
- `plan.jpg`: a planta manuscrita de 1615.
- `desenhos/`: os desenhos em SVG, para imprimir ou abrir num programa de desenho. As plantas de hoje (pisos 0 a 6) estão todas na mesma moldura, por isso sobrepõem-se certas. Os alçados usam as imagens de `elev/`; mantenha as duas pastas juntas.

## Mudar textos

Cada texto existe em três línguas. Em `js/app.js` e `js/dados.js` aparecem como `{pt:"…",en:"…",nl:"…"}`; em `index.html`, como blocos com `data-l="pt"`, `data-l="en"` e `data-l="nl"`. Depois de editar, guarde o ficheiro e recarregue a página.

## Créditos

- Mapas: dados © OpenStreetMap contributors (ODbL).
- Letras: SIL Open Font License.
- Fotografias: as suas, exceto as dos painéis da exposição do mosteiro e as fotografias de terceiros dos arredores (por exemplo, o interior da Igreja Matriz do Crato, de Rui Ponte e Sousa, 2017). Antes de publicar o site, confirme que pode usá-las.

## In English

The same page as the published one, as a multi-file project that works offline: unzip the whole folder and open `index.html`. Styles are in `css/`, code and texts in `js/` (every text has `pt`, `en` and `nl` versions), images in `photos/`, `thumbs/`, `maps/` and `elev/`, and the SVG drawings in `desenhos/`. To put it online, upload the folder as it is to any static host.
