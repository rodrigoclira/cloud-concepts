
---

## Elastic Cloud Computing (EC2) 

O **Amazon EC2** é o serviço de computação virtual da AWS. Ele permite provisionar instâncias (servidores virtuais) com diferentes combinações de CPU, memória, armazenamento e capacidade de rede, de acordo com a demanda da aplicação.

As instâncias EC2 são configuradas a partir de **AMIs** (Amazon Machine Images), que definem o sistema operacional e o software base. O serviço suporta múltiplos modelos de precificação: On-Demand, Reserved Instances e Spot Instances, permitindo otimização de custo conforme o padrão de uso.

### Security Group
Um **Security Group** funciona como um firewall virtual associado a instâncias EC2. Ele controla o tráfego de entrada (*inbound*) e saída (*outbound*) com base em regras definidas por protocolo, porta e origem/destino (CIDR ou outro Security Group).

Security Groups são **stateful**: se uma requisição de entrada é permitida, a resposta correspondente é automaticamente permitida, independentemente das regras de saída. Por padrão, todo tráfego de entrada é bloqueado e todo tráfego de saída é permitido.

### Elastic IP 

Um **Elastic IP** é um endereço IPv4 estático e público alocado para uso em uma conta AWS. Por padrão, instâncias EC2 recebem IPs públicos dinâmicos que mudam a cada reinicialização. O Elastic IP resolve esse problema ao fornecer um endereço fixo que pode ser associado e reassociado a instâncias ou interfaces de rede conforme necessário.

É importante notar que a AWS cobra pelo Elastic IP quando ele está alocado mas **não associado** a uma instância em execução, incentivando o uso eficiente do recurso.
