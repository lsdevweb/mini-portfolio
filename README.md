# 📱 Mini-Portfólio Cartão Virtual (Dobra Única)

Aplicação desenvolvida sob uma abordagem moderna e ágil para portfólios técnicos. O site funciona como um cartão de visitas digital e interativo, projetado sob o conceito estrito de **Dobra Única (Above the Fold)** para monitores desktop, com foco total em máxima performance, conversão e acessibilidade.

---

## 🚀 Objetivo do Projeto

O objetivo deste projeto é centralizar a presença web com um alto índice de conversão, direcionando potenciais clientes e redes profissionais diretamente para canais estratégicos (como GitHub e WhatsApp). A interface concentra todas as informações essenciais (perfil, portfólio de serviços, vídeo de demonstração dinâmico e conformidade com privacidade) em um único espaço visual, eliminando a necessidade de rolagem em telas desktop.

---

## 🛠️ Stack Tecnológica & Recursos

- **HTML5**: Estrutura semântica e acessível.
- **CSS3 Personalizado**: Gerenciamento de variáveis nativas (`:root`), animações de atenção para chamadas de ação (CTAs) e controle estrutural de limites de tela.
- **Bootstrap 5 (via CDN)**: Uso de classes utilitárias, sistema de grid responsivo para dispositivos móveis e componentes nativos leves.
- **PWA (Progressive Web App)**: Configuração de manifesto web (`manifest.json`) e múltiplos tamanhos de ícones personalizados, permitindo que a página seja instalada no celular do usuário como um aplicativo de verdade.
- **Google Tag Manager**: Integração limpa para monitoramento avançado de acessos e coleta de métricas de engajamento de forma não intrusiva.

---

## ⚙️ Arquitetura e Diferenciais Técnicos

### 1. Desempenho Estrito (Foco no PageSpeed)
- **Zero Framework Overhead**: Construído com foco em carregamento instantâneo, otimizando a experiência mesmo em redes móveis limitadas.
- **Modais Embutidos**: Elementos secundários, como a Política de Privacidade, foram acoplados em Modais responsivos do Bootstrap em vez de páginas externas, mantendo a árvore do DOM leve e garantindo ótimas notas nos critérios de auditoria web.
- **Padronização de Ativos**: Configuração completa de favicons multiplataforma (`16x16`, `32x32`, `apple-touch-icon`) para evitar erros de requisição e quebras de layout no navegador.

### 2. Controle de Interface (UX/UI)
- **Bloqueio de Rolagem em Desktop**: Trava estrita de tela em resoluções acima de `768px` através de regras de `overflow: hidden`, garantindo que o design visual se mantenha intacto na dobra única.
- **Fallback Fluido para Mobile**: Transição automática para rolagem vertical padrão em telas menores, assegurando usabilidade contínua em qualquer smartphone.

---

## 📂 Estrutura do Repositório

```text
📂 mini-portfolio/
├── 📄 index.html                      # Estrutura HTML principal e estilos CSS internos
├── 📄 manifest.json                   # Manifesto web para habilitar recursos de PWA
├── 🖼️ perfil.jpg                       # Imagem de perfil principal otimizada
├── 🖼️ android-chrome-192x192.png       # Ícone do aplicativo para telas mobile padrão
├── 🖼️ android-chrome-512x512.png       # Ícone do aplicativo para a tela de abertura (Splash)
├── 🖼️ apple-touch-icon.png            # Ícone de exibição específico para dispositivos iOS
├── 🖼️ favicon-16x16.png                # Micro-ícone para a barra de navegação do navegador
├── 🖼️ favicon-32x32.png                # Ícone padrão em alta resolução para abas de desktop
└── 🖼️ favicon.ico                     # Ícone de compatibilidade para navegadores legados