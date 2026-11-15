# 👂 ore.ia — o renderizador ia

> **Transforme qualquer imagem ou print do seu projeto em um render fotorrealista profissional em segundos.**

Uma plataforma de visualização arquitetônica baseada em Inteligência Artificial criada para arquitetos, designers de interiores, engenheiros e estudantes que desejam gerar imagens de alta fidelidade sem depender de softwares pesados ou configurações técnicas complexas de renderização.

🌐 **Aplicação no Ar:** [https://oreia.lovable.app/](https://oreia.lovable.app/)  

---

## 🎯 1. A Dor Escolhida e Por Que Vale um Negócio

### A Dor Real do Mercado
Profissionais e estudantes de arquitetura e design passam por gargalos diários para apresentar projetos aos clientes:
1. **Lentidão extrema e hardware caro:** Softwares tradicionais de renderização (V-Ray, Lumion, Corona) demandam computadores de alta performance com placas de vídeo caras e levam horas para processar uma única cena.
2. **Complexidade técnica desnecessária:** Configurar materiais complexos (bump, reflexos), física de iluminação solar e distribuição de spots e fitas de LED exige conhecimento avançado.
3. **Prazos apertados:** O cliente quer ver opções rápidas ("como fica de noite?", "e com luz natural?"), e o profissional perde dias apenas modelando bloquinhos de decoração e renderizando novamente.

### Por Que Vale um Negócio?
O setor de Arquitetura, Engenharia e Construção (AEC) movimenta bilhões e tem altíssima urgência por agilidade na apresentação e aprovação de projetos. Reduzir o tempo de entrega de 8 horas para menos de 60 segundos por imagem gera um ganho de produtividade imenso, tornando o modelo de assinatura anual extremamente atraente e lucrativo.

---

## 📊 2. Tamanho de Mercado (TAM, SAM e SOM) & Business Model Canvas

### Estimativa de Mercado
* **TAM (Total Addressable Market):** Mercado global de softwares de renderização e visualização arquitetônica 3D, estimado em mais de **US$ 3,5 bilhões**.
* **SAM (Serviceable Addressable Market):** Mercado brasileiro e latino-americano de escritórios de arquitetura, designers de interiores autônomos e estudantes universitários que utilizam SketchUp, Revit e Archicad diariamente (~**R$ 380 milhões**).
* **SOM (Serviceable Obtainable Market):** 500 a 1.200 arquitetos autônomos e freelancers atingidos via redes sociais (Instagram/TikTok) e comunidades de arquitetura no primeiro ano (~**R$ 250.000 a R$ 600.000 ARR**).

### Business Model Canvas Sintético

| Bloco | Descrição |
| :--- | :--- |
| **Proposta de Valor** | Renders fotorrealistas em menos de 60s via IA a partir de prints/capturas, com controle de horário solar, LEDs em marcenaria, ambientação automática e pós-produção integrada. |
| **Segmento de Clientes** | Arquitetos, designers de interiores, desenhistas cadistas, estudantes de arquitetura e profissionais de visualização imobiliária. |
| **Canais** | Landing Page responsiva, Arquitiktok, Instagram Reels com "Antes e Depois", tráfego direto e fechamento de planos no WhatsApp. |
| **Relacionamento com Clientes** | Modelo *Product-Led Growth (Freemium)*: 3 testes gratuitos imediatos, comunidade e atendimento próximo e consultivo via WhatsApp para assinaturas anuais. |
| **Fontes de Receita** | • **Plano Starter Anual:** R$ 297/ano (10 renders/dia)<br>• **Plano Pro Anual:** R$ 497/ano (Renders 4K ilimitados sem marca d'água)<br>• **Upgrades de plano** |
| **Recursos-Chave** | Motor de IA generativa especializada em arquitetura, interface intuitiva (Dark Theme com suporte a `Ctrl+V`), banco de dados Lovable Cloud. |
| **Atividades-Chave** | Curadoria de estilo arquitetônico da IA, marketing de conteúdo visual (Antes e Depois) e gestão de assinaturas no painel `/admin`. |
| **Parcerias-Chave** | Lovable Cloud / Supabase, fornecedores de APIs de IA generativa e comunidades do nicho de arquitetura/interiores. |
| **Estrutura de Custos** | Custos de infraestrutura e processamento de IA por imagem, hospedagem e taxa de processamento de pagamentos. |

---

## 🧪 3. A Tese do MVP e o que Ficou Manual de Propósito

### A Tese Validada pelo MVP
> *"Profissionais de arquitetura e design preferem enviar um print rápido com atalho `Ctrl+V` e configurar luz e LEDs com 1 clique para gerar um render em 60 segundos do que passar horas configurando o V-Ray."*

### O Que Ficou Manual de Propósito
Seguindo as boas práticas de MVP enxuto:
1. **Fechamento e Cobrança da Assinatura Anual:** Ao atingir o limite de 3 renders gratuitos, o usuário é direcionado para o **WhatsApp** com uma mensagem pré-formatada. O pagamento via Pix ou link de cartão é combinado manualmente.
2. **Ativação e Liberação de Planos:** O administrador acessa a rota `/admin` e altera com um clique o status do cliente de `"Gratuito (3 Testes)"` para `"Starter Ativo"` ou `"Pro Ilimitado"`, sem necessidade de integração complexa de webhooks/gateways no primeiro momento.

---

## 🎨 4. Identidade Visual do Produto

* **Preto Grafite (`#1D1D1B`):** Fundo principal, painéis laterais e cards de alto contraste.
* **Branco Gelo (`#F9F5EF`):** Textos principais, tipografia e seções de alta legibilidade.
* **Lilás Claro (`#E2CBEF`):** Badges informativos, contornos suaves e tags de status.
* **Verde-Limão (`#E2F981`):** Acentos energéticos, botões de ação principal (CTA), upgrades e status ativos.
* **Tipografia:** *Inter* e *Plus Jakarta Sans*.

---

## 💻 5. Funcionalidades Desenvolvidas

* [x] **Landing Page de Alta Conversão:** Hero section com proposta direta, prova social (+10.000 renders), métricas e FAQ.
* [x] **Galeria Interativa Antes/Depois:** Slider arrastável demonstrando a evolução de prints brutos para renders realistas.
* [x] **Autenticação com Free Trial Automático:** Cada novo usuário recebe 3 créditos gratuitos para testar sem necessidade de cartão.
* [x] **Área de Trabalho com Pastas de Projeto:** Organização por clientes e ambientes (*ex: Residência Alphaville, Apartamento 42*).
* [x] **Upload Ágil com `Ctrl+V`:** Suporte a arrastar, selecionar ou colar o print direto da área de transferência.
* [x] **Controles de Iluminação e Ambientação:**
  * Horários: Manhã suave, Tarde ensolarada, Golden hour e Noturno.
  * Toggles independentes: Fitas de LED em móveis e Spots/luminárias acesas.
  * Ambientação automática: Objetos decorativos (livros, vasos, almofadas) e paisagismo leve.
* [x] **Comparador Interativo Antes/Depois:** Slider em tempo real na tela do estúdio.
* [x] **Mini Editor de Pós-Produção (Estilo Photoshop Leve):** Sliders de Brilho, Contraste, Saturação, Temperatura de Cor e Nitidez.
* [x] **Painel Administrativo (`/admin`):** Controle de usuários cadastrados, consumo de renders, métricas globais e botões manuais de ativação de planos anuais.

---

## 📸 6. Evidências da Aplicação (Telas Reais do MVP)

### 🌟 1. Landing Page & Galeria Interativa Antes/Depois
Demonstração do slider interativo comparando a imagem original do projeto com o render gerado pela IA:
<img width="100%" alt="Landing Page e Slider Antes e Depois" src="https://github.com/user-attachments/assets/e2855cea-c485-4fe0-a106-6c2a93d2e5ba" />

---

### 🎨 2. Estúdio de Renderização, Controles de Luz e Iluminação Artificial
Upload com suporte a `Ctrl+V`, seletores de iluminação (Manhã, Tarde, Golden Hour, Noturno), fitas de LED e ambientação inteligente:
<img width="100%" alt="Estúdio de Renderização e Controles" src="https://github.com/user-attachments/assets/de60a03f-243a-4283-b095-3930a8217cbe" />

---

### 🎛️ 3. Pós-Produção Integrada & Exportação
Mini editor de pós-produção com sliders de ajuste fino em tempo real (brilho, contraste, saturação, temperatura e nitidez) e opções de download:
<img width="100%" alt="Pós-Produção e Edição" src="https://github.com/user-attachments/assets/011a6abe-622e-4fef-b90e-c9ac17c09f0b" />

---

## 🤖 7. Mega Prompt / PRD Utilizado

```markdown
# PRD — ore.ia

> **ore.ia**
>
> *o renderizador ia*

---

# Visão Geral

O **ore.ia** é uma plataforma de visualização arquitetônica baseada em IA que transforma imagens de projetos em renders fotorrealistas profissionais em menos de 60 segundos.

O produto foi criado para arquitetos, designers de interiores, estudantes e profissionais da construção que desejam gerar imagens de alta qualidade sem conhecimento técnico em renderização.

O foco da experiência é simplicidade:

- Sem prompts complexos
- Sem configurações difíceis
- Sem softwares pesados

Basta enviar uma imagem do projeto ou colar uma captura de tela e a IA cuida do restante.

---

# Proposta de Valor

## Transforme qualquer imagem do seu projeto em um render profissional em segundos.

- IA especializada em arquitetura
- Renderização em 1 clique
- Ambientação automática
- Iluminação inteligente
- Resultado pronto para apresentação ao cliente

---

# Identidade Visual

## Marca

**ore.ia**

Subtítulo:

**o renderizador ia**

---

## Paleta de Cores

### Preto Grafite

#1D1D1B

Uso:

- Fundo principal
- Sidebar
- Header
- Cards premium

### Branco Gelo

#F9F5EF

Uso:

- Textos principais
- Seções claras
- Contraste visual

### Lilás Claro

#E2CBEF

Uso:

- Badges
- Status
- Bordas suaves
- Elementos secundários

### Verde-Limão

#E2F981

Uso:

- CTA principal
- Upgrade
- Destaques
- Status ativos

---

## Tipografia

- Inter
- Plus Jakarta Sans

Estilo visual:

- Moderno
- Premium
- Minimalista
- Tecnológico

---

# Landing Page

## Hero Section

### Headline

# Seu projeto em render profissional em segundos.

### Subheadline

Transforme imagens simples em renders fotorrealistas prontos para apresentar ao cliente utilizando inteligência artificial especializada em arquitetura.

### CTA Principal

**Testar Grátis — 3 Renders**

### CTA Secundário

**Ver Exemplos**

---

# Galeria Antes e Depois

Slider interativo com exemplos reais.

Categorias:

- Fachadas
- Salas
- Cozinhas
- Quartos
- Banheiros
- Áreas Gourmet

Comparação:

**Imagem Original → Render ore.ia**

---

# Benefícios

## ⚡ Menos de 60 segundos

Sem esperar horas por renderizações tradicionais.

## 🧠 IA especializada em arquitetura

Compreende geometrias, materiais e iluminação automaticamente.

## 🏺 Decoração automática

A IA identifica o ambiente e adiciona elementos coerentes.

## 💡 Iluminação profissional

Aplicação automática de LEDs, spots e luz natural.

## 📈 Mais apresentações, menos trabalho

Aumente a velocidade de aprovação dos projetos.

---

# Prova Social

Exibir métricas:

- +10.000 renders gerados
- +1.500 arquitetos atendidos
- Economia média de 8 horas por projeto

---

# FAQ

Perguntas frequentes sobre:

- Como funciona
- Quanto tempo demora
- Compatibilidade
- Créditos
- Planos

---

# Sistema de Autenticação

## Cadastro

Campos:

- Nome
- E-mail
- Senha
- WhatsApp

---

## Login

Campos:

- E-mail
- Senha

---

# Sistema de Teste Gratuito

Todo usuário recebe automaticamente:

## 3 renders gratuitos

Após cadastro.

---

# Indicador de Créditos

Exibir no Header:

⚡ Renders restantes: X de 3

Quando os créditos acabarem:

Abrir modal de upgrade.

---

# Planos

## Plano Starter

### R$ 297/ano

ou

### 12x de R$ 29,70

### Inclui

- Até 10 renders por dia
- Todos os horários de iluminação
- LEDs
- Spots
- Ambientação automática
- Pastas de projeto
- Histórico de renders

### CTA

Assinar Starter no WhatsApp

---

## Plano Pro

### R$ 497/ano

ou

### 12x de R$ 49,70

### Badge

⭐ Mais Popular

### Benefícios

- Renders ilimitados
- Prioridade na fila
- Exportação em 4K
- Sem marca d'água
- Todas as funcionalidades

### CTA

Assinar Pro Ilimitado

Destaque visual:

- Borda Verde-Limão
- Selo Mais Popular

---

# Upgrade

Usuários Starter podem migrar para Pro.

Botão:

**Fazer Upgrade para Pro**

---

# Dashboard

Após login.

---

# Header

Itens:

- Logo ore.ia
- Créditos disponíveis
- Plano atual
- Upgrade
- Perfil

Logo:

ore.ia

Com ".ia" destacado em Verde-Limão.

---

# Métricas do Usuário

Exibir no Dashboard:

✅ 37 renders gerados

✅ 18 horas economizadas

✅ 5 projetos ativos

Objetivo:

Aumentar retenção e percepção de valor.

---

# Gestão de Projetos

## Botão

+ Nova Pasta de Projeto

---

# Estrutura de Pastas

Exemplos:

- Residência Alphaville
- Apartamento 42
- Casa de Praia
- Escritório Corporativo

---

# Cards de Projeto

Exibir:

- Nome do projeto
- Quantidade de renders
- Última atualização

---

# Compatibilidade de Entrada

O ore.ia aceita qualquer imagem arquitetônica como entrada.

Exemplos:

- Prints do SketchUp
- Exportações do SketchUp
- Imagens do Revit
- Imagens do Archicad
- Capturas de tela de softwares 3D
- Wireframes arquitetônicos
- Estudos volumétricos
- Perspectivas preliminares

A IA interpreta automaticamente a geometria da imagem para gerar um render fotorrealista.

---

# Estúdio de Renderização

Ao abrir um projeto.

---

# Upload de Imagem

O usuário pode fornecer a imagem de três formas.

## 📂 Upload de Arquivo

Formatos aceitos:

- JPG
- PNG
- WEBP

---

## 🖱️ Arrastar e Soltar

Arrastar a imagem diretamente para o estúdio.

---

## 📋 Colar da Área de Transferência

Atalhos:

- Ctrl + V (Windows)
- Cmd + V (Mac)

Ideal para prints recém-capturados.

---

# Preview

Exibir imediatamente a imagem enviada.

---

# Referência Opcional

Upload opcional de imagem inspiracional.

Exemplos:

- Pinterest
- Behance
- Render pronto
- Foto real

Objetivo:

Guiar o estilo visual mantendo a geometria original do projeto.

---

# Tipo de Espaço

## 🏠 Fachada / Externo

## 🛋️ Interno

---

# Horário da Luz

## 🌅 Manhã Suave

Luz natural difusa.

## ☀️ Tarde Ensolarada

Sombras marcadas.

## 🌇 Golden Hour

Tons dourados e mais quentes.

## 🌙 Noturno

Iluminação noturna.

---

# Iluminação Artificial

## 💡 Fitas de LED

Adicionar LEDs em marcenaria.

## 💡 Spots e Pendentes

Adicionar iluminação quente e acolhedora.

---

# Ambientação Inteligente

## 🏺 Objetos Decorativos

Adicionar automaticamente:

- Livros
- Vasos
- Velas
- Almofadas
- Adornos

---

## 🌿 Paisagismo

Adicionar automaticamente:

- Plantas
- Vasos
- Vegetação externa

---

# Renderização

Botão principal:

## Renderizar com ore.ia ✨

Cor:

- Fundo Verde-Limão
- Texto Preto Grafite

---

# Regras de Consumo

## Plano Gratuito

- 3 renders totais
- Consome 1 crédito por render

## Plano Starter

- Até 10 renders por dia

## Plano Pro

- Renderizações ilimitadas

---

# Feedback de Processamento

Exibir progresso em tempo real.

✅ Geometria analisada

✅ Materiais identificados

✅ Ambientação aplicada

✅ LEDs configurados

✅ Iluminação finalizada

✅ Render concluído

Exibir também:

Tempo estimado restante: XX segundos

---

# Comparação Antes e Depois

Slider interativo.

## Lado Esquerdo

Imagem Original

## Lado Direito

Render Gerado

---

# Histórico de Versões

Cada render gerado cria uma nova versão.

Exemplo:

v1 - Golden Hour

v2 - Noturno

v3 - LEDs Ativados

v4 - Paisagismo

v5 - Referência Externa

Permitir restaurar qualquer versão.

---

# Pós-Produção

Mini editor integrado.

---

# Ajustes Disponíveis

- Brilho
- Contraste
- Saturação
- Temperatura de Cor
- Nitidez

Atualização em tempo real.

---

# Salvamento

Botão:

💾 Salvar na Pasta

---

# Exportação

Formatos:

- PNG
- JPG

---

# Recursos Pro

- Exportação 4K
- Sem marca d'água

---

# Ações

⬇️ Baixar Render

⬇️ Baixar Antes e Depois

---

# Modal de Limite Atingido

Quando os créditos acabarem.

## Título

Você utilizou todos os seus renders disponíveis.

## Mensagem

Continue renderizando assinando um dos planos anuais.

## Botões

- Assinar Starter
- Assinar Pro

Redirecionamento:

WhatsApp.

---

# Painel Administrativo

## URL

/admin

---

# Gestão de Usuários

Tabela contendo:

- Data de Cadastro
- Nome
- E-mail
- WhatsApp
- Plano Atual
- Renders Utilizados
- Status

---

# Planos Disponíveis

- Gratuito (3 Testes)
- Starter
- Pro

---

# Status

- Ativo
- Aguardando Pagamento
- Expirado

---

# Ações Administrativas

- Ativar Starter
- Ativar Pro
- Alterar Plano
- Resetar Créditos
- Bloquear Usuário

---

# Dashboard Administrativo

Cards de KPIs:

## Total de Usuários

## Usuários Gratuitos

## Assinantes Starter

## Assinantes Pro

## Faturamento Anual

## Total de Renders Gerados

---

# Diferenciais Competitivos

## ✅ IA especializada em arquitetura

Treinada para compreender ambientes internos e externos.

## ✅ Não exige prompts complexos

O usuário apenas envia a imagem.

## ✅ Decoração automática contextual

A IA entende o ambiente e adiciona decoração coerente.

## ✅ Iluminação profissional automática

LEDs, spots e iluminação natural gerados automaticamente.

## ✅ Fluxo em menos de 60 segundos

Pensado para apresentações rápidas ao cliente.

---

# Posicionamento da Marca

O ore.ia não deve ser apresentado apenas como um gerador de renders.

## Posicionamento Oficial

> A primeira plataforma de visualização arquitetônica com IA focada em transformar imagens de projetos em apresentações visuais prontas para clientes em menos de 60 segundos.

---

# Visão de Futuro

O posicionamento deve permitir evolução para:

- Vídeos gerados por IA
- Passeios virtuais
- Reformas virtuais
- Troca inteligente de materiais
- Visualização arquitetônica avançada
- Apresentações automáticas para clientes
- Animações de projeto
- Geração de múltiplas versões visuais

Sem limitar a marca apenas à criação de imagens.
```

---


## 🛠️ Tecnologias Utilizadas

* **[Lovable.dev](https://lovable.dev)** (Desenvolvimento com IA)

---

## 👩‍💻 Autoria


Desenvolvido por **Letícia Sousa** como entrega do Desafio de Código da [Digital Innovation One (DIO)](https://web.dio.me/).
