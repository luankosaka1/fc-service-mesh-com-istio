# Service Mesh com Istio

## Introdução

Service Mesh: malha de serviço

Permite monitorar e gerenciar a comunicação entre os serviços

Istio, permite rodar em cima do Kubernetes

### O Mundo Distribuído

No mundo distribuído temos diversos microserviços que se comunicam e são dependentes uma das outras, com isso precisamos garantir que todos estejam saudáveis para que não comprometa a comunicação.

![O mundo distribuído](https://github.com/luankosaka1/fullcycle-service-mesh-com-istio/blob/main/images/o-mundo-distribuido.png)

### Service Mesh vs Istio

#### Service Mesh

É uma camada extra adiciionada junto ao seu cluster visando monitorar e modificar em tempo real o tráfego das aplicações.

#### Istio

É um projeto open-source que imploementa service mesh visando diminuir a complexidade no gerenciamento de aplicações distribuídas idependente de qual linguagem ou tecnologia as elas foram desenvolvidas.

- Kubernetes
- Apache MESOS
- Consul
- HashiCorp Noad

### Principais Recursos

### Por que preciso de um Service Mesh? Istio?

- Gerenciamento de tráfego
-- Gateways (entrada: ingress traffic e saída: egress traffic)
-- Load Balacing
-- Timeout
-- Políticas de retry
-- Circuit Breaker(quantas requisições pode suportar)
-- Fault Injection (simular o comportamento do sistema)
- Observabilidade
-- Métricas
-- Traces distribuídos
-- Logs
- Segurança
-- Man-in-the-middle (interceptar a comunicação e capturar dados sensíveis)
-- mTLS
-- AAA (authentication, authorization e audit)

## Arquitetura do Istio

### Dinâmica && Sidecar Proxy

![Sidecar-proxy](https://github.com/luankosaka1/fullcycle-service-mesh-com-istio/blob/main/images/sidecar-proxy.png)

### Arquitetura

![Arquitetura](https://github.com/luankosaka1/fullcycle-service-mesh-com-istio/blob/main/images/arquitetura.png)

### Istiod

- Pilot: Controla as configurações
- Citadel: Controla a autenticação e  identidade
- Gallery: Faz a tradução do que vc esta fazendo a configuração na linguagem do istio (istio é utilizado em outras plataformas)

### Moniitoramento em tempo real

![Kiali](https://github.com/luankosaka1/fullcycle-service-mesh-com-istio/blob/main/images/kiali.png)