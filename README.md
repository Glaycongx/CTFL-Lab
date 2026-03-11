# 🧪 CTFL Lab — Módulo de Estudos

> Plataforma completa de estudos para a certificação **ISTQB Certified Tester Foundation Level (CTFL) v4.0** — instalável como PWA em Android e iOS.

[![GitHub Pages](https://img.shields.io/badge/Live-GitHub%20Pages-6c63ff?style=flat-square)](https://seu-usuario.github.io/ctfl-lab/CTFL_4.0_Estudos.html)

---

## 📚 Conteúdo

| # | Capítulo | Tempo |
|---|----------|-------|
| 1 | Fundamentos de Teste | 180 min |
| 2 | Testes ao Longo do Ciclo de Vida | 130 min |
| 3 | Teste Estático | 80 min |
| 4 | Análise e Modelagem de Teste | 390 min |
| 5 | Gerenciamento das Atividades de Teste | 335 min |
| 6 | Ferramentas de Teste | 20 min |

## ✨ Funcionalidades

- 📖 **6 capítulos** completos com conteúdo alinhado ao Syllabus CTFL 4.0
- 🃏 **Flashcards interativos** por capítulo com rastreamento Acertei/Errei
- 📝 **3 Simulados** (40 questões · 75 min · aprovação 65%) com opção de aleatorização
- 🎯 **Treino por Capítulo** com feedback imediato
- 🔍 **Glossário** com 150+ termos oficiais ISTQB
- 🌙 **Tema escuro/claro** persistido
- 📊 **Progresso** salvo localmente (localStorage)
- 📶 **Funciona offline** (PWA com Service Worker)
- 📱 **Instalável** em Android e iOS

## 🚀 Instalação como PWA

### Android (Chrome)
1. Abra o app no Chrome
2. Toque no ícone de menu (⋮) → "Adicionar à tela inicial"
3. Ou aguarde o banner de instalação aparecer

### iOS (Safari)
1. Abra no Safari
2. Toque no botão de compartilhar (□↑)
3. Selecione "Adicionar à Tela de Início"

## 🛠️ Setup do Projeto

### 1. Gerar os ícones (uma única vez)
```bash
# Abra no navegador e clique em "Baixar Todos"
open generate-icons.html

# Mova os ícones baixados para a pasta icons/
mv ~/Downloads/icon-*.png icons/
```

### 2. Rodar localmente
```bash
# Com Python (mais simples)
python3 -m http.server 8080
# Acesse: http://localhost:8080/CTFL_4.0_Estudos.html

# Com Node.js
npx serve .
```

> ⚠️ O Service Worker requer que o app seja servido via HTTP(S), não via `file://`.

### 3. Deploy no GitHub Pages
```bash
git init
git add .
git commit -m "feat: CTFL Lab PWA study app"
git remote add origin https://github.com/SEU-USUARIO/ctfl-lab.git
git push -u origin main

# Ativar em: Settings → Pages → Branch: main → Save
```

## 📁 Estrutura do Projeto

```
CTFLTrainning/
├── CTFL_4.0_Estudos.html   # App principal (HTML + CSS + JS inline)
├── manifest.json            # Configuração PWA
├── sw.js                    # Service Worker (cache offline)
├── generate-icons.html      # Gerador de ícones PNG
├── icons/
│   ├── icon-72.png
│   ├── icon-96.png
│   ├── icon-128.png
│   ├── icon-144.png
│   ├── icon-152.png
│   ├── icon-192.png
│   ├── icon-384.png
│   ├── icon-512.png
│   ├── icon-maskable-192.png
│   └── icon-maskable-512.png
└── README.md
```

## 📋 Baseado em

- [ISTQB® CTFL Syllabus v4.0](https://www.istqb.org/certifications/certified-tester-foundation-level)
- [BSTQB — Syllabus em Português](https://bstqb.online)
- [ISO/IEC 25010](https://www.iso.org/standard/35733.html) — Modelo de Qualidade
- [ISO/IEC 20246](https://www.iso.org/standard/68238.html) — Work Product Reviews
