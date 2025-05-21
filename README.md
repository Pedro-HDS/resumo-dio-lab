Resumo de Aulas Microsoft Azure.

Aula 1 -  Criação da conta Microsoft

Aula 2 - Apresentação de recursos basicos navegando por categorias, além de computação como areas de virtualização, criação de firewalls e servidores de bridge.

Aula 3 - Benefícios da Nuvem Azure, Escalabilidade e Elasticidade, Confiabilidade, Previsibilidade e Segurança, Governança e Gerenciabilidade.


====================================================================================================================================================================================


Aula 4 - Criando maquinas virtuais na Azure:

Acesse o Portal Azure (portal.azure.com)

Clique em "Criar um recurso" > "Máquina Virtual"

Preencha os campos básicos:

Assinatura

Grupo de recursos (crie ou use existente)

Nome da VM

Região

Imagem (SO, ex: Windows Server ou Ubuntu)

Tamanho (escolha a configuração)

Configure credenciais de administrador

Selecione portas de entrada (ex: RDP 3389 para Windows, SSH 22 para Linux)

Revise + criar > "Criar"

==========================================================================================================================================================================================

Aula 5 - IaaS, PaaS e SaaS e Responsabilidades.


Aula 6 - Para configurar uma instância de banco de dados no Azure, acesse o portal Azure > "Criar um recurso" > "Bancos de dados" > escolha o serviço (SQL Database, MySQL, PostgreSQL, etc.) > preencha nome, servidor (ou crie um novo), tipo de banco, tamanho, credenciais de acesso > configure rede (IPs permitidos) > revise e crie.

Aula 7 - Componentes da arquitetura da Azure.

Aula 8 e 9 -  Componentes de computação e rede, uso de Zonas de Disponibilidade Rede Virtual (VNet): Isola recursos em uma rede privada.
Azure Load Balancer: Distribui tráfego entre VMs. Gateway de VPN/Azure ExpressRoute: Conexão segura entre nuvem e local.

====================================================================================================================================================================================================================================================================
Aula 10 - Entendo escalabilidade, tamanho das VMs e custos:

Séries de VMs (selecione conforme a carga de trabalho):

Série B (Burstable): Para cargas variáveis (ex: dev/teste).

Série D/Dsv3: Uso geral (CPU balanceado).

Série E/Es_v4: Memória otimizada (aplicações em RAM).

Série Fsv2: Computação otimizada (alta CPU).

Série NCv3/NV: GPUs (IA, renderização).

Fatores de Dimensionamento:

vCPUs: Núcleos virtuais (ex: 2, 4, 8, 16).

Memória RAM: De 2 GB a 3,8 TB (depende da série).

Armazenamento Temporário (SSD): Discos locais não persistentes.****

====================================================================================================================================================================================================================================================================

Aula 11 - Identidade, Acesso e Segurança 


Microsoft Defender for Cloud
Função principal:

Monitoramento contínuo de segurança em ambientes Azure, híbridos (on-premises) e multicloud.

Identifica ameaças em tempo real (vulnerabilidades, ataques, configurações inseguras).
Principais recursos:

Proteção contra ameaças:

Detecta atividades maliciosas (ex: brute force, malware, tráfego suspeito).

Usa IA para análise comportamental.

Gerenciamento de vulnerabilidades:

Escaneia VMs, containers, SQL DBs em busca de falhas conhecidas.

Recomendações de segurança:

Nota de segurança (score) baseada no benchmark CIS.

Sugere correções (ex: habilitar MFA, atualizar sistemas).

Integração com ferramentas:

Conecta-se a Azure Sentinel (SIEM/SOAR) para resposta a incidentes.

Compatível com AWS e GCP (multicloud).

Conformidade:

Relatórios para padrões como NIST, ISO 27001, GDPR.

Como habilitar:

No portal Azure, acesse Defender for Cloud > Ativar Defender Plans (camada gratuita ou paga).


