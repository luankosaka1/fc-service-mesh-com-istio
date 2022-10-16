# Service Mesh com Istio

## Introdução

Service Mesh: malha de serviço

Permite monitorar e gerenciar a comunicação entre os serviços

Istio, permite rodar em cima do Kubernetes

## O Mundo Distribuído

No mundo distribuído temos diversos microserviços que se comunicam e são dependentes uma das outras, com isso precisamos garantir que todos estejam saudáveis para que não comprometa a comunicação.

![O mundo distribuído](https://github.com/luankosaka1/fullcycle-service-mesh-com-istio/blob/main/images/o-mundo-distribuido.png)

## Service Mesh vs Isti

### Service Mesh

É uma camada extra adiciionada junto ao seu cluster visando monitorar e modificar em tempo real o tráfego das aplicações.

### Istio

É um projeto open-source que imploementa service mesh visando diminuir a complexidade no gerenciamento de aplicações distribuídas idependente de qual linguagem ou tecnologia as elas foram desenvolvidas.

- Kubernetes
- Apache MESOS
- Consul
- HashiCorp Noad