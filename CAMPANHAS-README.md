# Estrutura de Campanhas - Kitchen Remodeling

## 📁 Estrutura de Pastas

```
KITCHEN REMODELING/
├── index.html              # Página principal (raiz)
├── thank-you.html          # Página de agradecimento (raiz)
│
├── meta/                   # Campanha Meta/Facebook
│   ├── index.html          # Landing page: seudominio.com/meta
│   └── thank-you.html      # Thank you: seudominio.com/meta/thank-you.html
│
└── google/                 # Campanha Google Ads
    ├── index.html          # Landing page: seudominio.com/google
    └── thank-you.html      # Thank you: seudominio.com/google/thank-you.html
```

## 🔗 URLs das Campanhas

### Meta/Facebook Ads
- **Landing Page:** `https://seudominio.com/meta`
- **Thank You:** `https://seudominio.com/meta/thank-you.html`

### Google Ads
- **Landing Page:** `https://seudominio.com/google`
- **Thank You:** `https://seudominio.com/google/thank-you.html`

### Principal (Orgânico/Direto)
- **Landing Page:** `https://seudominio.com/`
- **Thank You:** `https://seudominio.com/thank-you.html`

## ✅ O que foi feito

1. ✅ Criadas pastas `/meta` e `/google`
2. ✅ Duplicados `index.html` e `thank-you.html` para cada pasta
3. ✅ Atualizados todos os caminhos de recursos (imagens, vídeos, etc.) com `../`
4. ✅ Formulários redirecionam para `thank-you.html` dentro de cada pasta
5. ✅ Página principal mantida intacta na raiz

## 📊 Tracking e Diferenciação

Para diferenciar as campanhas, você pode:

1. **Adicionar parâmetros UTM nos anúncios:**
   - Meta: `?utm_source=meta&utm_medium=paid&utm_campaign=kitchen_remodeling`
   - Google: `?utm_source=google&utm_medium=cpc&utm_campaign=kitchen_remodeling`

2. **Configurar eventos de conversão separados** no Google Analytics/Meta Pixel

3. **Usar diferentes números de telefone ou emails** (opcional) para tracking

## 🚀 Deploy

Ao fazer upload para o servidor, mantenha a estrutura de pastas:
- Raiz do domínio: `index.html` e `thank-you.html`
- Subpasta `/meta`: arquivos da campanha Meta
- Subpasta `/google`: arquivos da campanha Google

## 📝 Notas Importantes

- Todos os recursos (imagens, vídeos, CSS, JS) estão na pasta raiz
- As páginas nas pastas `/meta` e `/google` referenciam os recursos com `../`
- Cada campanha tem sua própria página de agradecimento para melhor tracking
- O formulário em cada versão redireciona para sua respectiva página thank-you

## 🔄 Atualizações Futuras

Se precisar atualizar o conteúdo:
1. Atualize a página principal (`index.html` na raiz)
2. Copie as alterações para `/meta/index.html` e `/google/index.html`
3. Execute os comandos sed novamente para corrigir os caminhos (se necessário)
