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



=================================================== Entrega Desafio- Análise de Sentimentos com Language Studio no Azure AI  =============================================================



A Análise de Sentimentos é uma técnica de Processamento de Linguagem Natural (NLP) que identifica e classifica opiniões, emoções e intenções em textos. É amplamente usada em redes sociais, chatbots, pesquisas de satisfação e análise de feedback.

O Azure AI Language é um serviço da Microsoft que oferece ferramentas de NLP, incluindo:

Análise de Sentimentos

Reconhecimento de Entidades

Extração de Frases-Chave

Detecção de Idioma

O Language Studio é uma interface gráfica que permite usar esses recursos sem escrever código.

3. Principais Recursos para Análise de Sentimentos
Classificação de polaridade: Positivo, negativo ou neutro.

Pontuação de confiança: Probabilidade da classificação estar correta.

Análise por frase: Detalha o sentimento em diferentes partes do texto.

Opinião e aspecto (Aspect-Based Sentiment Analysis - ABSA): Identifica sentimentos sobre elementos específicos (ex.: "A bateria do celular é ruim, mas a tela é ótima").

4. Como Usar no Language Studio
Acessar o Azure AI Language (portal.azure.com).

Criar um recurso de Language Service.

Abrir o Language Studio (language.cognitive.azure.com).

Selecionar "Análise de Sentimentos" e inserir o texto para análise.

Visualizar resultados: Sentimento geral, scores e análise por frase.

5. Integração com Aplicações
API REST: Usar o endpoint do serviço para integrar a análise em apps.

SDKs (Python, C#, Java): Facilitam a implementação em código.

Power Automate/Azure Logic Apps: Automatizar análises em fluxos de trabalho.

6. Casos de Uso
Monitoramento de redes sociais: Avaliar reações a marcas.

Atendimento ao cliente: Priorizar reclamações.

Pesquisas de mercado: Analisar feedback de produtos.

7. Vantagens do Azure AI Language
Pré-treinado: Funciona bem sem necessidade de treinamento personalizado.

Escalável: Processa grandes volumes de texto.

Fácil integração: Compatível com outros serviços Azure.

8. Limitações
Idiomas suportados: Melhor desempenho em inglês; outros idiomas podem ter precisão menor.

Contexto complexo: Ironia, sarcasmo e gírias podem gerar falsos positivos.

Pra quem quer integrar em app, tem API REST e SDKs (Python, C#, etc.), então dá pra botar isso num chatbot, sistema de suporte ou até num dashboard de análise de redes sociais. O Azure já vem com modelos pré-treinados, então funciona bem pra inglês e mais ou menos pra português (depende do contexto – sarcasmo ainda pega meio mal).

======================================================================================================================================================



=================================================== Entrega Desafio- Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados  =============================================================

É um serviço de busca em nuvem que usa IA para indexar e consultar dados de forma avançada. Com o AI Search, ele vai além da busca tradicional, extraindo informações de textos, imagens e até documentos complexos.

Como Funciona?
Indexação – Extrai dados de fontes como Blob Storage, SQL DB ou Cosmos DB.

Enriquecimento com IA – Usa modelos de NLP e visão computacional para:

Reconhecer entidades (nomes, lugares).

Extrair palavras-chave.

Analisar imagens (OCR, detecção de objetos).

Busca Inteligente – Consultas com:

Correção ortográfica.

Filtros semânticos (ex.: "encontrar contratos de 2024 relacionados a impostos").

Principais Vantagens
✔ Escalável – Lida com milhões de documentos.
✔ Integrado com Azure – Conecta a Azure Functions, Power BI, etc.
✔ Customizável – Define pesos de relevância e sinônimos.

Casos de Uso
Busca em sites (e-commerce, portais).

Mineração de documentos corporativos (PDFs, emails).

Aplicações com dados estruturados e não estruturados.

======================================================================================================================================================


Explorando os Recursos de IA Generativa com Copilot e OpenAI



O Copilot (Microsoft) e a OpenAI (como ChatGPT e GPT-4) são ferramentas poderosas que usam IA generativa para criar textos, código, análises e até imagens a partir de prompts simples.

Copilot no GitHub: Sugere e completa código em tempo real.

Copilot no Microsoft 365: Gera documentos, e-mails e apresentações no Word, Outlook e PowerPoint.

Azure OpenAI Service: Integra modelos da OpenAI (GPT-4, DALL·E) em aplicações corporativas.


ChatGPT: Gera textos, responde perguntas e ajuda em criatividade.

DALL·E: Cria imagens a partir de descrições textuais.

Assistants API: Permite criar assistentes personalizados para tarefas específicas.

Vantagens:
Produtividade acelerada – Automatiza redação, código e análise de dados.
Personalização – Adapta respostas com fine-tuning ou prompts específicos.
Integração fácil – Usa APIs para conectar a apps, chatbots e fluxos de trabalho.


======================================================================================================================================================
