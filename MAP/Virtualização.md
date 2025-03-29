# Cloud Computing (Computação em nuvem)

É um modelo de entrega de recursos computacionais (como servidores, armazenamento, banco de dados, redes e software) pela internet, sob demanda. Em vez de manter infraestruturas própria, os usuários podem acessar esses recursos de provedores de nuvem.

## Principais características  

- **Serviço sob demanda:** Os usuários podem acessar e configurar recursos computacionais automaticamente, sem intervenção manual do provedor.
- **Acesso remoto e ubiquidade:** Os serviços podem ser acessados de qualquer lugar, a qualquer momento, desde que haja conexão com a internet.
- **Elasticidade:** Refere-se à capacidade de aumentar ou reduzir automaticamente os recursos computacionais, em tempo real, conforme a demanda. *Ajuste dinâmico e temporário dos recursos.* 
- **Escalabilidade:** Refere-se à capacidade de expandir permanentemente os recursos para suportar um crescimento contínuo. Pode ser vertical (melhoria do hardware, como mais RAM ou CPU) ou horizontal (adição de mais servidores). *Expansão contínua e planejada da capacidade.* 
- **Pagamento baseado no uso (Pay-as-you-go):** Os usuários pagam apenas pelos usos consumidos, reduzindo desperdícios e otimizando investimentos.
- **Multitenancy (Compartilhamento de recursos):** Os provedores de nuvem utilizam um modelo de multiusuários, onde vários clientes utilizam compartilham a mesma infraestrutura física de forma isolada e segura.

## Modelos de serviços
Um modelo de serviço define como os recursos de computação são fornecidos na nuvem.  Cada modelo oferece um nível diferente de controle, flexibilidade e responsabilidade para o usuário.

### SaaS (Software as a Service):
Fornece software pronto para uso diretamente pela internet, sem necessidade de instalação ou manutenção do usuário.
Exemplo: Google Drive, Microsoft 365.

**Quem gerencia o quê?**
- O provedor gerencia tudo (infraestrutura, plataforma e software).
- O usuário apenas usa o serviço.

### PaaS (Platform as a Service):
Oferece uma plataforma pronta para desenvolvimento e hospedagem de aplicativos. O usuários não precisa se preocupar com infraestruturas subjacentes.
Exemplo: Heroku, Google App Engine.

**Quem gerencia o quê?**
- O provedor gerencia infraestrutura, o sistema operacional e o ambiente de execução.
- O usuário gerencia o código e as configurações do aplicativo.

### IaaS (Infrastructure as a Service):
Fornece infraestrutura virtualizada, como servidores, armazenamento, redes e sistemas operacionais. O usuário gerencia a configuração e instalação dos softwares.
Exemplo: Amazon EC2 (AWS), Microsoft Azure Virtual Machines.

**Quem gerencia o quê?**
- O provedor gerencia hardware, rede e virtualização. 
- O usuário gerencia sistema operacional, aplicativos e configurações.

### HaaS (Hardware as a Service):
Permite que empresas aluguem hardware físicos (servidores, roteadores, equipamentos de TI) em vez de comprá-los.
Exemplo: Dell APEX, HP Device as a Service (DaaS).

**Quem gerencia o quê?**
- O provedor gerencia a manutenção do hardware.
- O usuário usa os dispositivos conforme contratado.

### XaaS (Everything as a Service):
É um termo genérico que engloba qualquer serviço oferecido via nuvem, além de IaaS, PaaS e SaaS.
Exemplo: (DaaS) - Computadores virtuais remotos, (BaaS) - Infraestrutura para aplicativos móveis e web.

**Quem gerencia o quê?**
- O provedor gerencia infraestrutura e os serviços específicos do modelo.
- O usuário acessa e usa o serviço conforme necessidade.

### Resumo: Diferenças entre modelos

| Modelo | O que oferece?                                      | Quem gerencia?                          |
| ------ | --------------------------------------------------- | --------------------------------------- |
| SaaS   | Software pronto para uso                            | Usuário apenas usa o software           |
| PaaS   | Plataforma pronta para desenvolvimento              | Usuário gerencia código e apps          |
| IaaS   | Infraestrutura virtualizada (Servidores, redes, SO) | Usuário gerencia o SO e apps            |
| HaaS   | Hardware físico alugado                             | Usuário usu o hardware, provedor mantém |
| XaaS   | Qualquer serviço entregue via nuvem                 | Depende do tipo de serviço              |

## Modelos de implantação 
Os modelos de implantação determinam como e onde a infraestrutura da nuvem é hospedada e gerenciada. 

### Nuvem pública:
É um ambiente de nuvem compartilhamento entre vários usuários, gerenciada por um provedor de serviços terceirizado.
Exemplo: Amazon Web Services (AWS), Microsoft Azure

**Vantagens:**
- Baixo custo: Sem necessidade de comprar hardware.
- Alta escalabilidade: Recursos ajustados conforme a demanda.
- Manutenção gerenciada pelo provedor.
**Desvantagens:**
- Menor controle sobre segurança e personalização.
- Pode ter latência dependendo da rede.

Exemplo de uso: Hospedagem de sites, serviços de armazenamento como Google Drive e Dropbox, e aplicativos SaaS como Gmail e Microsoft 365.

### Nuvem privada:
Infraestrutura dedicada exclusivamente para uma empresa ou organização, podendo ser hospedada no local *(on-premises)* ou por um provedor.

**Vantagens:**
- Maior controle sobre segurança e dados.
- Melhor desempenho para aplicações críticas.
- Atende a requisitos regulatórios e compliance.
**Desvantagens:**
Alto custo de implementação e manutenção.
Escalabilidade limitada comparada à nuvem pública.

Exemplo de uso: Bancos, governos e grandes corporações que precisam de segurança e controle total sobre seus dados.

### Nuvem híbrida:
Combina a nuvem pública e privada, permitindo que dados e aplicações sejam compartilhadas entre elas.

**Vantagens:**
- Equilíbrio custo e desempenho.
- Permite que dados sensíveis fiquem na nuvem privada e aplicações menos críticas na pública.
- Flexibilidade parra escalar conforme necessário.
**Desvantagens:**
- Gerenciamento mais complexo.
- Integração entre ambientes pode ser desafiadora.

Exemplo de uso: Uma empresa pode armazenar dados sensíveis (como registros financeiros) na nuvem privada e rodar um site público na nuvem pública.

### Nuvem comunitária:
Infraestrutura compartilhada entre várias organizações com interesses comuns. (Hospitais, universidades, órgãos governamentais).

**Vantagens:**
- Custo reduzido ao ser compartilhado entre várias organizações.
- Foco em compliance e requisitos específicos do setor.
- Segurança aprimorada para setores críticos.
**Desvantagens:**
- Pode não ter a mesma escalabilidade da nuvem pública.
- Menos flexibilidade que a nuvem privada para personalizações específicas.

Exemplo de uso: Hospitais compartilhando uma nuvem comunitária para armazenar registros médicos de forma segura e regulamentada.

### Resumo: Comparação dos Modelos de Implantação


| Modelo            | Quem gerencia?        | Escalabilidade | Segurança | Custo         | Uso típico                                        |
| ----------------- | --------------------- | -------------- | --------- | ------------- | ------------------------------------------------- |
| Nuvem pública     | Provedor              | Alta           | Média     | Baixo         | Aplicações gerais e SaaS                          |
| Nuvem privada     | Empresa               | Média          | Alta      | Alto          | Empresas com requisitos de segurança rigorosos    |
| Nuvem híbrida     | Empresa + provedor    | Alta           | Altra     | Médio         | Empresas que precisam equilibrar custo e controle |
| Nuvem comunitária | Grupo de organizações | Média          | Alta      | Compartilhado | Setores regulados (saúde, governo, pesquisas)     |

# Virtualização e Emulação

## Virtualização:
Virtualização é a tecnologia que permite criar *versões virtuais de recursos computacionais*, como sistemas operacionais, servidores, armazenamento e redes. Isso é feito por meio de um software chamado Hipervesor, que separa o hardware físico dos sistemas operacionais, permitindo que várias máquinas virtuais (VMs) rodem de forma independente em um mesmo hardware.

## Emulação:
A emulação é um processo que permite que um sistema *imite outro sistema*, possibilitando a execução de software em um hardware ou sistema diferente do original. A emulação cria um ambiente que simula completamente o hardware e o software do sistema original. Como a emulação precisa converter instruções de um sistema para outro, *pode ser mais lenta* que a execução nativa. 

## Virtualização X Emulação

**Virtualização:**
- Cria máquinas virtuais (VMs) dentro de um hardware físico.
- Usa o mesmo conjunto de instruções do hardware subjacente.
- Mais rápido e eficiente, pois executa diretamente no processador.
- Exemplos: VMware, VirtualBox, KVM, Hyper-V.
**Emulação:**
- Simula completamente um hardware diferente.
- Converte instruções de um sistema para outro, o que pode ser mais lento.
- Permite rodar software de um arquitetura diferente (exemplo: rodar software de Windows no macOS).
- Exemplos: Dolphin, PCSX2, Wine, Rosetta 2.

## Resumo das diferenças:

| Caracteristica          | Virtualização                            | Emulação                                             |
| ----------------------- | ---------------------------------------- | ---------------------------------------------------- |
| Objetivo                | Criar máquinas virtuais                  | Imitar um hardware/sistema diferente                 |
| Desempenho              | Alto (quase nativo)                      | Mais lento devido à conversão de instruções          |
| Dependência de hardware | Sim (usa o mesmo conjunto de instruções) | Não (pode rodar software de arquiteturas diferentes) |
| Exemplos                | VMware, VirtualBox, Hyper-V              | Dolphin, Wine, PCSX2, Rosetta 2                      |
