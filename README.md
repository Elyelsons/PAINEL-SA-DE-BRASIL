
# Painel Saúde Brasil - Documentação

## Visão Geral

O Painel Saúde Brasil é uma plataforma interativa de visualização de dados da saúde pública brasileira. O projeto foi desenvolvido com o objetivo de promover transparência e facilitar o acesso à informação sobre o sistema de saúde no Brasil, disponibilizando métricas importantes como ocupação de leitos, cobertura vacinal e indicadores de saúde por região.

## Estrutura do Projeto

O projeto é dividido em dois componentes principais:

1. **Landing Page** - Página inicial que apresenta o projeto e seus objetivos
2. **Dashboard** - Interface interativa para visualização dos dados de saúde

### Tecnologias Utilizadas

- React
- TypeScript
- Tailwind CSS
- shadcn/ui (componentes de UI)
- Recharts (biblioteca de visualização de dados)
- React Router (navegação)
- Lucide React (ícones)

## Páginas Principais

### Landing Page

A landing page foi projetada para apresentar o projeto de forma clara e atrativa, destacando:

- Propósito do projeto
- Principais estatísticas
- Funcionalidades do dashboard
- Informações sobre as fontes de dados
- Call-to-action para acessar o dashboard completo

### Dashboard

O dashboard apresenta visualizações interativas dos dados de saúde, incluindo:

- Métricas principais (leitos SUS, vacinação, atendimentos)
- Dados regionais de saúde (filtráveis por região)
- Gráficos de cobertura vacinal por estado
- Indicadores de saúde (ocupação de leitos UTI, enfermaria, profissionais ativos)
- Capacidade hospitalar por região

## Componentes

### Componentes de Dashboard

#### RegionalData
Exibe dados tabulares sobre diferentes regiões do Brasil, incluindo casos, óbitos e taxas de incidência/mortalidade. Permite filtrar por região.

#### VaccinationChart
Apresenta gráficos de barras mostrando a cobertura vacinal por estado, separando por primeira dose, segunda dose e dose de reforço.

#### HealthMetrics
Exibe indicadores de saúde críticos como disponibilidade de leitos UTI, leitos de enfermaria e dados sobre profissionais ativos, com indicações visuais de tendências.

#### HospitalCapacity
Mostra a capacidade hospitalar por região do país, com indicadores de status (crítico, alto, médio, baixo) e dados sobre quantidade de leitos.

## Fontes de Dados

Os dados apresentados na plataforma são provenientes de:

- DATASUS / TABNET
- Brasil.IO
- OpenDataSUS
- Ministério da Saúde

## Como Executar o Projeto

### Requisitos

- Node.js & npm (versão recomendada: Node.js 18+ e npm 9+)

### Instalação

```sh
# Clonar o repositório
git clone <URL_DO_REPOSITÓRIO>

# Navegar até a pasta do projeto
cd painel-saude-brasil

# Instalar dependências
npm install

# Iniciar o servidor de desenvolvimento
npm run dev
```

## Desenvolvimento

### Estrutura de Arquivos

```
src/
  ├── components/         # Componentes reutilizáveis
  │   ├── ui/             # Componentes de interface do shadcn/ui
  │   └── dashboard/      # Componentes específicos do dashboard
  ├── hooks/              # Hooks React personalizados
  ├── lib/                # Funções utilitárias 
  ├── pages/              # Páginas principais da aplicação
  │   ├── Index.tsx       # Landing page
  │   └── Dashboard.tsx   # Dashboard interativo
  └── main.tsx           # Ponto de entrada da aplicação
```

### Contribuições

Para contribuir com o projeto:

1. Faça um fork do repositório
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Faça commit das suas alterações (`git commit -m 'Adiciona nova feature'`)
4. Envie para o branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

## Funcionalidades Planejadas

- Integração com dados em tempo real do DATASUS
- Filtros avançados por período e mais indicadores
- Comparativo histórico de dados
- Exportação de relatórios personalizados
- Visualização por mapa geográfico do Brasil

## Público-Alvo

- Secretarias de Saúde
- Profissionais de Saúde
- ONGs e Pesquisadores
- Cidadãos e Jornalistas

---

© 2025 Painel Saúde Brasil
