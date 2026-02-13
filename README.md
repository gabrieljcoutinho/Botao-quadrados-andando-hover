# Neon Glitch Button — Cyberpunk UI

Este projeto apresenta um botão com estética **Cyberpunk**, focado em efeitos de iluminação neon e detalhes geométricos que se movem dinamicamente durante a interação do usuário. O componente utiliza CSS puro para criar uma experiência visual de alta fidelidade sem a necessidade de imagens ou JavaScript.

---

## 🚀 Destaques Técnicos

### 1. Efeito de Brilho Neon (Glow)
O botão utiliza a propriedade `box-shadow` combinada com transições de cor de fundo para criar um efeito de iluminação intensa ao passar o mouse. A cor `#ff1867` (magenta neon) é aplicada tanto ao texto quanto à sombra externa, simulando uma lâmpada neon acesa.

### 2. Detalhes Geométricos Móveis
Utilizando os elementos internos `<i>` e pseudo-elementos `::before` e `::after`, o botão possui pequenos "detalhes" que deslizam pelas bordas:
* **Topo:** Um pequeno retângulo que se move da direita para a esquerda e se expande no hover.
* **Base:** Um detalhe simétrico que se move da esquerda para a direita.
* Esse movimento coordenado cria uma sensação de "scanner" ou tecnologia ativa.

### 3. Camadas de Profundidade
O botão utiliza o truque de `inset: 2px` no pseudo-elemento `::before` para criar uma moldura interna escura (`#222`), permitindo que a borda neon externa brilhe com mais contraste enquanto o centro permanece legível.

### 4. Tipografia Dinâmica
A propriedade `letter-spacing` é animada de `0.1em` para `0.25em` no hover, dando um efeito de expansão elegante que complementa o aumento do brilho.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5**: Estrutura minimalista utilizando apenas `button`, `span` e `i`.
* **CSS3**: 
    - Posicionamento absoluto e relativo.
    - Pseudo-elementos (`::before` / `::after`) para decoração complexa.
    - Transições suaves (`transition: 0.5s`).
    - Propriedade `inset` para controle de bordas internas.

---

## 📂 Estrutura do Código

A estrutura necessária para o funcionamento dos detalhes animados é:

```html`
<button>
    <span>Texto</span>
    <i></i> </button>

<img width="235" height="71" alt="Image" src="https://github.com/user-attachments/assets/ba53b355-a04b-468e-b9a1-9b64c580a40a" />
