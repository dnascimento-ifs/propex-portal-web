---
name: portal-pesquisa
description: Skill de domínio para o portal web "Fios da Memória" (Tobias Barreto). Contém a arquitetura das seções, estrutura de dados locais, referências ao template base e diretrizes pedagógicas para orientar o aluno na programação manual de cada componente.
---

# Skill: Portal de Pesquisa — Fios da Memória (Tobias Barreto)

## 1. Contexto e Identidade Visual do Projeto
O portal é uma plataforma web estática dedicada a hospedar e divulgar a pesquisa sobre as bordadeiras de Tobias Barreto (SE), com foco especial na técnica do **Richelieu**.
- **Stack Tecnológica:** HTML5, Tailwind CSS (via CDN v4), e JavaScript Vanilla.
- **Paleta de Cores e Estilo:** 
  - Fundo neutro e acolhedor (`bg-[#FDFBF7]`, tons de `stone` e `amber-900`).
  - Tipografia clássica e elegante (`Playfair Display` para títulos e `Inter` para o corpo).
- **Modelo Base:** O projeto parte de um arquivo central (`template-base.html` ou `index.html`) que já possui a estrutura de navegação, Hero Section, seção histórica, galeria de vídeos e mapa cartográfico.

---

## 2. Estrutura de Conteúdo e Seções do Portal
O site está dividido nos seguintes blocos lógicos que serão construídos gradualmente pelo aluno:
1. **Navegação Fixa (`<header>`):** Menu com links âncora suaves (`scroll-smooth`) para as seções principais.
2. **Hero Section:** Apresentação poética e institucional da pesquisa com CTA para os vídeos e mapa.
3. **Seção Histórica e Técnica (`#historia`):** Explicação acadêmica/cultural da tradição têxtil em Tobias Barreto e da Vila Samambaia.
4. **Vozes & Vídeos (`#documentarios`):** Grid de cards estáticos simulando os mini-documentários e relatos das artesãs locais.
5. **Cartografia Social (`#cartografia`):** Seção preparada para receber um mapa interativo (Leaflet ou Google My Maps) mapeando ateliês e associações.
6. **Rodapé (`<footer>`):** Assinatura institucional do projeto de pesquisa.

---

## 3. Diretrizes de Organização de Dados Locais
Como o portal opera inteiramente local (sem banco de dados de backend):
- **Artigos e Relatos:** Caso sejam adicionados novos textos ou artigos da pesquisa, eles devem ser organizados em arquivos estáticos dedicados (ex: uma pasta `/artigos/` ou incorporados modularmente via JavaScript com arquivos JSON locais).
- **Modularização Futura:** Conforme o site crescer, componentes repetitivos (como os cards de vídeos) poderão ser gerados dinamicamente via JavaScript puro a partir de uma estrutura de dados local.

---

## 4. Diretrizes Pedagógicas para o Mentor (Antigravity)
Sempre que esta skill for acionada pelo aluno para evoluir o portal:
- **Respeitar o Design System:** Manter rigorosamente a consistência com as classes do Tailwind (`amber-900`, `stone-800`, `font-serif-custom`, etc.) definidas no modelo base.
- **Abordagem Socrática:** Nunca entregar blocos inteiros de código prontos. Conduzir o aluno a preencher a lógica passo a passo, explicando o fluxo mental antes de mexer na sintaxe.
- **Manutenção do Template:** Auxiliar o aluno a expandir o modelo base de forma limpa, garantindo que ele compreenda o papel de cada tag HTML e classe CSS utilizada.