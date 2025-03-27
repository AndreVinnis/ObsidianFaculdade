Define a organização do sistema, padrões de desenvolvimento e tecnologias utilizadas. Garantindo que o software seja escalável, manutenível e eficiente.

# Arquiteturas

## Cliente-Servidor
Modelo em que um cliente solicita serviços a um servidor central

**Vantagens:**
- Centralização de controle
- Facilidade de manuteção

**Desvantages:**
- Pode gerar sobrecarga no servidor, possui ponto único de falha

## Arquitetura em camadas
Divide o sistema em camadas (apresentação, controle, lógica, dados)

**Vantagens:**
- Modularidade
- Facilidade de manutenção

**Desvantages:**
- Pode adicionar complexidade e latência

## Publisher-Subscriber
Comunicação baseada em eventos, em que o publisher envia mensagens aos subscribers

**Vantagens:**
- Desacoplamento 
- Escabalabilidade

**Desvantagens:**
- Difícil de depurar e garantir consistência

## Plugins
Permite extensão da funcionalidade de um sistema por meio de módulos externos (plugins)

**Vantagens:**
- Flexibilidade
- Modularidade

**Desvantagens:**
- Pode ser difícil gerenciar dependências e compartibilidade

## Monolítica
Todo o sistema é construído como uma única unidade

**Vantagens:**
- Simples de desenvolver e implantar

**Desvantagens:**
- Difícil de escalar e manter à medida que cresce

## Microserviços
Divide o sistema em pequenos serviços independentes, que se comunicam via APIs

**Vantegens:**
- Escalabilidade
- Deploy independentes

**Desvantagens:**
- Complexidade em comunicação e gerenciamento 

## SOA (Service-Driented Architeture)
Modelo baseado em integração de serviços reutilizáveis; diferentes sistemas ser comunicam por se comunicam por interfaces bem definidas

## Hexagonal
Separa regras de negõcio da infraestrutura e interfaces externas

**Vantagens:**
- Alta testabilidade
- Desacoplamento

**Desvantagens:**
- Curva de aprendizado. Pode ser difícil de implantar