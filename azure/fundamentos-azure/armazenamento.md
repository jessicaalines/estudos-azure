
* Armazenamento - domínio de objetivo:
	* Contas de Armazenamento:
		* Precisa ter um nome globalmente exclusivo (criar um padrão parecido)
		* Fornecer acesso à internet em todo o mundo
		* Determinar os serviços de armazenamento e as opções de redundância
* Redundância de armazenamento:
	* LRS: armazenamento com redundância local (datacenter individual na região primária) >> 11 noves
	* ZRS: armazenamento com redundância de zona (três zonas de disponibilidade na região primária) >> 12 noves >> 3 CÓPIAS EM 3 LUGARES DIFERENTES
	* GRS: armazenamento com redundância geográfica (datacenter único no primário e região secundária) >> 16 noves >> 3 CÓPIAS NA REGIÃO PRINCIPAL E 3 NA SECUNDÁRIA
	* GZRS: armazenamento com redundância de zona geográfica (três zonas de disponibilidade na região primária e um único datacenter na região secundária) >> 16 noves >> 3 CÓPIAS EM 3 LUGARES >> DADOS ABSURDAMENTE VALIOSOS
* Serviços de armazenamento do Azure e pontos de extremidade:
	* Blob do Azure: otimizado para o armazenamento de quantidades massivas de dados não estruturados, como textos ou dados binários
	* Disco do Azure: fornece discos para máquinas virtuais, aplicativos e outros serviços acessarem e utilizarem
	* Fila do Azure: serviço de armazenamento de mensagens que fornece armazenamento e recuperação para grandes quantidades de mensagens, cada uma com até 64 kb
	* Arquivos do Azure: configura um compartilhamento de arquivos de rede altamente disponível que pode ser utilizado usando o protocolo Bloco de Mensagens do Servidor
	* Tabelas do Azure: fornece uma opção de chave/atributo para o armazenamento de dados estruturados não relacionais com um design sem esquema
* Camadas de acesso de armazenamento do Azure:
	* Quanto mais frequente a camada, maior o valor e menor o tempo de download
	* Frequente: otimizada para armazenamento de dados acessados com frequência
	* Esporádico: otimizada para armazenamento de dados acessados com pouca frequência e armazenados por pelo menos 30 dias
	* Frio: otimizado para o armazenamento de dados acessados com pouca frequência e armazenados por pelo menos 90 dias
	* Arquivo morto: otimizada para armazenamento de dados acessados raramente e armazenados por pelo menos 180 dias com requisitos de latência flexíveis
* Azure Data Box:
	* Armazena até 80 terabytes de dados
	* Mova os backups de recuperação de desastre para o Azure
	* Proteja seus dados em uma caixa robusta durante o trânsito
	* Migre dados do Azure para conformidade ou necessidades regulatórias
	* Migre dados para o Azure de locais remotos com conectividade limitada ou sem conectividade