# 🏗️ Kitchen Remodeling - Innov Builders
## Landing Pages para Campanhas Google Ads e Meta Ads

---

## 📋 Visão Geral

Projeto de landing pages otimizadas para conversão de leads de kitchen remodeling em Massachusetts, com formulários integrados a webhooks e detecção automática de origem da campanha.

---

## 🌐 Landing Pages Ativas

### 1. **Página Principal** (`index.html`)
- URL: Raiz do domínio
- Uso: Tráfego orgânico e direto
- Plataforma detectada: **ORGÂNICO**

### 2. **Google Ads** (`/google/index.html`)
- URL: `/google/`
- Uso: Campanhas Google Ads
- Plataforma detectada: **GOOGLE ADS**

### 3. **Meta Ads** (`/meta/index.html`)  
- URL: `/meta/`
- Uso: Campanhas Meta/Facebook/Instagram
- Plataforma detectada: **META**

---

## 📊 Webhook & Formulários

### Campos Enviados em Todos os Forms:
```json
{
  "NOME": "Nome do lead",
  "E-MAIL": "email@exemplo.com",
  "TELEFONE": "(123) 456-7890",
  "PERGUNTA": "full-renovation, partial-remodel",
  "PLATAFORMA": "META | GOOGLE ADS | ORGÂNICO",
  "FONTE": "Título da página",
  "QUANDO": "15/12/2025, 10:30:45"
}
```

### Detecção Automática de Plataforma:
- URL contém **"google"** → `GOOGLE ADS`
- URL contém **"meta"**, **"facebook"** ou **"instagram"** → `META`
- Outros casos → `ORGÂNICO`

### Webhook URL:
```
https://hook.us2.make.com/ctp3mh229k0mi9ujiy1xcu1xh84fpa3x
```

---

## 📁 Estrutura de Arquivos

```
KITCHEN REMODELING/
├── 📄 index.html                     # LP principal
├── 📄 thank-you.html                 # Página obrigado
├── 📄 gerenciador_projetos.html     # Gerenciador
├── 📄 logo innov builders.jpg       # Logo
│
├── 📁 google/                        # LP Google Ads (completa)
│   ├── index.html
│   ├── thank-you.html
│   └── [assets copiados]
│
├── 📁 meta/                          # LP Meta Ads (completa)
│   ├── index.html
│   ├── thank-you.html
│   └── [assets copiados]
│
├── 📁 1. bloco herder overlay/       # Vídeos hero
├── 📁 2. Bloco 2 before.../          # Vídeo transformação
├── 📁 before and afters/             # Imagens antes/depois
├── 📁 foto iago/                     # Foto CEO
├── 📁 kitchen bevery videos/         # Vídeos projetos
├── 📁 lexington-progress/            # Galeria progresso
├── 📁 plantas de construção/         # Blueprints
├── 📁 sessão de fotos slider/        # Slider fotos
├── 📁 video generico/                # Vídeo genérico
├── 📁 galery/                        # Galeria adicional
├── 📁 ANÚNCIOS/                     # Materiais anúncios
├── 📁 _archive/                      # Arquivos teste/backup
│
├── 📁 .github/instructions/          # Regras Snyk/Copilot
└── 📁 .vscode/                       # Config VS Code
```

---

## 🚀 Como Usar

### Visualizar Localmente:
```bash
# Iniciar servidor local
cd "KITCHEN REMODELING"
python3 -m http.server 8080

# Acessar no navegador:
# http://localhost:8080/              (LP principal)
# http://localhost:8080/google/       (LP Google)
# http://localhost:8080/meta/         (LP Meta)
```

### Deploy:
- Upload para servidor web
- URLs sugeridas:
  - `dominio.com/` → index.html principal
  - `dominio.com/google/` → Google Ads
  - `dominio.com/meta/` → Meta Ads

---

## 🎯 Tracking & Analytics

### Meta Pixel (Meta Ads):
```javascript
fbq('init', '811056244975308');
fbq('track', 'PageView');
```

### Microsoft Clarity:
```javascript
clarity("u1d4stb1wy");
```

---

## ✅ Checklist de Validação

- [x] Landing pages funcionais (principal, google, meta)
- [x] Formulários com validação
- [x] Webhook integrado e testado
- [x] Detecção automática de plataforma
- [x] Assets (imagens/vídeos) carregando
- [x] Responsivo mobile
- [x] Meta Pixel instalado
- [x] Microsoft Clarity instalado
- [x] Thank-you pages configuradas

---

## 📞 Contato Innov Builders

- **Telefone:** (978) 871-0597
- **Email:** contact@innovbuildersusa.com
- **Endereço:** 50 New Salem St, Wakefield, MA 01880
- **HIC License:** 212869

---

## 📝 Notas de Desenvolvimento

### Assets Duplicados:
As pastas `google/` e `meta/` contêm cópias completas de todos os assets para usar caminhos relativos simples, facilitando manutenção e evitando erros 404.

### Arquivos de Teste:
Movidos para `_archive/` para manter workspace limpo.

### Próximas Melhorias:
1. A/B testing de headlines
2. Formulário multi-step
3. Chat ao vivo
4. Calculadora de orçamento
5. Vídeos testemunhais adicionais

---

**Última atualização:** 15 de dezembro de 2025
