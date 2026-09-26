# Timer Ragnarök

Uma aplicação web de timer temática nórdica, inspirada no mundo de Ragnarök e no ambiente medieval de banquetes e festividades. O projeto foi criado para contar um tempo de 2 minutos e 30 segundos com visual imersivo, alerta sonoro e mensagem final.

## Visão geral

O projeto consiste em uma página única em HTML, CSS e JavaScript que exibe:

- Contador regressivo em formato MM:SS
- Botão para iniciar/reiniciar o tempo
- Avisos visuais à medida que o tempo se esgota
- Alerta sonoro ao fim do cronômetro
- Modal de encerramento com feedback visual
- Design responsivo com visual rústico vikingo

## Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript (vanilla)
- Áudio Web API para o alerta sonoro

## Estrutura do projeto

```text
timer-ragnarock/
├── index.html.html      # Página principal do projeto
├── img-fundo.png         # Imagem de fundo da interface
├── README.md            # Documentação do projeto
└── .git/                # Configuração do repositório Git
```

## Como executar

### Opção 1: abrir diretamente no navegador

1. Abra o arquivo [index.html.html](index.html.html) em um navegador moderno.
2. Clique em "INICIAR BANQUETE".
3. O timer começará a contar regressivamente.

### Opção 2: rodar via servidor local

Se preferir, você pode iniciar um servidor local para servir a página:

```bash
cd timer-ragnarock
python -m http.server 8000
```

Depois, abra no navegador:

```text
http://localhost:8000/index.html.html
```

## Como personalizar

### Alterar o tempo total

No arquivo [index.html.html](index.html.html), procure a variável:

```javascript
const TOTAL_SECONDS = 150; // 2 minutos e 30 segundos
```

Você pode trocar o valor para qualquer duração em segundos.

### Alterar textos e mensagens

Os textos do botão, status e modal estão no próprio arquivo HTML e podem ser alterados diretamente no JavaScript.

### Alterar o tema visual

- Ajuste as cores no bloco `style`
- Troque a imagem de fundo em `img-fundo.png`
- Customize a fonte, bordas e sombras para reforçar o visual mitológico

## Funcionalidades principais

- Contagem regressiva com atualização em tempo real
- Aviso visual quando restam menos de 10 segundos
- Reinício simples do cronômetro
- Feedback auditivo ao final da contagem
- Tela elegante e responsiva para desktop e mobile

## Observações

Este projeto é uma página estática, então não exige dependências externas de instalação. Para uso em produção, o ideal é adaptar a estrutura para um ambiente mais robusto, como React, Vite ou outro framework, caso o projeto cresça.

## Autor

Projeto criado por Vitiello na Voz.

## Dica

Se quiser, posso continuar e transformar este projeto em:

- uma versão mais moderna e responsiva,
- uma versão com seleção de tempo customizável,
- uma versão com sons e animações mais avançadas,
- ou um projeto com estrutura em React/Vite.
