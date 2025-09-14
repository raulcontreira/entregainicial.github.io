
# Bootcamp Helper - Extensão Chrome MV3

Uma extensão simples para Google Chrome desenvolvida como projeto do Bootcamp II, utilizando Manifest V3.

## 📋 Descrição

O Bootcamp Helper é uma extensão educacional que demonstra os conceitos fundamentais do desenvolvimento de extensões para Chrome usando Manifest V3. A extensão inclui:

- **Popup Interface**: Interface amigável com botões interativos
- **Background Service Worker**: Gerenciamento de eventos em segundo plano
- **Content Script**: Manipulação de páginas web específicas
- **Storage API**: Armazenamento local de dados

## 🚀 Funcionalidades

- ✅ Popup com interface Bootstrap responsiva
- ✅ Comunicação entre popup e background script
- ✅ Content script que destaca links em páginas específicas
- ✅ Armazenamento local de dados
- ✅ Ícones em múltiplos tamanhos (16px, 32px, 48px, 128px)

## 📦 Instalação

### Modo Desenvolvedor (Recomendado para teste)

1. Abra o Chrome e navegue para `chrome://extensions/`
2. Ative o **Developer mode** no canto superior direito
3. Clique em **Load unpacked**
4. Selecione a pasta raiz do projeto
5. A extensão aparecerá na barra de ferramentas

### Estrutura do Projeto

```
bootcamp-helper/
├── src/
│   ├── popup/
│   │   ├── popup.html      # Interface do popup
│   │   └── popup.js        # Lógica do popup
│   ├── background/
│   │   └── service-worker.js # Service worker
│   ├── content/
│   │   └── content.js      # Content script
│   ├── styles/
│   │   └── style.css       # Estilos customizados
│   └── options/
│       └── options.html    # Página de opções
├── icons/
│   ├── icon16.png         # Ícone 16x16
│   ├── icon32.png         # Ícone 32x32
│   ├── icon48.png         # Ícone 48x48
│   └── icon128.png        # Ícone 128x128
├── docs/
│   └── index.html         # GitHub Pages
├── manifest.json          # Manifest V3
├── README.md             # Este arquivo
└── LICENSE               # Licença MIT
```

## 🔧 Tecnologias Utilizadas

- **Manifest V3**: Nova versão do sistema de extensões do Chrome
- **JavaScript ES6+**: Linguagem principal
- **Bootstrap 5**: Framework CSS para interface
- **Chrome Extension APIs**: 
  - `chrome.storage`
  - `chrome.runtime`
  - `chrome.tabs`

## 🛠️ Desenvolvimento

### Pré-requisitos

- Google Chrome 114+
- Editor de código (VS Code recomendado)
- Conhecimentos básicos de HTML, CSS e JavaScript

### Testando Localmente

1. Clone o repositório
2. Abra `chrome://extensions/`
3. Ative o modo desenvolvedor
4. Carregue a extensão usando "Load unpacked"
5. Teste as funcionalidades:
   - Clique no ícone da extensão para abrir o popup
   - Visite `https://developer.chrome.com/*` para ver o content script em ação
   - Verifique o console para logs do background script

### Debugging

- **Popup**: Clique com botão direito no popup → "Inspect"
- **Background**: Vá em `chrome://extensions/` → "Inspect views: background page"
- **Content Script**: Use F12 na página onde o script está ativo

## 📋 Permissões

A extensão solicita as seguintes permissões:

- `storage`: Para armazenar dados localmente
- `tabs`: Para acessar informações das abas
- `host_permissions`: Para executar content scripts em sites específicos

## 🎯 Como Usar

1. **Popup Principal**: Clique no ícone da extensão na barra de ferramentas
2. **Botão "Diga oi"**: Envia uma mensagem para o background script
3. **Botão "Reset"**: Limpa os dados armazenados
4. **Content Script**: Visite páginas do Chrome Developers para ver links destacados

## 🚀 Deploy

### GitHub Pages

O projeto inclui uma página de demonstração em `docs/index.html` que pode ser publicada via GitHub Pages:

1. Vá nas configurações do repositório
2. Ative GitHub Pages apontando para a pasta `/docs`
3. Acesse a URL gerada

## 📄 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

## 👨‍💻 Autor

**Raul Duarte**  
Projeto desenvolvido para a disciplina Bootcamp II

## 🤝 Contribuindo

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📚 Recursos Adicionais

- [Chrome Extension Documentation](https://developer.chrome.com/docs/extensions/)
- [Manifest V3 Migration Guide](https://developer.chrome.com/docs/extensions/migrating/)
- [Chrome Extension Samples](https://github.com/GoogleChrome/chrome-extensions-samples)

## 🔄 Changelog

### v1.0.0 (2024)
- ✅ Implementação inicial
- ✅ Popup com Bootstrap
- ✅ Background service worker
- ✅ Content script básico
- ✅ Documentação completa

