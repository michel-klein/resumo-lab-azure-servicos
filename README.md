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

## Máquinas Virtuais
Na criação de máquinas virtuais, há opções de seleção de região, níveis de disponibilidade, tipo de segurança, imagem e tamanho de instância. A configuração de conjunto de dimensionamento permite escalar a quantidade de máquinas virtuais conforme a necessidade de uso. Há diversos tamanhoa de máquinas virtuais para cada tipo de uso (otimizada CPU, memória, disco). A conta de administrador deve ser configurada, e as configurações de disco e rede devem ser selecionadas. Opção de excluir o disco com a VM. Anexação com disco existente. Gerenciamento de identidade, desligamento automático, backup. Monitoramento (alertas). A área de trabalho virtual do Azure é um desktop remoto destinado a colaboradores (sessão individual ou em grupo). Aplicativo de funções altera o sistema operacional conforme a linguagem de programação selecionada.

## Armazenamento
Conta de armazenamento: blob, files (compartilhamento), filas, tabelas. Nome único. Desempenho standard/premium. Redundância (LRS, GRS, ZRS, GZRS). Possibilidade de exclusão temporária de arquivos. Compartilhamento de arquivos. Conexão para compartilhamento de arquivos está disponível para Windows, Linux e MacOS. Migrações para o Azure. Azure Data Box: migração física. AzCopy: transferência unilateral de arquivos por linha de comando. Gerenciador de armazenamento: sincronização de arquivos com a nuvem (interface visual).

## Segurança e Identidade
Microsoft Entra ID realiza o gerenciamento de usuários. Sincronização apenas apenas unidirecional on premises para cloud. Usuários permanentemente deletado após 30 dias. Self service password reset. Diferentes licenciamentos, free não tem muitas opções de roles. Custom domain names para email de usuários. Microsoft Defender for cloud (multicloud): recomendações de segurança, Devops Security (github).

## Custos
TCO (Custo Total de Propriedade): Comparação de custos entre on premises e cloud. Calculadora de preço. Tags (marcas) para gerenciamento, não herdável do grupo de recursos para os recursos, deve ser utilizado policy.
