# resumo-lab-azure-servicos

## Serviços
Nesse lab, foram apresentadas as principais possibilidades de configuração da plataforma da Azure, como mudança de idioma e aparência. Também foram introduzidas as categorias de recursos, como compute, networking e storage. Foi informada a necessidade de evitar a utilização em produção dos serviços que estão em versão prévia, pois não há garantia de continuidade desses serviços.

## Criando Máquinas Virtuais
Foram apresentadas as faixas de SLA disponibilizadas pela Azure. Quanto maior o SLA, menor o limite de tempo de inatividade em cada período, o que obriga a Azure a ressarcir o usuário caso o tempo de indisponibilidade seja ultrapassado. Também foi realizada uma visão geral em máquinas virtuais e contas de armazenamento.

## Instância de Banco de Dados
As imagens da máquina virtual foram apresentadas, com os seus diversos sistemas operacionais. Também foram explicados os tipos de tamanho da instância e aspectos de rede. A criação de um banco de dados SQL também foi introduzida, com a seleção de um servidor e uma forma de autenticação, além das diversas formas de redundância de backup.

## Arquiteturas Azure
Existe um mapa das diversas regiões disponibilizadas pela Azure, com um tour dentro de alguns datacenters.
Antes de criar qualquer recurso, é necessário criar um grupo de recursos, que estará debaixo de uma assinatura e será uma coleção de recursos com o mesmo ciclo de vida, permissões e políticas. Dentro do grupo de recursos, há log de atividades, controles de acesso, visualizador de recursos, eventos(automatizações), bloqueios, gerenciamento de custos. A criação de uma rede virtual (vnet) deve ser criada dentro de um grupo de recursos e aparecerá no log de atividade, nas implantações e no visualizador de recursos.
