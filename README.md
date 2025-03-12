<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>


# Template para Disciplina de Engenharia de Software

O repositório define um modelo (*template*) que deverá ser seguido por cada grupo no projeto.

A seguir, os passos para a preparação do projeto:

1. Um dos membros do grupo deverá realizar um *fork* deste repositório.
2. O dono do repositório deverá convidar os demais membros do grupo para serem colaboradores.
3. O dono do repositório deverá convidar o professor para ser colaborador do repositório.
4. O dono do repositório deverá habilitar o GitHub Pages. Basta seguir o [procedimento para habilitar o GitHub Pages](https://docs.github.com/pt/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site), lembrando de escolher em *Source* a opção `/docs` em lugar da opção `/root`.
5. Cada membro do grupo deverá instalar o [Git](https://git-scm.com/downloads).
6. Para a edição do conteúdo deste projeto, sugere-se que cada membro do grupo faça a instalação do [Visual Studio Code](https://code.visualstudio.com/) com as extensões [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) e [GitHub Pull Requests and Issues](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github). No entanto, cada membro poderá utilizar a IDE de sua preferência.
7. Cada membro do grupo deverá [clonar o repositório do grupo no seu computador](https://learn.microsoft.com/en-us/azure/developer/javascript/how-to/with-visual-studio-code/clone-github-repository?tabs=create-repo-command-palette%2Cinitialize-repo-activity-bar%2Ccreate-branch-command-palette%2Ccommit-changes-command-palette%2Cpush-command-palette).
8. Cada membro do grupo deverá editar o seu próprio nome no arquivo em [/docs/index.md](./docs/index.md), de preferência [criando um novo *branch* e um *pull request*](https://www.youtube.com/watch?v=LdSwWxVzUpo).
9. O dono do repositório deverá editar este arquivo, removendo estas instruções iniciais e preenchendo o restante da página com os dados do projeto do seu grupo.
10. Segurança é imprescindível nas plataforma de hospedagem de repositórios GIT. CUIDADO com exposição de senha e acesso ao repositório.


# Projeto: Sistema de Farmacia

# Grupo: ProjEngSoft

# Descrição

Contextualização
A Farmácia Vida Saudável é um estabelecimento de pequeno porte localizado
na cidade de Santos-SP. Nos últimos meses, houve o crescimento da
clientela e à necessidade de maior controle sobre seus processos
internos, sendo assim, o proprietário, Sr. Boticário, decidiu modernizar
a farmácia e implementar um sistema informatizado para gestão de vendas,
estoque e clientes.
Atualmente, a farmácia opera de forma manual, registrando pedidos em
cadernos e utilizando planilhas para controlar o estoque. Isto tem
causado problemas como erros no controle de medicamentos, falta de
registro de clientes e dificuldades na gestão financeira. 
O Sr. Boticário contratou a nossa empresa de desenvolvimento - MACK
Solutions SW - para criar um sistema que otimize a operação da farmácia.
Ele espera um sistema simples e eficiente que facilite as operações
diárias dos funcionários, garantindo maior precisão e rapidez no
atendimento.
2.2. Requisitos e Funcionalidades
Após reuniões da equipe com o Sr. Boticário e os seus funcionários, as
seguintes informações foram identificadas:
1. Cadastro de Medicamentos e Produtos:- Nome, descrição, fabricante,
lote, data de validade e quantidade em estoque.
- Preço de venda.
2. Cadastro de Clientes:
- Nome, CPF, telefone e histórico de compras.
3. Processo de Venda:
- Consulta de produtos disponíveis.
- Registro de venda associada a um cliente.
- Geração de cupom fiscal.
- Atualização do estoque.
4. Controle de Estoque:
- Atualização automática após cada venda.
- Alerta para itens com estoque baixo.
5. Relatórios Gerenciais:
- Relatórios de vendas diárias, semanais e mensais.
- Relatórios de produtos mais vendidos.
- Relatórios de clientes mais frequentes.
6. Autenticação e Controle de Acesso:
- Perfis de usuário: atendente e administrador.
- Atendentes podem realizar vendas e consultar estoque.
- Administradores podem cadastrar produtos, gerar relatórios e visualizar
histórico completo.
2.3. Fluxo do Sistema
Segundo os Arquitetos de Software da MACK Solutions SW, o processo típico
dentro da farmácia possui as seguintes etapas:
1. O cliente chega à farmácia e solicita um medicamento.
2. O atendente pesquisa no sistema se o produto está disponível.
3. Caso disponível, o atendente registra a venda, vinculando ao CPF do
cliente.
4. O sistema atualiza automaticamente o estoque e gera o cupom fiscal.
5. O cliente realiza o pagamento e recebe seu produto.
6. O administrador pode visualizar relatórios de vendas e estoque
diariamente.

# Documentação

Os arquivos da documentação deste projeto estão na pasta [/docs](/docs), e o seu conteúdo é publicado em **https://<usuario>.github.io/UML-Classroom-FCI/blob/master/docs/index.md**



# Releases

Deverá ser publicado um release ao término de cada entrega do projeto.
