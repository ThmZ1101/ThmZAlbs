Eventos: Projeto POPSTARSHOW

__Objetivo do Projeto:__

- O objetivo do POSTARSHOW é desenvolver um aplicativo web eficiente e seguro para que os clientes da Multishows possam gerenciar suas compras de ingressos para o evento POPSTARSHOW, oferecendo uma experiência intuitiva e fluida, utilizando tecnologias modernas que garantem a segurança e escalabilidade necessárias para o evento de grande porte.

# Funcionalidades Principais:

__Autenticação e Autorização:__

- Registro de Usuário: Precisamos implementar um sistema de registro que permita aos novos usuários se inscreverem com nome de usuário, e-mail e senha.
- Login: Deve haver um sistema de login seguro para que os usuários possam acessar áreas restritas da aplicação.
- JWT: Usaremos JWT para gerenciar sessões de usuário e proteger rotas que exigem autenticação.


__Objetivos SMART:__

1. Específico
Criar um aplicativo web to-do-list que permita aos usuários visualizar e adquirir ingressos para o POPSTARSHOW, integrando funcionalidades de gerenciamento de compras, autenticação segura com JWT, e processamento ágil de dados utilizando React, Node.js e MongoDB.

2. Mensurável 
Garantir que o aplicativo suporte a aquisição de 50.000 ingressos em até 30 minutos após o lançamento, e atenda a pelo menos 10.000 usuários simultâneos, com feedback positivo de pelo menos 85% dos usuários durante o evento.

3. Atingível 
Implementar um sistema robusto de autenticação JWT e proteção de dados, além de garantir uma arquitetura escalável com Node.js e MongoDB, em um cronograma de 3 meses, com lançamento da versão funcional em 30 dias antes do evento.

4. Relevante
O POSTARSHOW é crucial para garantir a experiência fluida e segura dos usuários na compra de ingressos do POPSTARSHOW, um dos maiores eventos musicais do mundo, oferecendo uma plataforma tecnológica de ponta que suporte a alta demanda com rapidez e segurança.

5. Temporal
Lançar o aplicativo em 3 meses, com testes de carga e segurança realizados nas últimas 4 semanas antes do evento, garantindo a disponibilidade total da plataforma 30 dias antes do início da venda dos ingressos.

# Cronograma do Projeto:

Mês 1: Planejamento e Desenvolvimento Inicial

Semana 1-2: Definição detalhada dos requisitos e fluxos de usuários.
Configuração inicial do ambiente de desenvolvimento (Node.js, MongoDB, Express, React).
Criação do sistema de autenticação e autorização com JWT.

Semana 3-4:

Implementação do registro e login de usuários.
Criação da interface do usuário com React (Componentes de Login, Registro).
Configuração do banco de dados MongoDB e integração com Node.js (modelo de usuário).

Mês 2: Funcionalidades Principais e Integração

Semana 1-2:

Implementação das rotas protegidas por JWT (para gerenciar compras).
Desenvolver o fluxo de compra de ingressos (API para gerenciamento de ingressos).
Integração de front-end (React) com back-end (Node.js/Express).

Semana 3-4:

Implementação do carrinho de compras e histórico de pedidos.
Otimização da escalabilidade e performance do servidor (Node.js e MongoDB).
Testes unitários e de integração das principais funcionalidades.

Mês 3: Testes e Preparação para Lançamento

Semana 1-2:

Realização de testes de carga (para garantir suporte a 10.000 usuários simultâneos).
Testes de segurança (incluindo ataques comuns, como CSRF e XSS).
Implementação de melhorias de interface com base no feedback inicial.

Semana 3-4:

Otimização final e correção de bugs.
Testes finais de carga, segurança e usabilidade.
Lançamento da versão de teste para validação de usuários.

Semana 4:

Preparação para o lançamento oficial (deploy em ambiente de produção).
Monitoramento inicial e suporte durante o período de vendas.


# Análise de Erros Potenciais:


Problema: Latência Alta ou Lentidão Durante o Pico de Usuários

Causa: Falta de otimização no banco de dados ou no servidor.
Solução: Utilizar índices adequados no MongoDB, caching de dados com Redis ou outro mecanismo, e balanceamento de carga com serviços como Nginx.
Problema: Falhas na Autenticação JWT

Causa: Erros de configuração no middleware ou gerenciamento incorreto de tokens.
Solução: Garantir que os tokens JWT estejam sendo corretamente gerados e verificados, implementar um sistema de refresh tokens para sessões prolongadas.
Problema: Erro ao Processar Alto Volume de Pedidos

Causa: Conexões simultâneas e sobrecarga do servidor.
Solução: Implementar uma arquitetura baseada em microsserviços ou filas de mensagens para distribuição de carga (RabbitMQ ou Kafka).


# Recursos Tecnológicos

1. Node.js: Servidor back-end com escalabilidade, usando a biblioteca jsonwebtoken para JWT.

2. Express: Framework leve e flexível para criação de APIs REST.

3. MongoDB: Banco de dados NoSQL para armazenamento de usuários, ingressos e transações, focado em escalabilidade e flexibilidade.

4. React: Biblioteca front-end para criar uma interface de usuário dinâmica e intuitiva.

5. JWT (JSON Web Tokens): Para gerenciamento de sessões seguras, garantindo que apenas usuários autenticados possam acessar áreas protegidas da aplicação.

# Diagramas Usuario:

__Uso:__

![DiagramaDeUso](diagramas/diagrama-uso.png)

__Classe:__

![DiagramaDeClasse](diagramas/diagrama-classe.png)

__Fluxo:__

![DiagramaDeFluxo](diagramas/diagrama-fluxo.png)

# Diagramas ADM

![DiagramaDeUso](diagramas/diagrama-uso.png)

__Classe:__

![DiagramaDeClasse](diagramas/diagrama-classe.png)

__Fluxo:__

![DiagramaDeFluxo](diagramas/diagrama-fluxo.png)

__Prototipagem:__

https://www.figma.com/design/oeaZJAuyEQ6VDR5qSErb0c/Untitled?node-id=0-1&t=TesPjHiOBj0jRTGu-1