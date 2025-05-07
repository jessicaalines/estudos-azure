Serviços de computação do Azure:
	* Serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais
		* VMs, aplicativo de serviços, contêiner de instâncias, AKS, área de trabalho virtual do Azure
		* VM: emulações de software de computadores físicos
			* Inclui processador virtual, memória, armazenamento e rede
			* Oferta de IaaS que oferece personalização e controle total
* Serviços de contêineres do Azure:
	* Fornecem um ambiente leve e virtualizado que não exige o gerenciamento do sistema operacional e pode responder a alterações sob demanda
		* Instâncias de contêiner do Azure: uma oferta de PaaS que executa um contêiner ou pod de contêineres do Azure
		* Aplicativos de contêiner do Azure: uma oferta de PaaS, como instâncias de contêineres que podem balancear a carga e escalar
		* Serviço de Kubernetes do Azure (AKS): um serviço de orquestração para contêineres com arquiteturas distribuídas e grandes volumes de contêineres
			* Orquestrar, escalar e gerenciar contêineres em clusters
			* Vantagem em relação às instância de contêiner: escalabilidade, garantia de disponibilidade, melhor opção para multicloud
	* Azure functions: oferta de PaaS que dá suporte a operações de computação sem servidor. O código baseado em eventos é executado quando chamado, sem exigir uma infraestrutura de servidor durante períodos inativos
		* Limite de escalabilidade
	* Serviços de aplicativos do Azure:
		* Plataforma totalmente gerenciada para criar, implantar e dimensionar aplicativos web e APIs rapidamente
			* Trabalha com: .NET, .NET Core, Node.js, Java, Pyhton pu PHP
			* Oferta de PaaS com requisitos de nível corporativo de desempenho, segurança e conformidade
			* Para aplicações maiores > resiliência e escalabilidade sem necessidade de um contêiner
	* Serviços de rede do Azure:
		* Rede Virtual do Azure (VNET) permite que os recursos do Azure se comuniquem uns com os outros, com a internet e com as redes locais
			* Rede privada no Azure que permite a comunicação segura entre recursos, como VMs e bancos de dados
			* Pontos de extremidade públicos, acessíveis de qualquer local com internet
			* Pontos de extremidade privados, acessíveis somente de dentro da sua rede
			* Sub-redes virtuais segmentam a sua rede para atender às necessidades
			* Emparelhamento de rede conecta suas redes privadas diretamente
	* DNS do Azure:
		* Confiabilidade e desempenho aproveitando uma rede global de servidores de nome DNS, usando a rede Anycast
		* A segurança do DNS do Azure se baseia no gerenciador de recursos do Azure, habilitando o controle de acesso baseado em função e o monitoramento e o registro em log
		* Facilidade de uso para gerenciar seus recursos externos e do Azure com um único serviço DNS
		* As redes virtuais personalizáveis, permitem que se use nomes de domínio privados e totalmente personalizados em suas redes virtuais privadas
		* Os registros de alias dão suporte a conjuntos de registros de alias para apontar diretamente para um recurso do Azure
