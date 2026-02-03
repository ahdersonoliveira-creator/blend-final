# 📊 Gerador de Blends - Sistema de Cinzas

Sistema completo para geração e gerenciamento de blends de cinzas com autenticação, histórico e funcionalidade offline.

## 🎯 Funcionalidades Implementadas

### ✅ Novas Funcionalidades
1. **Sistema de Histórico Completo**
   - Salvamento automático ao clicar em "Salvar Lote"
   - Visualização de todos os lotes salvos
   - Informações detalhadas: data, status, PCS, cinza, toneladas
   - **Exclusão de lotes** - remova lotes indesejados do histórico
   - Status visual (APROVADO ✅ / REPROVADO ❌)

2. **Funcionalidade Offline**
   - Service Worker implementado
   - Funciona sem internet após primeiro acesso
   - Dados salvos localmente no navegador
   - Progressive Web App (PWA)

3. **Hospedagem Gratuita**
   - Pronto para deploy em plataformas gratuitas
   - Compatível com: GitHub Pages, Netlify, Vercel, Render

### 📋 Funcionalidades Originais (Mantidas)
- Sistema de autenticação com usuários
- Cálculo automático de blends
- Otimização de custos
- Geração de relatórios PDF
- Exportação JSON
- Gerenciamento de estoque
- Temas claro/escuro
- Layout responsivo

## 🚀 Como Usar Localmente (Offline)

### Opção 1: Abrir Diretamente no Navegador
1. Baixe todos os arquivos para uma pasta no seu computador
2. Abra o arquivo `index.html` no seu navegador (Chrome, Edge, Firefox)
3. O sistema funcionará completamente offline!

### Opção 2: Servidor Local Simples (Recomendado)
Para melhor funcionamento do Service Worker:

**Windows:**
```cmd
cd caminho\da\pasta
python -m http.server 8000
```

**Linux/Mac:**
```bash
cd /caminho/da/pasta
python3 -m http.server 8000
```

Depois acesse: `http://localhost:8000`

## 🌐 Como Hospedar Gratuitamente

### Opção 1: GitHub Pages (Recomendado)
1. Crie uma conta no GitHub (gratuito)
2. Crie um novo repositório
3. Faça upload dos arquivos: `index.html`, `manifest.json`, `sw.js`
4. Vá em Settings → Pages
5. Selecione a branch `main` e clique em Save
6. Seu site estará em: `https://seu-usuario.github.io/nome-repositorio`

### Opção 2: Netlify
1. Acesse [netlify.com](https://www.netlify.com)
2. Crie uma conta gratuita
3. Arraste a pasta com os arquivos para o Netlify Drop
4. Pronto! Seu site estará online em segundos

### Opção 3: Vercel
1. Acesse [vercel.com](https://vercel.com)
2. Crie uma conta gratuita
3. Clique em "New Project"
4. Faça upload dos arquivos
5. Deploy automático!

### Opção 4: Render
1. Acesse [render.com](https://render.com)
2. Crie uma conta gratuita
3. Crie um "Static Site"
4. Conecte seu repositório GitHub ou faça upload
5. Deploy automático!

## 📁 Arquivos Necessários

```
gerador-blends/
├── index.html          (Arquivo principal - 114KB)
├── manifest.json       (Configuração PWA)
├── sw.js              (Service Worker para offline)
└── README.md          (Este arquivo)
```

## 🔐 Usuário Padrão

- **Usuário:** Anderson
- **Senha:** 200678
- **Tipo:** Administrador

## 💾 Armazenamento de Dados

Todos os dados são salvos localmente no navegador usando:
- **localStorage** - para materiais, configurações e usuários
- **sessionStorage** - para sessão de login

**Importante:** Os dados são específicos de cada navegador/dispositivo. Para sincronizar entre computadores, use as opções de exportar/importar usuários e dados.

## 🔧 Solução de Problemas

### O histórico não aparece
- Certifique-se de clicar em "Salvar Lote" antes de verificar o histórico
- Verifique se o navegador permite localStorage

### Service Worker não funciona
- Use um servidor local (http.server) em vez de abrir o arquivo diretamente
- Ou hospede online em uma das plataformas sugeridas

### Dados perdidos ao trocar de computador
- Os dados são salvos localmente no navegador
- Use as funções de exportar/importar para transferir dados
- Ou hospede online para acesso de qualquer lugar

## 📱 Compatibilidade

- ✅ Chrome/Edge (Recomendado)
- ✅ Firefox
- ✅ Safari
- ✅ Opera
- ✅ Navegadores móveis (Android/iOS)

## 🆘 Suporte

Para dúvidas ou problemas:
1. Verifique se todos os arquivos estão na mesma pasta
2. Teste em um navegador atualizado
3. Limpe o cache do navegador se necessário
4. Use o console do navegador (F12) para verificar erros

## 📄 Licença

Sistema desenvolvido para uso interno da Carbonífera Catarinense.

---

**Versão:** 2.0 com Histórico e Exclusão  
**Data:** Fevereiro 2026  
**Desenvolvido por:** Manus AI
