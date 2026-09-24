---
name: escolher-animacoes-ui
description: Escolher e integrar animações ou componentes dos catálogos Unlumen UI, Magic UI, SmoothUI, Retro UI e Canvas UI em sites e apps web. Use quando o usuário pedir animações, microinterações ou um componente dessas bibliotecas para uma interface. Não use para tarefas sem interface visual.
---

# Escolher animações para o site

O usuário indicou cinco catálogos: Unlumen UI, Magic UI, SmoothUI, Retro UI e Canvas UI. Use-os como fontes de opções, sem animar toda tela por padrão.

## Catálogos

| Fonte | Catálogo oficial | Uso provável |
| --- | --- | --- |
| Unlumen UI | https://ui.unlumen.com/components | Primitivos e componentes React animados; conferir dependências e disponibilidade de cada item. |
| Magic UI | https://magicui.design/docs/components | Efeitos de texto, fundo, destaque e componentes para páginas de apresentação. |
| SmoothUI | https://smoothui.dev/docs/components | Microinterações, transições e componentes React com Motion ou GSAP. |
| Retro UI | https://retroui.io/ | Componentes React com estética pixelada. O nome também foi usado por https://retroui.dev/; esse endereço redireciona para https://neobrutalism.com/. Se o usuário pedir um componente específico de “Retro UI”, confirmar qual catálogo ele quer. |
| Canvas UI | https://canvasui.dev/components | Efeitos visuais em canvas, WebGL ou WebGPU. Há versões para React, Solid, Preact, Vue, Svelte e TypeScript puro. Conferir suporte do navegador e degradação antes de escolher um efeito. |

## Como decidir

1. Ler a interface existente: stack, estilo, componentes, propósito da tela e comportamento que precisa melhorar. Respeitar uma biblioteca já adotada pelo projeto.
2. Escolher uma animação que tenha função clara: sinalizar estado, orientar atenção, confirmar ação, mostrar relação espacial ou reforçar a identidade visual. Preferir poucas animações coerentes.
3. Consultar a página atual do componente escolhido antes de implementar. Verificar API, instalação, dependências, licença e eventuais partes pagas. Não inventar comando de instalação nem copiar código de uma versão antiga. Para Canvas UI, verificar se o efeito depende de capacidade experimental do navegador e garantir que o conteúdo continue utilizável sem ele.
4. Integrar no código do projeto e adaptar cores, tipografia, duração e intensidade ao design existente. Manter interação por teclado, foco visível e conteúdo compreensível sem animação. Respeitar `prefers-reduced-motion`.
5. Verificar o resultado no navegador em desktop e celular, incluindo desempenho, layout e estados de interação. Ajustar ou remover o efeito se atrapalhar leitura, uso ou velocidade.

Se a stack não for compatível com o componente escolhido, procurar alternativa compatível no mesmo catálogo ou implementar um efeito simples com CSS nativo. Explicar ao usuário qual animação foi escolhida e por que combina com aquela tela.
