# Estrutura Organizada do Projeto Kitchen Remodeling

## 📁 Estrutura Atual (Organizada)

```
KITCHEN REMODELING/
├── 📄 index.html                          # Landing page principal
├── 📄 thank-you.html                      # Página de obrigado
├── 📄 gerenciador_projetos.html          # Gerenciador de projetos
├── 📄 CAMPANHAS-README.md                # Documentação campanhas
│
├── 📁 google/                             # Landing page Google Ads
│   ├── index.html
│   ├── thank-you.html
│   └── [todos os assets copiados]
│
├── 📁 meta/                               # Landing page Meta Ads
│   ├── index.html
│   ├── thank-you.html
│   └── [todos os assets copiados]
│
├── 📁 ANÚNCIOS/                          # Materiais de anúncios
│
├── 📁 1. bloco herder overlay/           # Vídeos hero
│   ├── kitchen remodeling.mp4
│   └── kitchen remodeling (2).mp4
│
├── 📁 2. Bloco 2 before and after em video/  # Vídeo transformação
│
├── 📁 before and afters/                 # Imagens antes/depois
│
├── 📁 foto iago/                         # Foto CEO
│
├── 📁 kitchen bevery videos/             # Vídeos projetos
│
├── 📁 lexington-progress/                # Galeria progresso
│
├── 📁 plantas de construção/             # Blueprints
│
├── 📁 sessão de fotos slider/            # Slider fotos
│
├── 📁 video generico/                    # Vídeo genérico
│
├── 📁 galery/                            # Galeria adicional
│
├── �� ✅ 1 Lexington rd.../              # Projeto específico
│
├── 📄 logo innov builders.jpg            # Logo
│
├── 📁 .github/                           # Configurações GitHub
│   └── instructions/
│
└── 📁 .vscode/                           # Configurações VS Code

```

## ✅ Status da Organização

### Landing Pages Funcionais
- ✅ **index.html** - LP principal (raiz)
- ✅ **google/index.html** - LP Google Ads (com assets próprios)
- ✅ **meta/index.html** - LP Meta Ads (com assets próprios)

### Assets Compartilhados (Raiz)
Mantidos na raiz para a LP principal funcionar:
- Pastas de vídeos
- Pastas de imagens
- Logo
- Blueprints

### Assets Duplicados
Google e Meta têm cópias próprias dos assets para usar caminhos relativos simples.

## 🔄 Webhooks Configurados

### Todos os formulários enviam:
- NOME
- E-MAIL
- TELEFONE
- PERGUNTA (múltipla escolha)
- PLATAFORMA (detectada automaticamente pela URL)
- FONTE (título da página)
- QUANDO (timestamp)

**Detecção automática de plataforma:**
- URL contém "google" → GOOGLE ADS
- URL contém "meta/facebook/instagram" → META
- Outros → ORGÂNICO

## 📝 Arquivos de Teste
- test-form.html
- test-images.html

## 💡 Próximas Melhorias Sugeridas
1. Mover arquivos de teste para pasta /tests
2. Consolidar documentação em /docs
3. Criar README.md principal
4. Adicionar .gitignore adequado
