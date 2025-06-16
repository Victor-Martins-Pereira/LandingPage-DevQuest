# 🚀 **Landing Page Huddle - DevQuest**

Desenvolvida como desafio do curso DevQuest. A página apresenta um design moderno e responsivo, utilizando técnicas avançadas de CSS Grid e Flexbox.

## 🌟 **Destaques do Projeto**

- **Design totalmente responsivo** (mobile, tablet e desktop)
- **Efeitos de hover interativos** em botões e ícones sociais
- **Otimização de performance** com lazy loading de imagens
- **Arquitetura CSS modular** com variáveis e media queries

## 🛠 **Tecnologias Utilizadas**

### **Front-End**
| Tecnologia | Uso no Projeto |
|------------|----------------|
| HTML5 | Estrutura semântica com tags modernas |
| CSS3 | Grid, Flexbox, Variáveis CSS, Media Queries |
| Font Awesome | Ícones sociais |
| Google Fonts | Família Poppins |

### **Principais Técnicas CSS**
```css
/* Layout principal com CSS Grid */
.container {
  min-height: 100dvh;
  display: grid;
  grid-template-areas:
    "cabecalho"
    "principal"
    "footer";
}

/* Design responsivo avançado */
@media (max-width: 1024px) {
  body {
    background-image: url(../../images/bg-mobile.svg);
  }
  
  .container-principal {
    grid-template-columns: 1fr;
    text-align: center;
  }
}
```

## 🎨 **Estrutura do Layout**

1. **Cabeçalho**
   - Logo responsivo com tamanho adaptável
   - Posicionamento flexível

2. **Conteúdo Principal**
   - Grid de duas colunas (desktop) → uma coluna (mobile)
   - Ilustração vetorial otimizada
   - Textos com hierarquia visual clara
   - Botão CTA com efeitos hover

3. **Rodapé**
   - Ícones sociais com interações
   - Posicionamento responsivo (direita/centro)

## 📱 **Responsividade**

| Breakpoint | Adaptações |
|------------|------------|
| Desktop (>1024px) | Layout em duas colunas, menu alinhado à esquerda |
| Tablet/Mobile (≤1024px) | Single column, centralização de elementos |
| Mobile | Background alternativo, font-size ajustado |

**Exemplo de código responsivo:**
```css
@media (max-width: 1024px) {
  .container-principal {
    grid-template-columns: 1fr;
    text-align: center;
  }
  
  .container-principal .texto {
    align-items: center;
  }
}
```

## 🎯 **O Que Aprendi**

### **Desafios Superados**
1. **CSS Grid vs Flexbox**
   - Domínio da combinação entre Grid (layout geral) e Flexbox (alinhamentos internos)
   ```css
   /* Grid para layout geral */
   .container {
     display: grid;
     grid-template-areas: "cabecalho" "principal" "footer";
   }
   
   /* Flexbox para alinhamentos internos */
   .footer .social {
     display: flex;
     gap: 15px;
   }
   ```

2. **Transições e Interações**
   - Criação de microinterações suaves:
   ```css
   .register:hover {
     transform: translateY(-2px);
     box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
     transition: 0.3s ease-in-out;
   }
   ```

3. **Mobile-First vs Desktop-First**
   - Entendimento prático das diferenças na abordagem:
   ```css
   /* Desktop-first com override mobile */
   body {
     background: var(--cor-primaria) url(../../images/bg-desktop.svg);
     
     @media (max-width: 1024px) {
       background-image: url(../../images/bg-mobile.svg);
     }
   }
   ```

## 📂 **Estrutura de Arquivos**

```
LandingPage-DevQuest/
├── images/
│   ├── bg-desktop.svg
│   ├── bg-mobile.svg
│   ├── illustration-mockups.svg
│   └── logo.svg
├── src/
│   ├── Css/
│   │   ├── reset.css
│   │   ├── variables.css
│   │   ├── styles.css
│   │   └── responsivo.css
└── index.html
```

## Demonstração 🚀

Você pode ver uma versão online e interativa do projeto aqui: [Projeto Landing Page - DevQuest](https://victor-martins-pereira.github.io/LandingPage-DevQuest/)

## Conecte-se Comigo

**Desenvolvido com ❤️ por [Victor Martins Pereira](https://www.instagram.com/victor_martins.p/)**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](www.linkedin.com/in/victor-martins-pereira-dev) [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Victor-Martins-Pereira)
