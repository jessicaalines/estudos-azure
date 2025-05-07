* Regiões:
	* Compostas de um ou mais datacenters muito próximos (geralmente são 3)
		* Em média 150 milhas de distância
	* Fornecem flexibilidade e escala para reduzir a latência do cliente
	* Preservam a residência dos dados com uma oferta abrangente de conformidade
	* Impactos: preço, disponibilidade do serviço
* Zonas de disponibilidade:
	* Pontos geográficos com 3 zonas de disponibilidade (datacenters)
	* Fornece proteção contra tempo de inatividade devido a falha do datacenter
	* Separa fisicamente os datacenters dentro da mesma região
	* Cada datacenter é equipado com alimentação, resfriamento e rede independentes
	* Conectadas por meio de redes privadas de fibra óptica
* Pares de região:
	* No mínimo 300 milhas de separação entre os pares de regiões (conceito pensado em Europa, porque atualmente, várias zonas pares são bastante distantes)
	* Replicação automática para alguns serviços
	* Recuperação de região priorizada em caso de interrupção
	* As atualizações são distribuídas sequencialmente para minimizar o tempo de inatividade
	* Exemplo: caiu a cloud no Brasil e a região par é do centro-sul dos EUA, fica garantido que todos os recursos que tem na cloud do Brasil, também tenham na sua região par
* Regiões soberanas do Azure (EUA e China):
	* EUA: Atende as necessidades de segurança e conformidade das agências federais, governos estaduais e locais dos EUA e seus provedores de soluções
	* Azure Governamental:
		* Instância separada do Azure
		* Fisicamente isolada de implantações que não sejam do governo dos EUA (localização não divulgada)
		* Acessível somente a pessoal autorizado
	* China: Microsoft é o primeiro provedor estrangeiro de serviços de nuvem pública da China, em conformidade com as regulamentações governamentais
		* Recursos do Azure China:
			* Instâncias fisicamente separadas dos serviços de nuvem do Azure, operados pela **21Vianet**
			* Todos os dados permanecem dentro da China, para garantir a conformidade
* Recursos do Azure:
	* Componentes como: armazenamento, VMs e redes que estão disponíveis para criar soluções de nuvem
	* Grupo de recursos:
		* Contêiner usado para agregar e gerenciar recursos em uma única unidade
		* Os recursos podem existir em apenas um grupo de recursos
		* Os recursos podem existir em regiões diferentes
		* Os recursos podem ser movidos para diferentes grupos de recursos
		* Os aplicativos podem utilizar vários grupos de recursos
		* Posso ter um grupo de recursos no Brasil e dentro dele um recurso nos EUA
* Assinaturas do Azure e grupos de gerenciamento:
	* Assinaturas do Azure: fornece acesso autenticado e autorizado às contas do Azure
		* Limite de cobrança: gerar relatórios de cobrança e faturas separados para cada assinatura
		* Limite do controle de acesso: gerenciar e controlar o acesso aos recursos que os usuários podem provisionar com assinaturas específicas
		* Para empresas com menos de 500 funcionários: a Azure não vende a assinatura diretamente, ela vende através de intermediários e são eles que enviam a conta para a empresa que está usando o serviço
		* Conta: o que será pago
		* O que tem dentro da assinatura? Grupo de recursos e recursos
		* Acima da assinatura há os grupos de gerenciamento
			* Exemplo: tenho 200 assinaturas e preciso replicar uma policy para todas: faço isso através do grupo de gerenciamento, porque ele é quem gerencia as assinaturas
		* Grupos de recursos: podem incluir várias assinaturas do Azure
			* As assinaturas herdam as condições aplicadas ao grupo de gerenciamento
			* É possível oferecer suporte a 10.000 grupos de gerenciamento em um único diretório
			* Uma árvore de grupos de gerenciamento pode oferecer suporte a até 6 níveis de profundidade