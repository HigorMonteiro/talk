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
        --color-red-500: oklch(63.7% .237 25.331);
        --color-red-600: oklch(57.7% .245 27.325);
        --color-red-700: oklch(50.5% .213 27.518);
        --color-amber-200: oklch(92.4% .12 95.746);
        --color-amber-400: oklch(82.8% .189 84.429);
        --color-cyan-50: oklch(98.4% .019 200.873);
        --color-cyan-100: oklch(95.6% .045 203.388);
        --color-cyan-200: oklch(91.7% .08 205.041);
        --color-cyan-400: oklch(78.9% .154 211.53);
        --color-cyan-600: oklch(60.9% .126 221.723);
        --color-cyan-700: oklch(52% .105 223.128);
        --color-cyan-800: oklch(45% .085 224.283);
        --color-cyan-900: oklch(39.8% .07 227.392);
        --color-cyan-950: oklch(30.2% .056 229.695);
        --color-sky-500: oklch(68.5% .169 237.323);
        --color-sky-700: oklch(50% .134 242.749);
        --color-blue-100: oklch(93.2% .032 255.585);
        --color-blue-500: oklch(62.3% .214 259.815);
        --color-blue-900: oklch(37.9% .146 265.522);
        --color-indigo-500: oklch(58.5% .233 277.117);
        --color-indigo-600: oklch(51.1% .262 276.966);
        --color-indigo-700: oklch(45.7% .24 277.023);
        --color-purple-400: oklch(71.4% .203 305.504);
        --color-pink-50: oklch(97.1% .014 343.198);
        --color-pink-500: oklch(65.6% .241 354.308);
        --color-pink-950: oklch(28.4% .109 3.907);
        --color-gray-300: oklch(87.2% .01 258.338);
        --color-gray-500: oklch(55.1% .027 264.364);
        --color-gray-600: oklch(44.6% .03 256.802);
        --color-gray-700: oklch(37.3% .034 259.733);
        --color-zinc-100: oklch(96.7% .001 286.375);
        --color-zinc-200: oklch(92% .004 286.32);
        --color-zinc-300: oklch(87.1% .006 286.286);
        --color-zinc-400: oklch(70.5% .015 286.067);
        --color-zinc-500: oklch(55.2% .016 285.938);
        --color-zinc-600: oklch(44.2% .017 285.786);
        --color-zinc-700: oklch(37% .013 285.805);
        --color-zinc-800: oklch(27.4% .006 286.033);
        --color-zinc-900: oklch(21% .006 285.885);
        --color-black: #000;
        --color-white: #fff;
        --spacing: .25rem;
        --container-3xl: 48rem;
        --text-xs: .75rem;
        --text-xs--line-height: calc(1/.75);
        --text-sm: .875rem;
        --text-sm--line-height: calc(1.25/.875);
        --text-base: 1rem;
        --text-base--line-height: 1.5;
        --text-lg: 1.125rem;
        --text-lg--line-height: calc(1.75/1.125);
        --text-xl: 1.25rem;
        --text-xl--line-height: calc(1.75/1.25);
        --text-2xl: 1.5rem;
        --text-2xl--line-height: calc(2/1.5);
        --text-3xl: 1.875rem;
        --text-3xl--line-height: 1.2;
        --text-4xl: 2.25rem;
        --text-4xl--line-height: calc(2.5/2.25);
        --text-5xl: 3rem;
        --text-5xl--line-height: 1;
        --text-6xl: 3.75rem;
        --text-6xl--line-height: 1;
        --font-weight-medium: 500;
        --font-weight-semibold: 600;
        --font-weight-bold: 700;
        --tracking-tight: -.025em;
        --radius-md: .375rem;
        --radius-lg: .5rem;
        --radius-xl: .75rem;
        --default-transition-duration: .15s;
        --default-transition-timing-function: cubic-bezier(.4,0,.2,1);
        --default-font-family: var(--font-sans);
        --default-mono-font-family: var(--font-mono);
        --animate-slide-up: slideUp .5s ease-in forwards;
        --color-accent: var(--color-cyan-600);
        --color-text: var(--color-zinc-900);
        --color-muted: var(--color-zinc-600);
        --color-bg-code: var(--color-zinc-100);
    }
}

.slidev-page {
    background: var(--color-white);
    color: var(--color-text);
    font-family: var(--font-sans);
    overflow: visible !important;
}

.slidev-layout {
    font-family: var(--font-sans);
    color: var(--color-text);
    overflow: visible !important;
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
    background: var(--color-bg-code);
    color: var(--color-indigo-700);
    padding: 0.25rem 0.5rem;
    border-radius: var(--radius-md);
}

pre {
    background: var(--color-bg-code);
    border-left: 3px solid var(--color-accent);
    padding: 1.125rem;
    border-radius: var(--radius-lg);
    font-family: var(--font-mono);
}

pre code {
    background: transparent;
    color: var(--color-zinc-900);
    padding: 0;
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

a {
    color: var(--color-blue-500);
    text-decoration: none;
    transition: color var(--default-transition-duration) var(--default-transition-timing-function);
}

a:hover {
    color: var(--color-blue-900);
}

strong {
    color: var(--color-zinc-900);
    font-weight: var(--font-weight-bold);
}

.slidev-layout h2 strong {
    color: var(--color-indigo-700);
}

.slidev-layout h3 strong {
    color: var(--color-purple-400);
}

blockquote {
    border-left: 4px solid var(--color-amber-400);
    padding-left: 1rem;
    color: var(--color-zinc-700);
    font-style: italic;
}

.slidev-layout.cover h1 {
    color: var(--color-black);
    text-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
}

.slidev-layout.cover h3 {
    color: var(--color-zinc-600);
}

.slidev-layout:not(.cover) h2 {
    border-bottom: 2px solid var(--color-cyan-200);
    padding-bottom: 0.5rem;
    margin-bottom: 1.5rem;
}

.slidev-layout:not(.cover) h3 {
    color: var(--color-indigo-600);
}

.examples-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1.5rem;
    margin: 2rem auto 0;
    max-width: 900px;
    width: 100%;
}

.example-card {
    background: var(--color-white);
    border: 2px solid var(--color-zinc-200);
    border-top-width: 4px;
    border-radius: var(--radius-lg);
    padding: 2rem;
    transition: all var(--default-transition-duration) var(--default-transition-timing-function);
    cursor: pointer;
    position: relative;
    overflow: hidden;
}

.example-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 4px;
    height: 100%;
    background: var(--color-accent);
    transform: scaleY(0);
    transition: transform var(--default-transition-duration) var(--default-transition-timing-function);
}

.example-card:hover {
    border-color: var(--color-accent);
    transform: translateY(-4px);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
}

.example-card:hover::before {
    transform: scaleY(1);
}

.example-card:nth-child(1) {
    border-top-color: var(--color-pink-500);
}

.example-card:nth-child(2) {
    border-top-color: var(--color-sky-500);
}

.example-card:nth-child(3) {
    border-top-color: var(--color-blue-500);
}

.example-card:nth-child(4) {
    border-top-color: var(--color-purple-400);
}

.example-card-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 40px;
    height: 40px;
}

.example-card-icon svg {
    width: 100%;
    height: 100%;
    display: block;
}

.example-card-title {
    font-size: var(--text-xl);
    font-weight: var(--font-weight-semibold);
    color: var(--color-zinc-900);
    margin: 0;
}

.example-card:nth-child(1) .example-card-icon {
    color: var(--color-pink-500);
}

.example-card:nth-child(2) .example-card-icon {
    color: var(--color-sky-500);
}

.example-card:nth-child(3) .example-card-icon {
    color: var(--color-blue-500);
}

.example-card:nth-child(4) .example-card-icon {
    color: var(--color-purple-400);
}

@media (max-width: 768px) {
    .examples-grid {
        grid-template-columns: 1fr;
        gap: 1rem;
    }
}

.funny-quote {
    background: linear-gradient(135deg, var(--color-amber-200) 0%, var(--color-pink-50) 100%);
    border-left: 4px solid var(--color-amber-400);
    border-radius: var(--radius-lg);
    padding: 1.25rem 1.5rem;
    margin: 1.5rem 0;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
    position: relative;
}

.funny-quote::before {
    content: '😅';
    position: absolute;
    top: -10px;
    right: 15px;
    font-size: 1.5rem;
    background: var(--color-white);
    padding: 0.25rem;
    border-radius: 50%;
}

.funny-quote p {
    margin: 0;
    font-style: italic;
    color: var(--color-zinc-800);
    font-size: var(--text-lg);
    font-weight: var(--font-weight-medium);
    line-height: 1.6;
}

.funny-quote-center {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 60vh;
    padding: 2rem;
    gap: 2rem;
    overflow: visible;
}

.funny-quote-center p {
    background: linear-gradient(135deg, var(--color-amber-200) 0%, var(--color-pink-50) 100%);
    border-left: 6px solid var(--color-amber-400);
    border-radius: var(--radius-xl);
    padding: 2rem 3rem;
    margin: 0;
    font-style: italic;
    color: var(--color-zinc-800);
    font-size: clamp(var(--text-xl), 3vw, var(--text-3xl));
    font-weight: var(--font-weight-semibold);
    line-height: 1.5;
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.1);
    position: relative;
    max-width: 800px;
    text-align: center;
}

.funny-quote-center p::before {
    content: '😅';
    position: absolute;
    top: -20px;
    right: 30px;
    font-size: 3rem;
    background: var(--color-white);
    padding: 0.5rem;
    border-radius: 50%;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    z-index: 1;
}

.css-animation-demo {
    margin-top: 3rem;
    display: flex;
    flex-direction: column;
    gap: 2rem;
    align-items: center;
    width: 100%;
    max-width: 900px;
    overflow: visible;
}

.code-editor {
    background: var(--color-zinc-900);
    border-radius: var(--radius-lg);
    padding: 1.5rem;
    font-family: var(--font-mono);
    font-size: var(--text-base);
    width: 100%;
    max-width: 400px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
}

.code-line {
    margin: 0.5rem 0;
    opacity: 0;
    animation: typeIn 0.8s ease-in forwards;
}

.code-line:nth-child(1) {
    animation-delay: 0.5s;
}

.code-line:nth-child(2) {
    animation-delay: 1.3s;
}

.code-line:nth-child(3) {
    animation-delay: 2.1s;
}

.code-selector {
    color: var(--color-pink-500);
}

.code-property {
    color: var(--color-cyan-400);
}

.code-value {
    color: var(--color-amber-400);
}

.code-bracket {
    color: var(--color-white);
}

.html-elements {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    min-height: 180px;
    padding: 2rem;
    overflow: visible;
    width: 100%;
    position: relative;
}

.box-element {
    background: var(--color-blue-500);
    color: var(--color-white);
    padding: 1rem 1.5rem;
    border-radius: var(--radius-md);
    font-weight: var(--font-weight-semibold);
    opacity: 0;
    position: relative;
    overflow: visible;
    animation: appear 0.5s ease-out forwards, disobey 2s ease-in-out infinite;
}

.box-1 {
    animation-delay: 2.5s, 4s;
}

.box-2 {
    animation-delay: 2.7s, 4.2s;
    background: var(--color-purple-400);
}

.box-3 {
    animation-delay: 2.9s, 4.4s;
    background: var(--color-indigo-500);
}

.box-element::after {
    content: '❌';
    position: absolute;
    top: -12px;
    right: -12px;
    font-size: 1.2rem;
    opacity: 0;
    animation: shake 0.5s ease-in-out infinite, fadeIn 0.3s ease-out forwards;
    animation-delay: 3.5s, 3.5s;
    z-index: 10;
    background: var(--color-white);
    border-radius: 50%;
    width: 24px;
    height: 24px;
    display: flex;
    align-items: center;
    justify-content: center;
}

@keyframes typeIn {
    from {
        opacity: 0;
        transform: translateX(-10px);
    }
    to {
        opacity: 1;
        transform: translateX(0);
    }
}

@keyframes appear {
    from {
        opacity: 0;
        transform: scale(0.8);
    }
    to {
        opacity: 1;
        transform: scale(1);
    }
}

@keyframes shake {
    0%, 100% {
        transform: translateX(0) rotate(0deg);
        opacity: 1;
    }
    25% {
        transform: translateX(-5px) rotate(-5deg);
    }
    75% {
        transform: translateX(5px) rotate(5deg);
    }
}

@keyframes disobey {
    0%, 100% {
        transform: translateX(0) translateY(0);
    }
    25% {
        transform: translateX(15px) translateY(-10px);
    }
    50% {
        transform: translateX(-15px) translateY(10px);
    }
    75% {
        transform: translateX(10px) translateY(-5px);
    }
}

.box-element::after {
    animation: shake 0.5s ease-in-out infinite, fadeIn 0.3s ease-out forwards;
    animation-delay: 3.5s, 3.5s;
}

@keyframes fadeIn {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}

.demo-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    margin-top: 2rem;
    align-items: center;
    max-width: 1000px;
    margin-left: auto;
    margin-right: auto;
}

.demo-code {
    background: var(--color-zinc-900);
    border-radius: var(--radius-lg);
    padding: 2rem;
    font-family: var(--font-mono);
    font-size: var(--text-sm);
    line-height: 1.8;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
}

.code-line-demo {
    opacity: 0;
    animation: codeTypeIn 1s ease-out forwards;
    margin: 0.75rem 0;
}

.code-line-demo:nth-child(1) {
    animation-delay: 0.5s;
}

.code-line-demo:nth-child(2) {
    animation-delay: 1.5s;
}

.code-keyword {
    color: var(--color-purple-400);
}

.code-variable {
    color: var(--color-cyan-400);
}

.code-function {
    color: var(--color-pink-500);
}

.code-string {
    color: var(--color-amber-400);
}

.demo-preview {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 2rem;
    padding: 2rem;
    background: var(--color-zinc-100);
    border-radius: var(--radius-lg);
    min-height: 200px;
    justify-content: center;
}

.demo-toggle {
    display: none;
}

.demo-controls {
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 2.5s;
}

.demo-button-label {
    display: inline-block;
    cursor: pointer;
}

.demo-button {
    display: inline-block;
    background: var(--color-blue-500);
    color: var(--color-white);
    border: none;
    padding: 1rem 2rem;
    border-radius: var(--radius-md);
    font-size: var(--text-lg);
    font-weight: var(--font-weight-semibold);
    cursor: pointer;
    transition: all 0.3s ease;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
    font-family: var(--font-sans);
    user-select: none;
}

.demo-button-label:hover .demo-button {
    transform: translateY(-2px);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
}

.demo-toggle:checked + .demo-button {
    background: var(--color-cyan-600);
    animation: buttonPulse 0.3s ease-out;
}

.demo-button-label:active .demo-button {
    transform: translateY(0);
}

.demo-status {
    margin-top: 0;
}

.status-text {
    font-size: var(--text-base);
    color: var(--color-zinc-700);
    font-weight: var(--font-weight-medium);
}

.status-value {
    color: var(--color-blue-500);
    font-weight: var(--font-weight-semibold);
    transition: color 0.3s ease;
}

.demo-controls {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 2rem;
}

.demo-toggle:checked ~ .demo-button-label .demo-button {
    background: var(--color-cyan-600);
    animation: buttonPulse 0.3s ease-out;
}

.demo-toggle:checked ~ .demo-status .status-value {
    color: var(--color-cyan-600);
}

.demo-toggle:checked ~ .demo-status .status-value::after {
    content: 'Ativo';
}

.demo-toggle:not(:checked) ~ .demo-status .status-value::after {
    content: 'Inativo';
}

.status-value::before {
    content: '';
}

.status-value::after {
    content: 'Inativo';
}

@keyframes codeTypeIn {
    from {
        opacity: 0;
        transform: translateX(-20px);
    }
    to {
        opacity: 1;
        transform: translateX(0);
    }
}

@keyframes buttonAppear {
    from {
        opacity: 0;
        transform: scale(0.8);
    }
    to {
        opacity: 1;
        transform: scale(1);
    }
}

@keyframes buttonPulse {
    0% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.05);
    }
    100% {
        transform: scale(1);
    }
}

@media (max-width: 768px) {
    .demo-container {
        grid-template-columns: 1fr;
        gap: 2rem;
    }
}

.slidev-layout:has(.frontend-tasks) {
    padding: 2rem 3rem !important;
    overflow: visible !important;
}

.slidev-layout:has(.frontend-tasks) h1 {
    margin-bottom: 1rem;
    font-size: clamp(var(--text-2xl), 3vw, var(--text-3xl));
}

.frontend-tasks {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1.5rem;
    margin-top: 1rem;
    max-width: 900px;
    margin-left: auto;
    margin-right: auto;
    padding: 0 1rem;
    overflow: visible;
}

.task-card {
    background: var(--color-white);
    border-radius: var(--radius-lg);
    overflow: hidden;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    transition: all 0.3s ease;
    border: 2px solid var(--color-zinc-200);
    max-width: 100%;
}

.task-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 16px rgba(0, 0, 0, 0.15);
    border-color: var(--color-accent);
}

.task-image {
    width: 100%;
    height: 160px;
    overflow: hidden;
    background: var(--color-zinc-100);
    position: relative;
}

.task-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.3s ease;
}

.task-card:hover .task-image img {
    transform: scale(1.03);
}

.task-card h3 {
    padding: 1rem 1.5rem;
    margin: 0;
    font-size: var(--text-base);
    font-weight: var(--font-weight-semibold);
    color: var(--color-zinc-900);
    text-align: center;
    border-top: 2px solid var(--color-zinc-100);
    line-height: 1.4;
}

.task-card:nth-child(1) {
    border-top-color: var(--color-pink-500);
}

.task-card:nth-child(2) {
    border-top-color: var(--color-sky-500);
}

.task-card:nth-child(3) {
    border-top-color: var(--color-blue-500);
}

.task-card:nth-child(4) {
    border-top-color: var(--color-purple-400);
}

.task-card:nth-child(1) h3 {
    border-top-color: var(--color-pink-500);
}

.task-card:nth-child(2) h3 {
    border-top-color: var(--color-sky-500);
}

.task-card:nth-child(3) h3 {
    border-top-color: var(--color-blue-500);
}

.task-card:nth-child(4) h3 {
    border-top-color: var(--color-purple-400);
}

@media (max-width: 768px) {
    .frontend-tasks {
        grid-template-columns: 1fr;
        gap: 1rem;
        padding: 0;
    }
    
    .task-image {
        height: 150px;
    }
    
    .task-card h3 {
        padding: 0.875rem 1rem;
        font-size: var(--text-sm);
    }
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

<div class="examples-grid">

<div class="example-card">
  <span class="example-card-icon">
    <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round">
      <rect x="2" y="2" width="20" height="20" rx="5" ry="5"/>
      <path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/>
      <line x1="17.5" y1="6.5" x2="17.51" y2="6.5"/>
    </svg>
  </span>
  <h3 class="example-card-title">Instagram Web</h3>
</div>

<div class="example-card">
  <span class="example-card-icon">
    <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24" fill="currentColor">
      <path d="M12 0C5.4 0 0 5.4 0 12s5.4 12 12 12 12-5.4 12-12S18.66 0 12 0zm5.521 17.34c-.24.359-.66.48-1.021.24-2.82-1.74-6.36-2.101-10.561-1.141-.418.122-.779-.179-.899-.539-.12-.421.18-.78.54-.9 4.56-1.021 8.52-.6 11.64 1.32.42.18.479.659.301 1.02zm1.44-3.3c-.301.42-.841.6-1.262.3-3.239-1.98-8.159-2.58-11.939-1.38-.479.12-1.02-.12-1.14-.6-.12-.48.12-1.021.6-1.141C9.6 9.9 15 10.561 18.72 12.84c.361.181.54.78.241 1.2zm.12-3.36C15.24 8.4 8.82 8.16 5.16 9.281c-.6.179-1.2-.181-1.38-.721-.18-.601.18-1.2.72-1.381 4.26-1.26 11.28-1.02 15.721 1.621.539.3.719 1.02.42 1.56-.299.421-1.02.599-1.559.3z"/>
    </svg>
  </span>
  <h3 class="example-card-title">Spotify Web</h3>
</div>

<div class="example-card">
  <span class="example-card-icon">
    <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round">
      <circle cx="9" cy="21" r="1"/>
      <circle cx="20" cy="21" r="1"/>
      <path d="M1 1h4l2.68 13.39a2 2 0 0 0 2 1.61h9.72a2 2 0 0 0 2-1.61L23 6H6"/>
    </svg>
  </span>
  <h3 class="example-card-title">Sites de compras</h3>
</div>

<div class="example-card">
  <span class="example-card-icon">
    <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round">
      <path d="M22 10v6M2 10l10-5 10 5-10 5z"/>
      <path d="M6 12v5c0 1.1.9 2 2 2h8c1.1 0 2-.9 2-2v-5"/>
    </svg>
  </span>
  <h3 class="example-card-title">Portais escolares</h3>
</div>

</div>

---

# **O que um frontend faz**

<div class="frontend-tasks">
  <div class="task-card">
    <div class="task-image">
      <img src="https://images.unsplash.com/photo-1467232004584-a241de8bcf5d?w=400&h=300&fit=crop" alt="Constrói telas" />
    </div>
    <h3>Constrói telas</h3>
  </div>
  
  <div class="task-card">
    <div class="task-image">
      <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?w=400&h=300&fit=crop" alt="Implementa interações" />
    </div>
    <h3>Implementa interações</h3>
  </div>
  
  <div class="task-card">
    <div class="task-image">
      <img src="https://images.unsplash.com/photo-1558494949-ef010cbdcc31?w=400&h=300&fit=crop" alt="Consome APIs" />
    </div>
    <h3>Consome APIs</h3>
  </div>
  
  <div class="task-card">
    <div class="task-image">
      <img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?w=400&h=300&fit=crop" alt="Trabalha em equipe" />
    </div>
    <h3>Trabalha com designers e backend</h3>
  </div>
</div>

---

# **A base da Web**

### **HTML — estrutura**

### **CSS — estilo**

### **JavaScript — comportamento**

---

<div class="funny-quote-center">
  <p>"Escrever CSS é fácil. Difícil é o CSS obedecer."</p>
</div>
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

<div class="demo-container">
  <div class="demo-code">
    <div class="code-line-demo">
      <span class="code-keyword">const</span> <span class="code-variable">btn</span> = <span class="code-function">document</span>.<span class="code-function">getElementById</span>(<span class="code-string">'btn'</span>);
    </div>
    <div class="code-line-demo">
      <span class="code-variable">btn</span>.<span class="code-function">addEventListener</span>(<span class="code-string">'click'</span>, () => <span class="code-variable">btn</span>.<span class="code-function">classList</span>.<span class="code-function">toggle</span>(<span class="code-string">'active'</span>))
    </div>
  </div>
  
  <div class="demo-preview">
    <div class="demo-controls">
      <input type="checkbox" id="demo-toggle" class="demo-toggle" />
      <label for="demo-toggle" class="demo-button-label">
        <span class="demo-button">Clique em mim!</span>
      </label>
      <div class="demo-status">
        <span class="status-text">Status: <span class="status-value"></span></span>
      </div>
    </div>
  </div>
</div>

---
layout: cover
---

# **"Você pode criar coisas que o mundo inteiro usa."**
