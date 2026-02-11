# 📺 Transmissões Legislativas – Câmara Municipal de Coronel Barros

Página estática para exibição automática:

- 🔴 Transmissão ao vivo (quando houver sessão em andamento)
- 📼 Lista das transmissões anteriores
- Pronto para uso via **GitHub Pages**
- Integrável ao site oficial via **iframe (embed)**

---

## 🔗 Canal Oficial

Canal da Câmara no YouTube:  
https://www.youtube.com/@CamaraCoronelBarros

Channel ID utilizado:
```
UCl8gLTIMl99eKsKj7DNUWGg
```

---

## 🚀 Como funciona

A página utiliza a **YouTube Data API v3** para:

1. Verificar automaticamente se existe transmissão ao vivo no canal
2. Exibir o player ao vivo com destaque
3. Listar as transmissões concluídas mais recentes

Tudo é carregado dinamicamente via JavaScript.

---

## 🔑 Configuração da API

Para funcionamento correto, é necessário:

1. Criar um projeto no Google Cloud Console  
2. Ativar a **YouTube Data API v3**
3. Gerar uma **API Key**
4. Inserir a chave no arquivo `index.html`:

```javascript
const API_KEY = "SUA_API_KEY_AQUI";
```

Recomenda-se restringir a chave para uso apenas no domínio do GitHub Pages.

---

## 🌐 Publicação no GitHub Pages

1. Acesse **Settings → Pages**
2. Selecione:
   - Source: `Deploy from branch`
   - Branch: `main`
   - Folder: `/root`
3. Salve

A página ficará disponível em:

```
https://cmcb-labs.github.io/transmissoes-legislativo/
```

---

## 🧩 Como incorporar no site da Câmara

Utilize um iframe:

```html
<iframe 
    src="https://cmcb-labs.github.io/transmissoes-legislativo/"
    width="100%"
    height="900"
    frameborder="0">
</iframe>
```

---

## 📁 Estrutura do Projeto

```
/transmissoes-legislativo
 ├── index.html
 └── README.md
```

---

## ⚙️ Funcionalidades

- Detecção automática de live
- Exibição das últimas transmissões
- Layout responsivo
- Atualização automática ao carregar a página
- Sem necessidade de backend

---

## 🏛️ Desenvolvido por

Câmara Municipal de Coronel Barros  
Organização GitHub: https://github.com/CMCB-Labs

---

## 📌 Observações

- Caso não haja transmissão ao vivo, será exibida mensagem informativa.
- O número de transmissões listadas pode ser ajustado alterando o parâmetro:
  ```
  maxResults=12
  ```
- O sistema depende do limite de requisições da API do YouTube.
