# 🥤 Página Animada de Refrigerantes 🍓🥑🍊

Um projeto visual e interativo que apresenta uma **animação moderna com transições suaves, efeitos neon e frutas flutuantes**.  
Cada sabor (Morango, Abacate e Laranja) tem seu próprio tema de cor, criando uma experiência envolvente e dinâmica.  

---

## 🎬 Demonstração

<img width="1905" height="913" alt="image" src="https://github.com/user-attachments/assets/60ccbd56-476f-41fa-9775-694740be0550" />


---

## 💡 Sobre o Projeto

Este projeto foi criado com o objetivo de **praticar animações CSS, manipulação de classes com JavaScript e design responsivo**, resultando em uma página interativa de apresentação de produtos.  

A ideia é simular uma **campanha de bebidas saborizadas**, destacando cada sabor com uma cor, transição e efeito únicos.

---

## ⚙️ Tecnologias Utilizadas

| Tecnologia | Função |
|-------------|--------|
| **HTML5** | Estrutura e semântica da página |
| **CSS3 (com animações e keyframes)** | Estilização e efeitos visuais |
| **JavaScript (Vanilla)** | Controle da navegação entre os slides |
| **Responsividade (Media Queries)** | Adaptação para diferentes tamanhos de tela |

---

## 🧩 Estrutura dos Arquivos

```bash
📂 Projeto
 ┣ 📜 index.html     # Estrutura principal da página
 ┣ 📜 styles.css     # Estilos e animações
 ┣ 📜 script.js      # Lógica de navegação (botões anterior/próximo)
 ┗ 📂 img/           # Imagens das frutas e refrigerantes

🕹️ Funcionalidades

Alternância entre sabores clicando nas setas laterais

Efeitos de entrada e saída personalizados para cada fruta

Títulos com efeito neon pulsante

Fundo animado com gradiente pulsante

Animações de flutuação suave (float) nos elementos

Totalmente responsivo (se adapta a telas pequenas)

Efeito visual de bolhas animadas no fundo

🧠 Lógica de Navegação (JavaScript)

O funcionamento das setas é feito trocando a classe .active entre os elementos .item.
Trecho simplificado:

let list = document.querySelectorAll('.item');
let next = document.getElementById('next');
let prev = document.getElementById('prev');
let active = 0;

next.onclick = () => {
  list[active].classList.remove('active');
  active = (active + 1) % list.length;
  list[active].classList.add('active');
};

prev.onclick = () => {
  list[active].classList.remove('active');
  active = (active - 1 + list.length) % list.length;
  list[active].classList.add('active');
};

🎨 Destaques do CSS

Efeito neon pulsante no título:

@keyframes neonPulse {
    0% { text-shadow: 0 0 20px #fff; }
    100% { text-shadow: 0 0 150px var(--background); }
}


Animações de entrada personalizadas:

Morango → entra pela esquerda

Abacate → entra pela direita

Laranja → sobe de baixo

Flutuação constante nas imagens:

@keyframes floatY {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-15px); }
}

📱 Responsividade

O layout foi ajustado para telas menores com @media queries:

Tamanho da tela	Ajuste
Até 900px	Fonte reduzida, garrafas menores
Até 600px	Botões e textos mais compactos
🧩 Possíveis Melhorias Futuras

 Adicionar transição automática (carrossel automático)

 Incluir efeito sonoro suave nas trocas

 Criar versão com mais sabores

 Adicionar descrição de cada sabor

 Inserir botão “pause/play” da animação

👨‍💻 Autor

Fábio Detofolli Silva
💻 Desenvolvedor Front-End
🔗 LinkedIn - https://www.linkedin.com/in/fabio-detofolli-silva-31b52716b/

📧 Email - fabim.cajobi@hotmail.com

📝 Licença

Este projeto está sob a licença MIT — você pode usá-lo, modificá-lo e compartilhá-lo livremente.

✨ “Criatividade é o combustível por trás de cada linha de código.”
— Projeto Página Animada
