🍔 LancheFácil - Sistema de Cardápio e Pedidos Online
Projeto prático e funcional desenvolvido para a disciplina de Ciclo de Vida e Qualidade de Software do curso de Engenharia de Software / Sistemas de Informação na Univille (Universidade da Região de Joinville).

O LancheFácil é uma aplicação web responsiva projetada para modernizar e agilizar o atendimento em lanchonetes, quiosques e lancherias. O sistema elimina a necessidade de cardápios físicos de papel e integra, em um único ecossistema serverless, a realização do pedido pelo cliente, o monitoramento de produção na cozinha e o controle gerencial administrativo.

🚀 Funcionalidades do Sistema
O sistema é dividido em dois grandes fluxos integrados que totalizam 7 telas principais:

🧑‍💻 Área do Cliente
Tela 1 – Cardápio Interativo: Listagem dinâmica de produtos separada por abas (Lanches, Bebidas, Sobremesas), barra de pesquisa por texto, filtro rápido por faixa de preço, alternância de tema (Claro/Escuro) e Modo Quiosque.

Modal de Adicionais: Janela flutuante que se abre ao selecionar um item, permitindo a customização do lanche (ex: adicionar bacon ou transformar em combo) com soma automática ao valor unitário.

Tela 2 – Formulário de Checkout: Validação de dados em tempo real, seleção da modalidade de consumo (Comer no Local, Viagem ou Entrega), exibição dinâmica de campos de endereço (apenas para entrega), aplicação de cupom de desconto (PROMO10) e resumo financeiro detalhado.

Tela 3 – Confirmação e Recibo: Exibição do número sequencial do pedido e botão de impressão nativa formatada via CSS (@media print) para cupons térmicos de 80mm.

Tela 5 – Rastreio Público: Interface onde o cliente pode digitar o número do seu pedido e acompanhar o status de produção através de uma barra de progresso dinâmica.

⚙️ Área da Lanchonete (Restrita)
Tela 6 – Login de Segurança: Tela de autenticação para proteção das rotas administrativas, contando com recurso visual para ocultar/revelar a senha.

Tela 4 – Monitor de Cozinha (KDS): Painel que exibe os pedidos em aberto de forma cronológica. Conta com cronômetro de alerta visual por cores para evitar atrasos e botão "Marcar como Pronto".

Tela 7 – Dashboard e Painel Admin: Gráfico analítico de barras com o faturamento por categoria de produto e controle completo (CRUD) para cadastrar, editar e remover itens do cardápio.

🛠️ Stack Tecnológica
Front-end: HTML5 semântico e CSS3 estruturado com variáveis nativas, Flexbox/Grid e Media Queries para total responsividade em smartphones, tablets e computadores.

Lógica e Regras de Negócio: JavaScript Avançado (ES6+) focado em manipulação assíncrona do DOM, gerenciamento de estado da aplicação e tratamento de eventos.

Banco de Dados (Nuvem): Firebase Realtime Database – Banco NoSQL baseado em estrutura JSON que provê sincronização de dados estável ponta-a-ponta via WebSockets, dispensando atualizações manuais de página (F5).

📐 Estratégia de Qualidade e Testes
A arquitetura de garantia de qualidade foi modelada estritamente sob o conceito da Pirâmide de Testes:

Testes Unitários (Nível 1): Validação isolada de funções lógicas essenciais no console do desenvolvedor (validarNome(), calcularTotal(), calcDesconto(), fmtBRL(), parseCartKey()).

Testes de Integração e Sistema (Nível 2): Validação dos fluxos completos de navegação entre telas, comportamento das validações de formulário sob dados inválidos e persistência de dados em tempo real no banco Firebase.

Teste de Aceitação (Nível 3 - UAT): Homologação final executada por uma equipe externa de testes baseada rigorosamente nos critérios de aceite documentados.

📦 Como Executar a Aplicação
Por ser um projeto estruturado em arquitetura Serverless (sem necessidade de compilação ou servidores locais pesados), a execução é extremamente simples:

Faça o download ou clone este repositório em sua máquina.

Certifique-se de que a estrutura de arquivos contém o index.html na raiz do diretório.

Dê um duplo clique sobre o arquivo index.html para abri-lo diretamente em qualquer navegador moderno (Google Chrome, Mozilla Firefox, Microsoft Edge ou Safari).

Opcional: Para uma experiência de desenvolvimento ideal com suporte a recarregamento automático, execute o projeto utilizando a extensão Live Server no VS Code.

👥 Organização do Time (Matriz RACI)
A distribuição de papéis da equipe foi desenhada para garantir que o desenvolvimento e o controle de qualidade corressem em paralelo:

Gustavo do Rosário Nunes | Product Owner / Analista de Requisitos

Definição do escopo, mapeamento das User Stories, refinamento dos critérios de aceite e acompanhamento do cronograma macro.

Vinicius Henrique Wener | Desenvolvedor Full Stack

Arquitetura de software, codificação das interfaces em HTML/CSS, desenvolvimento da lógica JavaScript, integração com o Firebase e escrita dos Testes Unitários.

João Vitor Rosera | Analista de QA (Quality Assurance)

Planejamento da estratégia de testes, execução dos roteiros de integração/sistema, abertura e controle do ciclo de vida dos relatórios de bugs.

Trabalho acadêmico apresentado à Universidade da Região de Joinville - UNIVILLE, Junho de 2026.
