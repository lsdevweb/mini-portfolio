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
### 🔄 Auditoria e Melhoria Contínua (Pós-Deploy)

Após o deploy inicial da aplicação na infraestrutura da Netlify, o projeto foi submetido a testes de estresse e auditorias rigorosas através do **W3C Markup Validation Service** e do **Google PageSpeed Insights**. Com base nos diagnósticos em ambiente de produção, foram aplicadas as seguintes otimizações estruturais:

* **Refatoração Semântica e Acessibilidade (W3C):** Correção de aninhamentos de tags de cabeçalho (`<h3>`, `<h5>`) e ajustes nos atributos de acessibilidade (`aria-labelledby`) dos modais Bootstrap. O resultado eliminou 100% dos alertas de sintaxe, elevando a nota de **Acessibilidade para 95+**.
* **Otimização do Critical Rendering Path (PageSpeed):** Antecipação da resolução de DNS e handshake através da implementação de diretivas `preconnect` no topo do `<head>` para ativos críticos (Google Fonts e iframes do YouTube), reduzindo o tempo de bloqueio de renderização.
* **Eficiência de Ativos e Resolução de Imagem:** Identificação e redimensionamento físico da imagem de perfil (passando de uma resolução de câmera nativa para 400x533px em formato comprimido de 73KB via GIMP). Isso solucionou o aviso de *imagem maior do que as dimensões exibidas*, otimizando o consumo de dados móveis.
* **Ajuste de Enquadramento Responsivo (Mobile):** Correção na folha de estilo dentro da `@media query (max-width: 767.98px)` para estabilizar as dimensões do container da foto, utilizando `object-position: center 20%` para garantir o enquadramento perfeito do rosto sem cortes agressivos em telas verticais de smartphones.

#### 🚀 Próximos Passos & Evolução Futura
* **Lazy Loading Avançado:** Implementar o carregamento tardio dinâmico (com JavaScript) para o iframe do YouTube, fazendo com que o player de vídeo só consuma processamento e rede após a primeira interação do usuário, visando cravar a nota de Desempenho Mobile em **100/100**.
* **Conversão para WebP:** Migrar as imagens do formato tradicional `.jpg` para formatos de última geração como `.webp` ou `.avif` para reduzir ainda mais o peso total da página no carregamento inicial.
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
