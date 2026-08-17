# Aula 1 — Introdução ao Desenvolvimento Web

Este repositório reúne o projeto prático desenvolvido durante a primeira aula da disciplina de **Desenvolvimento Web**.

O objetivo foi compreender como uma página é estruturada com HTML, estilizada com CSS, armazenada em um repositório Git e publicada na internet por meio do GitHub Pages.

## Site publicado

- **Demonstração:** [cristofersousa.github.io/profile-ifc](https://cristofersousa.github.io/profile-ifc/)
- **Repositório:** [github.com/cristofersousa/profile-ifc](https://github.com/cristofersousa/profile-ifc)

## Conteúdos trabalhados

Durante a aula, foram abordados os seguintes conceitos:

- Funcionamento básico da Web;
- Comunicação entre cliente, servidor e navegador;
- Estrutura inicial de um documento HTML;
- Utilização de títulos, parágrafos, imagens, listas e links;
- Aplicação de estilos com CSS;
- Seletores por elemento e por classe;
- Cores, fontes, margens e espaçamentos;
- Bordas, sombras e arredondamento;
- Centralização e organização do conteúdo;
- Uso de `box-sizing: border-box`;
- Organização de arquivos e caminhos relativos;
- Criação de um repositório no GitHub;
- Publicação de uma página estática com GitHub Pages;
- Segurança na abertura de links externos.

## Tecnologias utilizadas

- HTML5;
- CSS3;
- Git;
- GitHub;
- GitHub Pages.

## Estrutura do projeto

```text
profile-ifc/
├── index.html
├── images/
│   └── profile.png
└── README.md
```

> Neste primeiro exemplo, parte do CSS foi mantida no próprio arquivo HTML para demonstrar como os estilos eram aplicados diretamente em uma página. Em projetos maiores, a recomendação é separar os estilos em um arquivo como `css/style.css`.

## Conceitos importantes

### HTML

O HTML é responsável pela estrutura e pelo conteúdo da página. Ele define elementos como títulos, textos, imagens, listas e links.

Exemplo:

```html
<h1>Meu perfil</h1>

<p>Esta é a minha primeira página publicada na internet.</p>

<img src="./images/profile.png" alt="Foto de perfil" />
```

### CSS

O CSS é responsável pela apresentação visual da página, permitindo configurar cores, fontes, tamanhos, espaçamentos e posicionamento.

Exemplo:

```css
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  background-color: #f5f5f5;
}

.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  background-color: #ffffff;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
```

### `box-sizing: border-box`

Por padrão, o navegador soma `padding` e `border` ao tamanho definido para um elemento. Com `border-box`, essas medidas passam a fazer parte da largura e da altura informadas.

```css
* {
  box-sizing: border-box;
}
```

Essa configuração facilita o controle do layout e evita que os elementos ocupem mais espaço do que o esperado.


### Segurança em links externos

Ao utilizar `target="_blank"`, o navegador abre o link em uma nova aba.

```html
<a href="https://github.com/" target="_blank" rel="noopener noreferrer">
  Acessar o GitHub
</a>
```
O atributo `rel="noopener noreferrer"` oferece proteção adicional:

- `noopener` impede que a nova página controle a aba de origem por meio de `window.opener`;
- `noreferrer` evita o envio do endereço da página de origem no cabeçalho de referência.

Essa proteção ajuda a evitar ataques conhecidos como **reverse tabnabbing**, nos quais uma página externa tenta alterar ou redirecionar a aba original.

## Como executar localmente

1. Clone o repositório:

```bash
git clone https://github.com/cristofersousa/profile-ifc.git
```

2. Acesse o diretório:

```bash
cd profile-ifc
```

3. Abra o arquivo `index.html` no navegador.

Também é possível executar o projeto com uma extensão de servidor local, como o **Live Server** do Visual Studio Code.

## Como publicar no GitHub Pages

1. Envie os arquivos para um repositório do GitHub;
2. Acesse a opção **Settings** do repositório;
3. No menu lateral, selecione **Pages**;
4. Em **Source**, escolha **Deploy from a branch**;
5. Selecione a branch `main`;
6. Selecione a pasta `/(root)`;
7. Clique em **Save**;
8. Aguarde a publicação e acesse o endereço informado pelo GitHub.

O endereço de um projeto publicado geralmente segue este formato:

```text
https://usuario.github.io/nome-do-repositorio/
```

## Aprendizados da aula

Ao finalizar a atividade, foi possível visualizar o ciclo inicial de desenvolvimento e publicação de uma página Web:

```text
Planejamento → HTML → CSS → Git → GitHub → GitHub Pages
```

Mais do que criar uma página visual, a atividade demonstrou como os arquivos produzidos localmente podem ser versionados e disponibilizados publicamente na internet.

## Próximos passos

- Separar o CSS em um arquivo externo;
- Melhorar a responsividade da página;
- Utilizar tags semânticas do HTML5;
- Adicionar novas seções ao perfil;
- Trabalhar com formulários;
- Introduzir comportamentos com JavaScript.

---

Material desenvolvido como apoio à **Aula 1 de Desenvolvimento Web**.

---

Atualizado em 16 de agosto de 2026.
