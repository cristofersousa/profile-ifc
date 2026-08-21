# Meu Portal Pessoal

Projeto desenvolvido na disciplina de **Desenvolvimento Web I**.

A proposta é transformar a página de perfil criada na primeira aula em um
pequeno portal com três páginas conectadas:

1. **Programação** — publicações sobre as disciplinas do semestre;
2. **Hobbies** — registros pessoais em formato de fotolog;
3. **Sobre mim** — página de perfil desenvolvida na primeira aula.

## Objetivos da aula

Ao desenvolver este projeto, o estudante deverá compreender:

- A estrutura básica de um documento HTML;
- A importância das tags semânticas;
- A diferença entre cabeçalho, conteúdo principal e rodapé;
- A criação de links entre páginas do mesmo site;
- A organização de uma publicação com título, imagem, texto e data;
- A ligação entre arquivos HTML e CSS;
- A diferença entre estilos globais e estilos específicos de cada página.

## Tags semânticas utilizadas

O projeto utiliza as seguintes tags:

| Tag | Finalidade |
| --- | --- |
| `header` | Representa o cabeçalho da página ou de uma publicação. |
| `nav` | Reúne os links do menu de navegação. |
| `main` | Identifica o conteúdo principal da página. |
| `section` | Agrupa conteúdos relacionados. |
| `article` | Representa uma publicação independente. |
| `figure` | Agrupa uma imagem e sua legenda. |
| `figcaption` | Adiciona uma legenda à imagem. |
| `time` | Representa uma data ou um horário. |
| `footer` | Representa o rodapé da página ou de uma publicação. |

## Organização dos arquivos

```text
meu-portal/
├── index.html
├── hobbies.html
├── perfil.html
├── README.md
├── css/
│   ├── reset.css
│   ├── global.css
│   ├── perfil.css
│   ├── programacao.css
│   └── hobbies.css
└── img/
    ├── hobbies/
    │   ├── musica.jpg
    │   ├── cinema.jpg
    │   └── hockey.jpg
    ├── dev/
    │   ├── vue.jpg
    │   └── frameworks.jpg
    └── profile/
        └── about-profile.jpg
```

## Páginas do portal

### Programação

A página `programacao.html` funciona como um pequeno blog acadêmico. Nela, o
estudante poderá publicar conteúdos sobre as disciplinas que está cursando.

Cada publicação pode apresentar:

- Nome da disciplina;
- Título;
- Subtítulo;
- Imagem;
- Texto descritivo;
- Data e horário.

### Hobbies

A página `hobbies.html` é inspirada nos antigos fotologs e nos feeds das redes
sociais. Nesta primeira versão, as publicações aparecem uma abaixo da outra.

Cada registro possui:

- Nome do usuário;
- Categoria;
- Fotografia;
- Legenda;
- Título;
- Texto descritivo;
- Data e horário.

### Sobre mim

O arquivo `index.html` apresenta o perfil criado na primeira aula. Ele pode
conter fotografia, apresentação pessoal, informações acadêmicas, hobbies,
tecnologias e links para redes sociais.

## Organização dos estilos

O projeto utiliza um arquivo global e um arquivo específico para cada página.

### `global.css`

Contém os estilos compartilhados por todo o portal:

- Cabeçalho;
- Menu de navegação;
- Espaçamento do conteúdo;
- Rodapé.

### `perfil.css`

Contém apenas os estilos da página Sobre mim.

### `programacao.css`

Contém apenas os estilos das publicações acadêmicas.

### `hobbies.css`

Contém apenas os estilos do fotolog.

Os arquivos CSS devem ser importados nesta ordem:

```html
<link rel="stylesheet" href="global.css">
<link rel="stylesheet" href="hobbies.css">
```

Primeiro carregamos as regras compartilhadas. Depois carregamos as regras
específicas da página.

## Menu de navegação

O mesmo menu deve aparecer nas três páginas:

```html
<nav class="menu-site">
    <ul>
        <li><a href="programacao.html">Programação</a></li>
        <li><a href="hobbies.html">Hobbies</a></li>
        <li><a href="index.html">Sobre mim</a></li>
    </ul>
</nav>
```

Esses são links internos porque conectam documentos do mesmo projeto.

## Como executar o projeto

1. Faça o download ou copie a pasta do projeto;
2. Confirme se os arquivos estão organizados conforme a estrutura apresentada;
3. Adicione as fotografias dentro da pasta `imagens`;
4. Abra o arquivo `index.html` no navegador;
5. Utilize o menu para navegar entre as páginas.

Não é necessário instalar programas adicionais ou iniciar um servidor nesta
etapa. Os arquivos podem ser abertos diretamente no navegador.

## Atividade proposta

Cada estudante deverá personalizar o portal com conteúdos próprios.

### Página Programação

- Criar pelo menos duas publicações;
- Utilizar disciplinas diferentes;
- Informar título, descrição e data;
- Adicionar pelo menos uma imagem.

### Página Hobbies

- Criar três registros;
- Escolher fotografias relacionadas aos seus hobbies;
- Escrever uma legenda para cada imagem;
- Informar categoria, título, descrição e data.

### Página Sobre mim

- Manter o conteúdo criado na primeira aula;
- Adicionar o menu compartilhado;
- Adicionar o rodapé compartilhado;
- Verificar se os links entre as páginas funcionam.

## Evolução na próxima aula

Nesta versão, o foco está na semântica, nas páginas e nos links internos. Por
isso, o CSS utiliza principalmente cores, margens, espaçamentos, bordas e
seletores básicos.

Na próxima etapa, a página de Hobbies poderá ser transformada em:

- Um feed semelhante ao Instagram utilizando Flexbox;
- Uma galeria de fotografias utilizando CSS Grid;
- Um mural de cartões inspirado no Pinterest;
- Um layout adaptado para diferentes tamanhos de tela.

## Checklist de entrega

- [ ] As três páginas foram criadas;
- [ ] O menu aparece nas três páginas;
- [ ] Todos os links funcionam;
- [ ] O `global.css` foi importado;
- [ ] Cada página possui seu próprio arquivo CSS;
- [ ] As imagens possuem o atributo `alt`;
- [ ] As publicações utilizam tags semânticas;
- [ ] As datas utilizam a tag `time`;
- [ ] Os arquivos estão organizados em pastas;
- [ ] O portal abre corretamente no navegador.

---

**Disciplina:** Desenvolvimento Web I  
**Instituição:** IFC — Campus Araquari  
**Projeto:** Portal Pessoal
