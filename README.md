## Síntese: Computação em Nuvem

Computação em nuvem é o modelo de fornecimento de recursos e serviços de computação (como armazenamento, processamento, bancos de dados, redes e software) por meio da internet, sob demanda. Empresas provedoras mantêm grandes datacenters com infraestrutura robusta, permitindo que outras empresas ou usuários acessem esses recursos sem precisar investir em equipamentos físicos próprios. Isso reduz custos iniciais e aumenta a flexibilidade e escalabilidade do uso de TI.

---

### Modelos de Implantação

* **On-Premises (Local):** Toda a infraestrutura de TI é mantida internamente pela empresa, incluindo servidores, redes e sistemas, o que implica em maiores custos de aquisição, manutenção e equipe especializada.
* **Nuvem Pública:** A infraestrutura é mantida por um provedor (como AWS, Azure ou GCP) e compartilhada entre múltiplos clientes. A empresa cliente paga apenas pelos recursos utilizados.
* **Nuvem Privada:** A infraestrutura é dedicada a uma única organização, podendo estar localizada no datacenter da empresa ou hospedada por terceiros. Garante maior controle e segurança.
* **Nuvem Híbrida:** Combinação de nuvem pública e privada, permitindo a integração entre ambientes, de acordo com as necessidades de negócio e segurança.

---

### Tipos de Despesas

* **CapEx (Capital Expenditure):** Investimento em bens de capital, como servidores, licenças e infraestrutura física. É mais comum no modelo **On-Premises**.
* **OpEx (Operational Expenditure):** Despesas operacionais contínuas, como assinatura de serviços em nuvem. É predominante no modelo **em nuvem**, com custos mais previsíveis e escaláveis.

---

### Modelos de Serviço

* **IaaS (Infrastructure as a Service):** Fornecimento de infraestrutura básica (máquinas virtuais, redes, armazenamento). O cliente gerencia os sistemas operacionais, aplicativos e dados.
  Ex: Amazon EC2, Azure VM, Google Compute Engine.

* **PaaS (Platform as a Service):** Provedor oferece um ambiente completo para desenvolvimento, teste e implantação de aplicações, sem que o cliente precise gerenciar a infraestrutura subjacente.
  Ex: Google App Engine, Azure App Services, Heroku.

* **SaaS (Software as a Service):** Aplicações prontas para uso, acessadas via navegador, sem necessidade de instalação ou manutenção local.
  Ex: Microsoft 365, Google Docs, Canva.

* **FaaS (Function as a Service – opcional):** Execução de funções sob demanda, ideal para tarefas event-driven, escalando automaticamente conforme a necessidade.
  Ex: AWS Lambda, Azure Functions.

---

### Serviços Comuns (geralmente IaaS ou PaaS)

* Armazenamento de dados
* Máquinas virtuais
* Serviços de DNS
* Containers e orquestração (ex: Kubernetes)
* Bancos de dados (relacionais e não-relacionais)
* Hospedagem de aplicações e servidores
* Execução de scripts e automações

---

### Características dos Serviços de Nuvem

* **Escalabilidade:** Capacidade de aumentar os recursos conforme o crescimento da demanda de forma permanente.
* **Elasticidade:** Capacidade de ajustar os recursos dinamicamente durante picos ou quedas de uso.
* **Segurança:** Os provedores oferecem mecanismos de proteção (criptografia, autenticação, backups), mas a segurança final depende da configuração e uso correto pelo cliente (**modelo de responsabilidade compartilhada**).
* **Alta disponibilidade:** Os serviços são projetados para funcionar continuamente com o mínimo de interrupções, com SLAs definidos em contrato.
* **Gerenciamento:** Ferramentas integradas permitem monitorar, configurar, escalar e controlar os recursos utilizados, muitas vezes com interfaces amigáveis ou APIs.

---

### Regiões e Zonas de Disponibilidade

* **Regiões:** Conjuntos de data centers localizados em áreas geográficas distintas (ex: Brasil, EUA, Europa), permitindo atender a requisitos de latência, conformidade e soberania de dados.
* **Zonas de Disponibilidade (AZ - Availability Zones):** São data centers independentes, mas interconectados dentro de uma mesma região. Garantem redundância e alta disponibilidade. Uma aplicação resiliente pode ser distribuída entre múltiplas zonas.

---

### Assinaturas e Acesso

* As assinaturas são utilizadas para segmentar e organizar o uso dos serviços dentro de uma conta. Elas controlam:

  * Limites de uso
  * Faturamento
  * Permissões e controle de acesso (via funções e grupos de usuários)
  * Organização por projetos, departamentos ou ambientes (ex: produção, teste, desenvolvimento)

---

### Camadas de Armazenamento por Frequência de Acesso

Classificação de dados baseada na frequência de uso, afetando diretamente o custo de armazenamento:

* **Acesso frequente (Hot):** Dados usados com regularidade. Custos mais altos de armazenamento, porém com acesso rápido.
* **Acesso esporádico (Cool):** Dados acessados ocasionalmente. Custo de armazenamento menor, porém com pequenas tarifas por acesso.
* **Acesso frio (Cold):** Dados raramente acessados, mas ainda relevantes para o negócio. Ideal para backup ou históricos.
* **Arquivo morto (Archive):** Dados arquivados por obrigação legal ou histórica. Armazenamento muito barato, mas com alto tempo de recuperação.

---

### Principais Provedores de Nuvem

* Microsoft Azure
* Amazon Web Services (AWS)
* Google Cloud Platform (GCP)

Todos seguem o modelo de pagamento por uso, oferecem alta disponibilidade, e suportam múltiplos serviços com **integração, segurança e escalabilidade.
