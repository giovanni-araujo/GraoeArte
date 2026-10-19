☕ Grão & Arte - Torrefação e Café Especial

Landing page institucional desenvolvida para a Grão & Arte, uma torrefação de cafés especiais com clube de assinatura mensal. Projeto focado na aplicação de conceitos fundamentais do desenvolvimento Front-End: semântica HTML5, arquitetura CSS limpa, metodologia BEM, acessibilidade, responsividade e escala tipográfica dinâmica.

📌 Sumário

Visão Geral e Objetivo

Tecnologias e Conceitos Aplicados

Organização da Arquitetura

Instruções de Visualização e Execução

Funcionalidades e Seções

Principais Desafios Técnicos e Aprendizados

Contato e Créditos

🎯 Visão Geral e Objetivo

Este projeto foi desenvolvido como parte das atividades práticas do curso de desenvolvimento Front-End (Escola SENAI Henrique Lupo). O objetivo principal é simular uma entrega profissional completa para um cliente fictício, aplicando boas práticas de código e design system consistente.

A aplicação apresenta a marca Grão & Arte, com foco em:

Divulgação de microlotes de café 100% Arábica (pontuação 85+ SCA).

Apresentação do processo artesanal de torra.

Comparativo dos planos do Clube de Assinatura.

FAQ interativo e canal direto de atendimento via WhatsApp.

🛠️ Tecnologias e Conceitos Aplicados

HTML5 Semântico: Estruturação acessível utilizando tags como <header>, <nav>, <main>, <section>, <article>, <details>, <summary> e <footer>.

CSS3 Moderno:

Variáveis CSS (Design Tokens) para padronização de cores, tipografia, sombras e transições.

Flexbox para alinhamentos e layouts fluidos dos cards.

Metodologia BEM (Block Element Modifier) para nomenclatura de classes, garantindo modularidade e legibilidade.

Escala Relativa e REM: Elemento raiz ajustado proporcionalmente para resgatar a escala base, com tipografia, espaçamentos e bordas usando unidades rem.

Unidades de Layout: Uso de %, vw e vh para seções responsivas, restringindo px estritamente a bordas e detalhes de alta precisão.

Tipografia Externa: Pesquisa e importação via Google Fonts:

Merriweather (pesos 400 e 700) para títulos.

Open Sans (pesos 400, 600 e 700) para corpo de texto e navegação.

Recursos Visuais: Placeholders dinâmicos via Placehold.co e ícones/links integrados.

Integração WhatsApp API: Direcionamento direto para atendimento oficial.

📂 Organização da Arquitetura

O projeto foi estruturado seguindo o princípio da separação de responsabilidades (RNF04), sem o uso de estilos inline ou blocos <style> embutidos no HTML:

grao-e-arte/
├── assets/
│   ├── css/
│   │   ├── variables.css   # Tokens de Design System (:root)
│   │   ├── global.css      # Reset, tipografia base e regras de escala REM
│   │   ├── components.css  # Estilos BEM (cards, botões, header, footer, faq)
│   │   └── media-queries.css # Regras de responsividade e breakpoints
│   └── images/             # Imagens e vetores do projeto
├── index.html              # Estrutura HTML5 semântica da aplicação
└── README.md               # Documentação completa do projeto

📋 Funcionalidades e Seções

[RF01 & RF02] Menu Superior Fixo & Navegação Suave: Header fixo (position: fixed) com compensação de recuo superior (padding-top) nas seções para evitar que o conteúdo seja coberto ao clicar nos links de navegação.

[RF03] Layout de Seções:

Banner Principal (#inicio): Chamada visual cobrindo 100% da área visível (100vh).

Catálogo de Grãos (#graos): Exibição dos microlotes Reserva da Serra, Chapada Diamantina e Vulcânico em cards padronizados.

Processo Artesanal (#processo): Exposição dos passos da colheita ao perfil de torra.

Clube de Assinatura (#assinatura): Tabela comparativa dos planos Entusiasta, Barista e Mestre da Torra.

[RF04] FAQ Interativo (#faq): Perguntas e respostas sanadas de forma nativa através de <details> e <summary>.

[RF05] Rodapé Fixo: Rodapé fixado com dados institucionais e direitos autorais.

[RF06] Botão Flutuante do WhatsApp: Botão fixo no canto inferior direito configurado para acionar diretamente o número oficial da Escola SENAI Henrique Lupo.

[RF07] Efeitos Interativos: Microinterações com pseudo-classes :hover, sombras dinâmicas e transições suaves nos cards e navegação.

🎓 Principais Desafios Técnicos e Aprendizados

Compensação do Header Fixo:

Desafio: Ao clicar nos links do menu com scroll-behavior: smooth, o topo da seção ficava escondido atrás do header fixo.

Solução: Aplicação de scroll-margin-top nas seções com o valor equivalente à altura do header.

Ajuste Fino da Escala REM e BEM:

Desafio: Manter a consistência visual em telas de diferentes dimensões sem quebrar as proporções.

Solução: Definir font-size: 62.5% na raiz html para facilitar o cálculo relativo (1rem = 10px) e aplicar rigorosamente a convenção BEM (ex: .card, .card__title, .card--highlight).

Responsividade Fluida:

Desafio: Adaptar as seções de layout de tela cheia sem gerar rolagem horizontal ou sobreposição de texto em dispositivos móveis.

Solução: Uso de unidades relativas (%, vw, vh) alinhado a Breakpoints estratégicos para smartphones, tablets e desktops via @media.

✉️ Contato e Créditos

Instituição: Escola SENAI Henrique Lupo

Projeto: Grão & Arte - Torrefação e Café Especial (Turma A)

Desenvolvido por: Giovanni Araújo

Telefone de Atendimento (SENAI): Integrado diretamente ao botão flutuante do WhatsApp.