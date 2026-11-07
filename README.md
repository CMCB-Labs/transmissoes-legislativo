# 🎥 Transmissões do Legislativo - CMCB

Painel interativo e responsivo de exibição e acompanhamento das **Transmissões ao Vivo e Sessões Gravadas** da Câmara Municipal de Coronel Barros/RS, conectado diretamente ao canal oficial no YouTube.

---

## 🌐 Acesso Direto
- **URL Oficial:** [https://cmcb-labs.github.io/transmissoes-legislativo/](https://cmcb-labs.github.io/transmissoes-legislativo/)

---

## ✨ Recursos
- 🔴 **Destaque em tempo real para Live:** quando uma sessão ou evento entra ao vivo no YouTube, um alerta visual animado com player automático é destacado no topo.
- 🏛️ **Acervo de transmissões anteriores:** busca instantânea por data ou número da sessão e opção de carregar mais gravações.
- 📱 **100% Responsivo e sem barra de rolagem:** integra-se com o tema do portal da Câmara disparando eventos de auto-altura (`sapl-resize`).

---

## 💻 Código para Incorporação (Embed / Iframe)

### 1. Para Notícias ou Matérias do Portal da Câmara (Recomendado)
Para embutir em matérias de notícias (ocultando o cabeçalho superior e ajustando a altura sem barras de rolagem):

```html
<iframe 
  src="https://cmcb-labs.github.io/transmissoes-legislativo/?embed=1&hide_header=1" 
  width="100%" 
  height="750" 
  frameborder="0" 
  scrolling="no" 
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen 
  style="border: none; width: 100%; min-height: 550px; overflow: hidden;">
</iframe>
```

### 2. Para a Página de Sessões ou Janela (Window) do Plone
```html
<iframe 
  src="https://cmcb-labs.github.io/transmissoes-legislativo/?embed=1" 
  width="100%" 
  height="900" 
  frameborder="0" 
  scrolling="no" 
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen 
  style="border: none; width: 100%; min-height: 700px; overflow: hidden;">
</iframe>
```

> **Parâmetros da URL:**
> - `?embed=1`: ativa modo embutido com fundo transparente e espaçamentos otimizados.
> - `&hide_header=1`: oculta o cabeçalho superior padrão (ideal para matérias de notícias que já possuem seu próprio título).
