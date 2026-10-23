<div align="center">

# 🐍 SNAKE NEON

### A Classic Reimagined.

**Uma releitura moderna do clássico jogo da cobrinha, desenvolvida com tecnologias web nativas.**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

![Status](https://img.shields.io/badge/STATUS-EM_DESENVOLVIMENTO-00C853?style=flat-square)
![License](https://img.shields.io/badge/LICENSE-NOT_SPECIFIED-555555?style=flat-square)

---

**[Sobre](#-sobre-o-projeto) • [Funcionalidades](#-funcionalidades) • [Tecnologias](#-tecnologias) • [Instalação](#-instalação) • [Arquitetura](#-arquitetura) • [Roadmap](#-roadmap)**

</div>

<br>

## 📖 Sobre o projeto

**Snake Neon** é uma implementação moderna do clássico *Snake Game*, desenvolvida inteiramente com **HTML5, CSS3 e JavaScript Vanilla**.

O projeto combina uma estética minimalista com elementos neon, animações suaves e uma experiência interativa responsiva.

Seu principal objetivo é explorar conceitos fundamentais de desenvolvimento Front-End, como manipulação de elementos gráficos, gerenciamento de estados, detecção de colisões e otimização de animações.

> [!NOTE]
> O projeto foi desenvolvido sem frameworks ou dependências externas. Toda a aplicação está contida em um único arquivo HTML.

---

## ✨ Funcionalidades

| Funcionalidade | Descrição |
|:---|:---|
| 🐍 Movimentação fluida | Animações suaves utilizando `requestAnimationFrame`. |
| 🎮 Controles intuitivos | Compatibilidade com setas direcionais e WASD. |
| 📱 Responsividade | Interface adaptável para desktop e dispositivos móveis. |
| 🍎 Sistema de alimentação | Geração aleatória de alimentos e crescimento progressivo. |
| 🏆 Sistema de pontuação | Contabilização dos pontos durante a partida. |
| 💾 Recorde persistente | Armazenamento local utilizando `localStorage`. |
| ⚡ Dificuldade dinâmica | Aumento gradual da velocidade conforme a pontuação. |
| ⏸️ Gerenciamento de estados | Sistemas de início, pausa, continuação e reinício. |
| 💀 Detecção de colisões | Identificação de colisões com paredes e com o próprio corpo. |
| 🌙 Interface Dark | Identidade visual moderna com cores neon. |

---

## 🛠 Tecnologias

O projeto utiliza exclusivamente tecnologias nativas da Web.

### HTML5
Responsável pela estrutura semântica e organização dos componentes da interface.

### CSS3
Utilizado para estilização, responsividade, transições e identidade visual.

### JavaScript
Responsável pela lógica do jogo, gerenciamento de estados, movimentação e interatividade.

### Canvas API
Utilizada para renderização gráfica da cobrinha, alimentos e tabuleiro.

### Web Storage API
Permite armazenar o recorde localmente, preservando-o entre sessões.

---

## 🚀 Instalação

### Pré-requisitos

Você precisará apenas de um navegador moderno, como Chrome, Firefox ou Edge.

### Clonando o repositório

```bash
git clone https://github.com/SEU-USUARIO/snake-neon.git
```

Acesse o diretório:

```bash
cd snake-neon
```

Abra o arquivo:

```text
snake.html
```

O jogo será executado diretamente no navegador.

**Não é necessário instalar dependências ou iniciar servidores.**

---

## 🎮 Como jogar

O objetivo é controlar a cobrinha, coletar alimentos e alcançar a maior pontuação possível sem colidir com as paredes ou com o próprio corpo.

### Controles

| Tecla | Ação |
|:---:|:---|
| `↑` ou `W` | Mover para cima |
| `↓` ou `S` | Mover para baixo |
| `←` ou `A` | Mover para esquerda |
| `→` ou `D` | Mover para direita |
| `Espaço` | Pausar / Continuar |
| `Enter` | Iniciar nova partida |

Em dispositivos móveis, utilize os controles direcionais disponíveis na interface.

---

## 🧠 Arquitetura

A lógica do Snake Neon foi estruturada para separar o processamento do jogo de sua renderização gráfica.

### Game Loop

O ciclo principal utiliza `requestAnimationFrame`, permitindo atualizar a interface de acordo com a frequência de atualização do navegador.

A lógica de movimentação é executada em intervalos controlados, enquanto a renderização utiliza interpolação para produzir transições visuais suaves.

```text
┌──────────────────────┐
│     GAME START       │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   INPUT HANDLING     │
│  Keyboard / Touch    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│    GAME UPDATE       │
│ Movement / Collision │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│      RENDERING       │
│      Canvas API      │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│    NEXT FRAME        │
└──────────────────────┘
```

### Gerenciamento de estados

O jogo possui diferentes estados de execução:

- **READY:** aguardando o início da partida.
- **RUNNING:** partida em andamento.
- **PAUSED:** execução temporariamente interrompida.
- **GAME OVER:** partida encerrada após uma colisão.

Essa abordagem permite controlar o comportamento do jogo e evitar múltiplos ciclos de execução simultâneos.

---

## 📂 Estrutura do projeto

```text
snake-neon/
│
├── snake.html       # Aplicação completa
│
└── README.md        # Documentação
```

Toda a lógica e estilização estão incorporadas ao arquivo `snake.html`.

---

## ⚡ Performance

O Snake Neon foi desenvolvido considerando boas práticas de desempenho em aplicações interativas.

Entre as principais estratégias utilizadas estão:

- Renderização com Canvas API.
- Atualização visual utilizando `requestAnimationFrame`.
- Separação entre lógica e renderização.
- Controle de velocidade independente da taxa de quadros.
- Prevenção de ciclos de animação duplicados.
- Interpolação para suavização dos movimentos.

---

## 🗺 Roadmap

Possíveis melhorias para versões futuras:

- [ ] Sistema de temas personalizáveis.
- [ ] Efeitos sonoros.
- [ ] Diferentes níveis de dificuldade.
- [ ] Obstáculos dinâmicos.
- [ ] Sistema de conquistas.
- [ ] Ranking de pontuações.
- [ ] Novos modos de jogo.
- [ ] Personalização da cobrinha.

---

## 🤝 Contribuições

Sugestões e contribuições são bem-vindas!

Para contribuir:

1. Faça um fork do repositório.
2. Crie uma branch para sua funcionalidade.
3. Implemente suas alterações.
4. Faça o commit.
5. Abra um Pull Request.

Exemplo:

```bash
git checkout -b feature/nova-funcionalidade

git add .

git commit -m "feat: adiciona nova funcionalidade"

git push origin feature/nova-funcionalidade
```

---

## 📄 Licença

Este projeto ainda não possui uma licença definida.

---

<div align="center">

### 🐍 SNAKE NEON

**Built with HTML, CSS & JavaScript.**

*Simple technologies. Modern experiences.*

⭐ Se você gostou do projeto, considere deixar uma estrela no repositório!

</div>
