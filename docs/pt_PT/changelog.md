# Registro de alterações Jeedom V4.1

## 4.1.0

### Pré-requisitos

- Debian 10 Buster

### Notícias / Melhorias

- **Síntese** : Adicionando uma nova página **Home → Resumo** oferecendo um resumo visual global das peças, com acesso rápido aos resumos.
- **Pesquisa** : Adição de um mecanismo de pesquisa em **Ferramentas → Pesquisa**.
- **Painel de instrumentos** : Modo de edição agora inserindo o bloco movido.
- **Painel de instrumentos** : Modo de edição: os ícones de atualização do equipamento são substituídos por um ícone que permite acesso à sua configuração, graças a um novo modal simplificado.
- **Painel de instrumentos** : Agora podemos clicar no *Tempo* widgets de ações de tempo para abrir a janela do histórico do comando info vinculado.
- **Painel de instrumentos** : O tamanho do bloco de um novo equipamento se adapta ao seu conteúdo.
- **Painel de instrumentos** : Adicionar (voltar!) Um botão para filtrar os itens exibidos por categoria.
- **Painel de instrumentos** : Ctrl Clique em uma informação para abrir a janela do histórico com todos os comandos históricos do equipamento visíveis no bloco. Ctrl Clique em uma legenda para exibir apenas esta, Alt Clique para exibir todas.
- **Painel de instrumentos** : Redesenho da exibição da árvore de objetos (seta à esquerda da pesquisa).
- **Painel de instrumentos** : Capacidade de desfocar imagens de fundo (Configuração -> Interface).
- **Ferramentas / Widgets** : A função *Aplicar em* mostra os comandos vinculados marcados, desmarcando um aplicará o widget principal padrão a este comando.
- **Widgets** : Adicionando um widget principal *sliderVertical*.
- **Widgets** : Adicionando um widget principal *binarySwitch*.
- **Update Center** : As atualizações são verificadas automaticamente quando a página é aberta, se for 120 minutos mais antiga.
- **Update Center** : A barra de progresso está agora na guia *Núcleo e plugins*, e o log aberto por padrão na guia *Informação*.
- **Update Center** : Se você abrir outro navegador durante uma atualização, a barra de progresso e o log indicarão.
- **Update Center** : Se a atualização terminar corretamente, é exibida uma janela pedindo para recarregar a página.
- **Atualizações principais** : Implementação de um sistema para limpar arquivos Core não utilizados antigos.
- **Cenas** : Adicionando um mecanismo de pesquisa (à esquerda do botão Executar).
- **Cenas** : Adição da função de idade (fornece a idade do valor da ordem).
- **Cenas** : *stateChanges()* agora aceite o período *Hoje* (meia-noite até agora), *ontem* e *dia* (por 1 dia).
- **Cenas** : FUNÇÕES *estatísticas (), média (), max (), min (), tendência (), duração()* : Bugfix ao longo do período *ontem*, e aceite agora *dia* (por 1 dia).
- **Cenas** : Possibilidade de desativar o sistema de cotação automática (Configurações → Sistema → Configuração : Commandes).
- **Cenas** : Visualizando um *Aviso* se nenhum gatilho estiver configurado.
- **Cenas** : Correção de bug de *selecionar* em bloco copiar / colar.
- **Cenas** : Copiar / colar do bloco entre diferentes cenários.
- **Cenas** : As funções desfazer / refazer estão agora disponíveis como botões (ao lado do botão de criação de bloco).
- **Cenas** :  adição de "Exportação histórica" (exportHistory)
- **Janela Variáveis de Cenário** : Ordenação alfabética na abertura.
- **Janela Variáveis de Cenário** : Os cenários usados pelas variáveis agora são clicáveis, com a abertura da pesquisa na variável.
- **Análise / História** : Ctrl Clique em uma legenda para exibir apenas esse histórico, Alt Clique para exibir todos eles.
- **Análise / História** : As opções *agrupamento, tipo, variação, escada* estão ativos apenas com uma única curva exibida.
- **Análise / História** : Agora podemos usar a opção *área* com a opção *Escada*.
- **Análise / Logs** : Nova fonte de tipo monoespaçado para logs.
- **Vista** : Possibilidade de colocar cenários.
- **Vista** : Modo de edição agora inserindo o bloco movido.
- **Vista** : Modo de edição: os ícones de atualização do equipamento são substituídos por um ícone que permite acesso à sua configuração, graças a um novo modal simplificado.
- **Vista** : A ordem de exibição agora é independente da ordem no painel.
- **Cronograma** : Separação das páginas de histórico e cronograma.
- **Cronograma** : Integração da linha do tempo no DB por motivos de confiabilidade.
- **Cronograma** : Gerenciamento de várias linhas do tempo.
- **Cronograma** : Completo redesenho gráfico da linha do tempo (Desktop / Mobile).
- **Resumo Global** : Visualização Resumo, suporte para resumos de um objeto diferente ou com um objeto raiz vazio (Desktop e WebApp).
- **Ferramentas / Objetos** : Nova aba *Resumo por equipamento*.
- **Resumo Automation** : Equipamentos de plug-in desativados e seus controles não têm mais os ícones à direita (configuração do equipamento e configuração avançada).
- **Resumo Automation** : Capacidade de pesquisar nas categorias de equipamentos.
- **Resumo Automation** : Possibilidade de mover várias peças de equipamento de um objeto para outro.
- **Resumo Automation** : Possibilidade de selecionar todo o equipamento de um objeto.
- **Mecanismo de tarefas** : Na guia *Demônio*, plugins desativados não aparecem mais.
- **Relatório** : O uso de *cromo* se disponível.
- **Relatório** : Possibilidade de exportar cronogramas.
- **Configuração** : A guia *Informação* agora está na guia *Geral*.
- **Configuração** : A guia *Comandos* agora está na guia *Instalações*.
- **Janela de configuração avançada de equipamentos** : Alteração dinâmica da configuração do quadro de distribuição.
- **Instalações** : Nova categoria *Abertura*.
- **Instalações** : Possibilidade de inverter comandos do tipo cursor (informação e ação)
- **Instalações** : Possibilidade de adicionar css de classe a um bloco (consulte a documentação do widget).
- **Sobre a janela** : Adição de atalhos ao Changelog e FAQ.
- Páginas de Widgets / Objetos / Cenários / Interações / Plugins :
	- Ctrl Clic / Clic Center em um equipamento de widget, objeto, cenário, interação, plug-in : Abre em uma nova guia.
	- Ctrl Clic / Clic Center também disponível em seus menus de contexto (nas guias).
- Nova página ModalDisplay :
	- Menu Análise : Ctrl Clique / Clique em Central no *Tempo real* : Abra a janela em uma nova guia, em tela cheia.
	- Menu Ferramentas : Ctrl Clique / Clique em Central no *Anotações*, *Testador de expressão*, *Variáveis*, *Pesquisa* : Abra a janela em uma nova guia, em tela cheia.
- Bloco de código, editor de arquivos, personalização avançada : Adaptação tema escuro.

### WebApp
- Integração da nova página Resumo.
- Na página Cenários, um clique no título do cenário exibe seu log.
- Agora podemos selecionar / copiar parte de um log.
- Na pesquisa em um log, adição de um botão x para cancelar a pesquisa.
- Persistência da alternância do tema (8h).
- Em um design, um clique com três dedos retorna à página inicial.
- Exibição de cenários por grupo.
- Nova fonte de tipo monoespaçado para logs.
- Muitas correções de bugs (UI, retrato / paisagem iOS, etc.).

### Autres
- **Documentação** : Adaptações de acordo com v4 e v4.1.
- **Documentação** : Nova página *Atalhos de teclado / mouse* incluindo um resumo de todos os atalhos no Jeedom. Acessível no documento do Painel ou nas Perguntas frequentes.
- **Lib** : Atualizar o HighStock v7.1.2 a v8.2.0.
- **Lib** : Atualizar o jQuery v3.4.1 a v3.5.1.
- **Lib** : Atualizar fonte Awesome 5.9.0 a 5.13.1.
- **API** :  adição de uma opção para proibir uma chave de API de um plugin de executar métodos centrais (geral)
- Protegendo solicitações Ajax.
- Protegendo chamadas de API.
- Correções de bugs.
- Inúmeras otimizações de desempenho de desktop / dispositivos móveis.

### Changements
- A função **cenário-> getHumanName()** da classe de cenário php não retorna mais *[objeto] [grupo] [nome]* Mas *[grupo] [objeto] [nome]*.
- A função **cenário-> byString()** agora deve ser chamado com a estrutura *[grupo] [objeto] [nome]*.
- Funções **rede-> getInterfaceIp () rede-> getInterfaceMac () rede-> getInterfaces()** foram substituídos por **rede-> getInterfacesInfo()**


# Changelog Jeedom V4.0

## 4.0.61

- Corrigido um problema ao aplicar um modelo de cenário
- Adição de uma opção para desativar a verificação SSL durante a comunicação com o mercado (não recomendado, mas útil em certas configurações de rede específicas)
- Corrigido um problema com o histórico de arquivamento se o modo de suavização fosse para sempre
- Correções de bugs
- Correção do comando trigger () em cenários para que ele retorne o nome do gatilho (sem o #) em vez do valor, para o valor você deve usar triggerValue()

## 4.0.60

- Remoção do novo sistema DNS em eu.jeedom.link seguindo muitos operadores que proíbem fluxos http2 permanentes

## 4.0.59

- Bugs corrigidos em widgets de tempo
- Aumento do número de senhas ruins antes do banimento (evita problemas com o aplicativo da web ao girar chaves da API)

## 4.0.57

- Reforço da segurança do cookie
- Usando cromo (se instalado) para relatórios
- Corrigido um problema com o cálculo do tempo de estado em widgets se o fuso horário jeedom não for o mesmo do navegador
- Correções de bugs

## 4.0.55

- O novo dns (\*. Eu.jeedom.link) torna-se o DNS primário (o DNS antigo ainda funciona)

## 4.0.54

- Início da atualização para o novo site de documentação

## 4.0.53

- Bug fix.

## 4.0.52

- Correção de bug (atualização para fazer absolutamente se você estiver na versão 4.0.51).

## 4.0.51

- Correções de bugs.
- Otimização do futuro sistema DNS.

## 4.0.49

- Possibilidade de escolher o motor Jeedom TTS e possibilidade de ter plugins que oferecem um novo motor TTS.
- Suporte aprimorado de webview no aplicativo móvel.
- Correções de bugs.
- Atualizando o documento.

## 4.0.47

- Testador de expressão aprimorado.
- Atualizando o repositório no smart.
- Correções de bugs.

## 4.0,44

- Traduções melhoradas.
- Correções de bugs.
- Restauração de backup em nuvem aprimorada.
- A restauração da nuvem agora recupera apenas o backup local, deixando a opção de fazer o download ou restaurá-lo.

## 4.0.43

- Traduções melhoradas.
- Bugs corrigidos em modelos de cenário.

## 4.0.0
- Redesenho completo do tema (Core 2019 Light / Dark / Legacy).
- Possibilidade de mudar o tema automaticamente dependendo do tempo.
- No celular, o tema pode mudar dependendo do brilho (Requer para ativar *sensor extra genérico* no chrome, página chrome://flags).<br/><br/>
- Melhoria e reorganização do menu principal.
- Menu de plugins : A lista de categorias e plugins agora está classificada em ordem alfabética.
- Menu Ferramentas : Adicione um botão para acessar o testador de expressão.
- Menu Ferramentas : Adicionando um botão para acessar as variáveis.<br/><br/>
- Os campos de pesquisa agora suportam acentos.
- Os campos de pesquisa (painel, cenários, objetos, widgets, interações, plug-ins) agora estão ativos quando a página é aberta, permitindo que você digite uma pesquisa diretamente.
- Adicionado um botão X nos campos de pesquisa para cancelar a pesquisa.
- Durante uma pesquisa, a chave *escapar* cancelar pesquisa.
- Painel de instrumentos : No modo de edição, o controle de pesquisa e seus botões são desativados e se tornam fixos.
- Painel de instrumentos : No modo de edição, um clique de um botão *expandir* à direita dos objetos redimensiona os ladrilhos do objeto para a altura do mais alto. Ctrl + clique os reduz à altura do mais baixo.
- Painel de instrumentos : A execução do comando em um bloco agora é sinalizada pelo botão *Atualizar*. Se não houver nenhum no bloco, ele aparecerá durante a execução.
- Painel de instrumentos : Os blocos indicam um comando de informação (historizado, que irá abrir a janela Histórico) ou ação ao passar o mouse.
- Painel de instrumentos : A janela de histórico agora permite que você abra este histórico em Análise / Histórico.
- Painel de instrumentos : A janela de histórico mantém sua posição / dimensões ao reabrir outro histórico.
- Janela Configuração de Comando: Ctrl + clique em "Salvar" fecha a janela após.
- Janela Configuração do equipamento: Ctrl + clique em "Salvar" fecha a janela após.
- Adicionar informações de uso ao excluir um dispositivo.
- Objetos : Adicionada opção para usar cores personalizadas.
- Objetos : Adição de um menu contextual nas guias (mudança rápida de objeto).
- Interações : Adição de um menu contextual nas guias (mudança rápida de interação).
- Plugins : Adição de um menu contextual nas abas (troca rápida de equipamento).
- Plugins : Na página de gerenciamento de plug-ins, um ponto laranja indica que os plug-ins em versão não estável.
- Melhorias na tabela com filtro e opção de classificação.
- Possibilidade de atribuir um ícone a uma interação.
- Cada página do Jeedom agora tem um título no idioma da interface (guia do navegador).
- Prevenção de preenchimento automático em campos 'Código de acesso''.
- Gestão de funções *Página anterior / próxima página* do navegador.<br/><br/>
- Widgets : Redesenho do sistema de widgets (menu Ferramentas / Widgets).
- Widgets : Possibilidade de substituir um widget por outro em todos os comandos que o utilizam.
- Widgets : Possibilidade de atribuir widgets a vários comandos.
- Widgets : Adicionar um widget de informação numérica horizontal.
- Widgets : Adicionar um widget de informação numérica vertical.
- Widgets : Adição de um widget de bússola / vento numérico (obrigado @thanaus).
- Widgets : Adicionado um widget numérico de informações de chuva (obrigado @thanaus)
- Widgets : Exibição do widget do obturador de informações / ação proporcional ao valor.<br/><br/>
- Configuração : Melhoria e reorganização de guias.
- Configuração : Adição de muitos *dicas* (aide).
- Configuração : Adicionar um motor de pesquisa.
- Configuração : Adicionado um botão para esvaziar o cache de widgets (guia Cache).
- Configuração : Adicionada uma opção para desativar o cache de widgets (guia Cache).
- Configuração : Possibilidade de centrar verticalmente o conteúdo dos tiles (guia Interface).
- Configuração : Adicionou um parâmetro para a eliminação global de logs (guia Pedidos).
- Configuração : Mudança de #message# à #subject# em Configuração / Logs / Mensagens para evitar a duplicação da mensagem.
- Configuração : Possibilidade nos resumos de adicionar uma exclusão de pedidos que não foram atualizados por mais de XX minutos (exemplo para o cálculo de médias de temperatura se um sensor não reportou nada por mais de 30min será excluído do cálculo)<br/><br/>
- Cenas : A colorização dos blocos não é mais aleatória, mas por tipo de bloco.
- Cenas : Possibilidade ao fazer um Ctrl + clique no botão *execução* salve-o, execute-o e exiba o log (se o nível de log não estiver ativado *Nemhum*).
- Cenas : Confirmação de exclusão de bloco. Ctrl + clique para evitar a confirmação.
- Cenas : Adição de uma função de pesquisa em blocos de código. Pesquisa : Ctrl + F e Enter, próximo resultado : Ctrl + G, resultado anterior : Ctrl + Shift + G
- Cenas : Possibilidade de condensar os blocos.
- Cenas : A ação 'Adicionar bloco' muda para a guia Cenário, se necessário.
- Cenas : Novas funções de copiar / colar em bloco. Ctrl + clique para cortar / substituir.
- Cenas : Um novo bloco não é mais adicionado ao final do cenário, mas após o bloco onde você estava antes de clicar, determinado pelo último campo que você clicou.
- Cenas : Configurando um sistema Desfazer / Refazer (Ctrl + Shift + Z / Ctrl + Shift + Y).
- Cenas : Remover compartilhamento de cenário.
- Cenas : Melhoria da janela de gerenciamento do modelo de cenário.<br/><br/>
- Análise / Equipamento : Adição de um motor de busca (guia Baterias, pesquisa por nomes e pais).
- Análise / Equipamento : A zona do dia do calendário / equipamento agora pode ser clicada para acessar diretamente a (s) troca (s) de bateria).
- Análise / Equipamento : Adicionando um campo de pesquisa.<br/><br/>
- Update Center : Aviso na guia 'Core e plug-ins' e / ou 'Outros' se uma atualização estiver disponível. Mude para 'Outros' se necessário.
- Update Center : diferenciação por versão (estável, beta, ...).
- Update Center : adição de uma barra de progresso durante a atualização.<br/><br/>
- Resumo Automation : O histórico de exclusões agora está disponível em uma guia (Resumo - Histórico).
- Resumo Automation : Redesenho completo, possibilidade de solicitar objetos, equipamentos, pedidos.
- Resumo Automation : Adicionando equipamentos e IDs de pedido, para exibir e pesquisar.
- Resumo Automation : Exportação CSV de objeto pai, id, equipamento e seu id, comando.
- Resumo Automation : Possibilidade de tornar visível ou não um ou mais comandos.<br/><br/>
- Projeto : Possibilidade de especificar a ordem (posição) do *Projetos* e *Projetos 3D* (Editar, Configurar Design).
- Projeto : Adição de um campo CSS personalizado nos elementos do *Projeto*.
- Projeto : Movidas as opções de exibição em Design da configuração avançada, nos parâmetros de exibição do *Projeto*. Isso para simplificar a interface e permitir ter diferentes parâmetros por *Projeto*.
- Projeto : Movendo e redimensionando componentes em *Projeto* leva seu tamanho em consideração, com ou sem magnetização.<br/><br/>
- Iluminação geral (estilos css / inline, refatoração, etc.) e melhorias de desempenho.
- Remova Font Awesome 4 para manter apenas Font Awesome 5.
- Atualização de libs : jquery 3.4.1, CodeMiror 5,46.0, tableorter 2.31.1.
- Inúmeras correções de bugs.
- Adição de um sistema de configuração em massa (usado na página Equipamento para configurar alertas de comunicações neles)
- Adição de compatibilidade global do DNS Jeedom com uma conexão à Internet 4G.
- Correção de segurança

>**IMPORTANTE**
>
>Se após a atualização você tiver um erro no Dashboard, tente reiniciar sua caixa para que ela leve em consideração as novas adições de componentes.

>**IMPORTANTE**
>
>O plugin do widget não é compatível com esta versão do Jeedom e não será mais suportado (porque os recursos foram levados internamente no núcleo). Mais Informações [aqui](https://www.Jeedom.com/blog/4368-les-widgets-en-v4).


