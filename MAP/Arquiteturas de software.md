Define a organização do sistema, padrões de desenvolvimento e tecnologias utilizadas. Garantindo que o software seja escalável, manutenível e eficiente.

# Arquiteturas

## Cliente-Servidor
Modelo em que um cliente solicita serviços a um servidor central

**Vantagens:**
- Centralização de controle
- Facilidade de manutenção

**Desvantagens:**
- Pode gerar sobrecarga no servidor, possui ponto único de falha

## Arquitetura em camadas
Divide o sistema em camadas (apresentação, controle, lógica, dados)

**Vantagens:**
- Modularidade 
- Facilidade de manutenção

**Desvantagens:**
- Pode adicionar complexidade e latência

## Publisher-Subscriber
Comunicação baseada em eventos, em que o publisher envia mensagens aos subscribers

**Vantagens:**
- Desacoplamento 
- Escalabilidade

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

**Vantagens:**
- Escalabilidade
- Deploy independentes 

**Desvantagens:**
- Complexidade em comunicação e gerenciamento 

## SOA (Service-Oriented Architeture)
Modelo baseado em integração de serviços reutilizáveis; diferentes sistemas se comunicam por interfaces bem definidas

## Hexagonal
Separa regras de negócio da infraestrutura e interfaces externas

**Vantagens:**
- Alta testabilidade
- Desacoplamento

**Desvantagens:**
- Curva de aprendizado. Pode ser difícil de implantar
## Resumo:

| Arquitetura      | Principais características                      | Vantagens                         | Desvantagens                    |
| ---------------- | ----------------------------------------------- | --------------------------------- | ------------------------------- |
| Cliente-servidor | Cliente faz requisições ao servidor             | Simples e centralizado            | Pode gerar gargalo              |
| Camadas          | Divisão lógica do sistema                       | Modular e organizado              | Pode ter sobrecarga de chamadas |
| Pub/Sub          | Comunicação assíncrona entre componentes        | Desacoplado e escalável           | Complexo de gerenciar           |
| Plugins          | Módulos que podem ser adicionados dinamicamente | Flexível e extensível             | Problemas de compartibilidade   |
| Monolítica       | Sistema único e integrado                       | Fácil desenvolvimento inical      | Difícil de escalar              |
| Microserviçõs    | Serviços independentes                          | Escalável e modular               | Complexidade operacional        |
| SOA              | Serviços reutilizáveis em diferentes sistemas   | Reutilização e interoperabilidade | Pode exigir um barramento (ESB) |
| Hexagol          | Núcleo isolado da infraestrutura                | Flexibilidade e desacomplamentp   | Complexidade na implementação   |

## Conceitos:
- **Modularidade:** Característica de sistema que permite ser dividido e módulos independentes, facilitando manutenção, reuso, escalabilidade.
- **Deploy:** Processo de disponibilizar um aplicação em um ambiente de produção.
- **Latência:** Tempo de espera entre a solicitação de uma ação e resposta.
- **Overhead:** Custo extra em processamento, memória ou tempo causado por um sistema ou método.
- **Depurar (Debugging):**  Processo de identificar e corrigir erros em um sistema ou código.