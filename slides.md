---
# Configuração do Slidev
theme: default
title: Desenvolvimento Frontend
info: |
  ## Apresentação sobre Desenvolvimento Frontend
  
  Criando tudo o que o usuário vê e toca
drawings:
  persist: false
transition: slide-left
mdc: true
colorSchema: light
highlighter: shiki
lineNumbers: false
---

<style>
@layer theme {
    :root,:host {
        --font-sans: ui-sans-serif,system-ui,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";
        --font-mono: ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;
        --color-accent: #00B8A9;
        --color-black: #000;
        --color-white: #fff;
        --color-text: #0f172a;
        --color-muted: #334155;
    }
}

.slidev-page {
    background: var(--color-white);
    color: var(--color-text);
    font-family: var(--font-sans);
}

.slidev-layout {
    font-family: var(--font-sans);
    color: var(--color-text);
}

h1 {
    color: var(--color-black);
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: -0.02em;
    line-height: 0.95;
}

h2 {
    color: var(--color-black);
    font-weight: 600;
}

h3 {
    color: var(--color-muted);
    font-weight: 500;
    font-size: 1.25rem;
}

ul li {
    color: var(--color-text);
    margin: 0.875rem 0;
}

ul li::marker {
    color: var(--color-accent);
}

code {
    font-family: var(--font-mono);
    background: #f5f7fa;
    padding: 0.25rem 0.5rem;
    border-radius: 0.375rem;
}

pre {
    background: #f5f7fa;
    padding: 1.125rem;
    border-radius: 0.75rem;
    font-family: var(--font-mono);
}

.slidev-layout.cover {
    text-align: center;
}

.slidev-layout.cover h1 {
    font-size: clamp(3rem, 6vw, 5.25rem);
}

.slidev-layout.cover h3 {
    margin-top: 1.125rem;
    font-size: 1.25rem;
}

h3 {
    color: var(--color-muted);
    font-weight: 500;
    font-size: 1.5rem;
    margin: 1rem 0;
}

ol li {
    color: var(--color-text);
    margin: 0.875rem 0;
    font-size: 1.125rem;
}

ol li::marker {
    color: var(--color-accent);
    font-weight: 600;
}
</style>

---
layout: cover
---

# **Desenvolvimento Frontend**

### Criando tudo o que o usuário vê e toca

---

# **O que é Frontend?**

* Parte visual das aplicações
* Interface + interação
* Mistura de design e tecnologia

---

# **Exemplos do dia a dia**

* Instagram Web
* Spotify Web
* Sites de compras
* Portais escolares

---

# **O que um frontend faz**

* Constrói telas
* Implementa interações
* Consome APIs
* Trabalha com designers e backend

---

# **A base da Web**

### **HTML — estrutura**

### **CSS — estilo**

### **JavaScript — comportamento**

---

# **Ferramentas utilizadas**

* VS Code
* Git & GitHub
* Figma
* DevTools do navegador

---

# **UX no Frontend**

* Facilidade de uso
* Organização da informação
* Acessibilidade (A11y)

---

# **Mercado de trabalho**

* Alta demanda
* React domina o mercado
* Boas práticas contam mais que diplomas

---

# **Como começar**

1. Aprender bases (HTML, CSS, JS)
2. Criar pequenos projetos
3. Publicar no GitHub
4. Criar portfólio

---
layout: default
---

# **Demonstração simples**

Criar um botão que muda de cor ao clicar.

```javascript
const btn = document.getElementById('btn');
btn.addEventListener('click', () => btn.classList.toggle('active'))
```

---
layout: cover
---

# **"Você pode criar coisas que o mundo inteiro usa."**
