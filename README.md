# Gerenciador-De-Estudos

# Estilo do Projeto
O arquivo CSS define o estilo da aplicação, proporcionando uma aparência moderna e responsiva com cores escuras, contraste acentuado e tipografia personalizada.

# Paleta de Cores:

A paleta de cores é baseada em tons escuros, com um fundo predominantemente preto ou cinza escuro. Isso cria um ambiente visual agradável, reduzindo a fadiga ocular e proporcionando um bom contraste com o texto claro e os elementos interativos.
# Tipografia:

A fonte utilizada é 'Kanit', uma fonte sans-serif moderna, que contribui para a legibilidade e uma estética limpa. A combinação de tamanhos de fonte e cores distintas (como o amarelo vibrante para os títulos) ajuda a destacar as informações importantes.
Layout e Estrutura:

O layout é centrado e responsivo, com um max-width definido para o container principal, garantindo que o conteúdo não se estenda excessivamente em telas maiores. O uso de margens automáticas (margin: auto) centraliza o conteúdo horizontalmente na página.
# Elementos de Entrada:

Os elementos de formulário, como input e select, são estilizados para terem bordas arredondadas, uma cor de fundo escura e transições suaves. Isso melhora a usabilidade e oferece uma aparência coerente em todo o aplicativo.
$ Botões:

Os botões possuem cores chamativas e transições que melhoram a interação do usuário. O botão principal para adicionar atividades é destacado com uma cor de fundo vermelha, enquanto o botão de remoção tem um vermelho mais escuro, enfatizando sua função.
# Componentes de Informações:

Os containers que exibem as atividades de estudo são organizados de forma flexível, utilizando display: flex para alinhar os itens de forma eficiente. Isso garante que as informações sejam apresentadas de maneira clara e estruturada, facilitando a leitura.
# Espaçamento e Sombreamento:

O uso de padding, margin e border-radius em diversos elementos proporciona um layout arejado e organizado. Além disso, sombras sutis nos containers adicionam profundidade, fazendo com que o aplicativo se destaque visualmente.

O código JS é um aplicativo React chamado "Gerenciador de Estudos 2024", que permite aos usuários organizar suas atividades de estudo ao longo da semana. Abaixo está uma visão geral de como o aplicativo funciona como um todo:
# Estado Inicial:

O aplicativo utiliza o hook useState do React para gerenciar três estados principais:
estudos: Um objeto que armazena as atividades de estudo para cada dia da semana, com períodos divididos em manhã, tarde e noite. Inicialmente, todos os períodos estão vazios.
atividade: Um string que armazena a atividade de estudo que o usuário deseja adicionar.
diaSelecionado: Um string que representa o dia da semana selecionado pelo usuário para adicionar uma atividade.
periodoSelecionado: Um string que indica qual período (manhã, tarde ou noite) a atividade se refere.
# Adicionando Atividades:

A função adicionarAtividade permite ao usuário adicionar uma nova atividade de estudo ao dia e período selecionados. Se o campo de atividade estiver vazio, a função não faz nada.
Após adicionar a atividade, o estado atividade é limpo para preparar para a próxima entrada.
# Removendo Atividades:

A função removerAtividade permite ao usuário remover uma atividade de estudo, definindo o valor correspondente (manhã, tarde ou noite) como uma string vazia.
# Interface do Usuário:

O layout é dividido em uma seção de entrada onde o usuário pode escolher o dia, o período e a matéria que deseja estudar, além de um botão para adicionar a atividade.
A lista de dias da semana é exibida, mostrando as atividades para cada período. Se não houver atividade para um período específico, o aplicativo exibe "Nenhum estudo".
Para cada atividade existente, há um botão "X" que permite ao usuário removê-la.
# Renderização:

O aplicativo renderiza dinamicamente a lista de dias e as atividades correspondentes, atualizando a interface sempre que o estado estudos é modificado. Isso permite que as mudanças sejam refletidas em tempo real, proporcionando uma experiência interativa ao usuário.
