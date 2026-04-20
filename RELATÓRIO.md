
## Visão Geral
Este relatório documenta todas as correções realizadas no ficheiro HTML original, com base nos comentários inseridos no código corrigido.

> ***Obs:*** Este relatório foi gerado com auxílio de IA

> **Nota:** Não encontrei erros no ficheiro de CSS

---

## 1. Correções Sintáticas

### 1.1 Fechamento de tags
Foram identificados e corrigidos erros de sintaxe que poderiam comprometer a renderização correta do HTML:

- Tag `<link>` não estava corretamente fechada:
```html
<link rel="stylesheet" href="style_erros.css" />
```

- Tag `<p>` não estava fechada na secção "Sobre":
```html
<p>...</p>
```

- Tag `<a>` não estava corretamente fechada no footer:
```html
<li><a href="#sobre">Sobre a F1</a></li>
```

## 2. Melhorias Semânticas

### 2.1 Estrutura da Navbar

- Substituição de `<div>` por `<header>` para representar corretamente o cabeçalho da página
  
- Uso adequado de `<nav>` para agrupar links de navegação.
```html
<header class="navbar">
```
  
### 2.2 Estrutura do logotipo

Substituição de `<span>` por `<h1>` para representar o título principal da página:
```html
<h1 class="logo-text">Fórmula 1</h1>
```

### 2.3 Hierarquia de headings

Correção de `<h4>` para `<h3>` para manter consistência estrutural

### 2.4 Uso de elementos semânticos

Substituição de `<div>` por `<article>` em conteúdos independentes:

- Secção "Sobre"
- Equipas
- Circuitos
- Pilotos
- Newsletter

```html
 <article class="sobre__card">
```

### 2.5 Uso de <figure> e <figcaption>

Estrutura melhorada para imagens com descrição:
```html
<figure>
  <img src="..." alt="..." />
  <figcaption>Descrição da imagem</figcaption>
</figure>
```

### 2.6 Navegação no Hero

Substituição de `<div>` por `<nav>` para botões de navegação:
```html
<nav class="hero__buttons">
```

## 3. Acessibilidade

### 3.1 Associação entre label e input

Adicionado atributo for na label:
```html
<label for="email-input">Endereço de email</label>
```

### 3.2 Tipo correto de input

Alteração de:
```html
<input type="text">
```
para:
```html
<input type="email">
```

### 3.3 Uso de atributo alt

Adicionadas descrições em imagens relevantes:
```html
<img src="..." alt="Descrição da imagem" />
```

## 4. Melhorias de Estrutura e Conteúdo

### 4.1 Elementos inline vs block

Substituição de `<span>` por `<p>` nas estatísticas:
```html
<p class="stat__number">24</p>
```

### 4.2 Organização com <article>

Uso consistente de `<article>` para conteúdos independentes

### 4.3 Atualização de imagens

Substituição de URLs por imagens mais adequadas

---

## 5. Correções Específicas

### 5.1 Correção de atributo href

Foi corrigido o uso incorreto de href em um elemento <div>.
Antes:
```html
<div href="/index_erros.html" class="navbar__logo">
```

Depois:
```html
<a href="/index_erros.html" class="navbar__logo">
```

## 6. Outras Melhorias

- Adição do atributo `lang="pt"` na tag `<html>`
- Melhor organização estrutural do documento
- Padronização de elementos HTML
- Uso consistente de boas práticas modernas















