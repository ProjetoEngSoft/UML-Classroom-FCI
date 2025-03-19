<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>


<font size="+12"><center>
*&lt;Sistema de Farmacia&gt;*
</center></font>

>*Observação 1: A estrutura inicial deste documento é só um exemplo. O seu grupo deverá alterar esta estrutura de acordo com o que está sendo solicitado na disciplina.*

>*Observação 2: O índice abaixo não precisa ser editado se você utilizar o Visual Studio Code com a extensão **Markdown All in One**. Essa extensão atualiza o índice automaticamente quando o arquivo é salvo.*

**Conteúdo**

- [Autores](#nome-alunos)
- [Descrição do Projeto](#introdução-do-projeto)
- [Análise de Requisitos Funcionais e Não-Fucionais](#descrição-dos-requisitos)
- [Diagrama de Atividades](#diagrama-de-atividades) 
- [Diagrama de Casos de Uso](#diagrama-de-comportamento-atores)
- [Descrição dos Casos de Uso](#descrição-das-funcões)
- [Diagrama de Senquencia](#diagrama-de-ordem-interações)
- [Diagrama de Classes](#diagrama-orientado-objetos)
- [Diagrama de Estados](#diagrama-estrutura-componente)
- [Diagrama de Implantação](#diagrama-de-hardware-software)
- [Referências](#referências)


# Autores

* Clovis Julião Arroyo Neto - 10395595
* Domingos Melo - 10402402


# Descrição do Projeto

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

# Análise de Requisitos Funcionais e Não-Funcionais
## Requisitos Funcionais
- RF-01(CADASTR0): O sistema deve conseguir cadastrar os produtos, com os seguintes atributos: Nome, descrição, fabricante, lote, data de validade, quantia de estoque e preço de venda;
- RF-02(CADASTRO): O sistema deve conseguir  cadastrar novos clientes com os seguintes atributos: Nome, CPF,  telefone e historico de compras;
- RF-03(VENDA): O sitema deve conseguir realizar o processo de venda, consultando produtos disponíveis (Pré-condição: produto existente), o registro associado ao cliente (Pré-condição: um cliente existente), geração de cupom fiscal e atualização de estoque;
- RF-04(VENDA): O sistema deve automaticamente calcular total e aplicar descontos promocionais, caso necessário;
- RF-05(CONSULTA): O sistema deve permitir consulta ao histórico de compras de clientes cadastrados;
- RF-06(ESTOQUE): O sistema deve ter um controle de estoque, que atualizará automaticamente após cada venda (Pré-condição: Processo de venda realizado) e disparar um alerta quando items estiverem com estoque baixo,  ou próximo da validade;
- RF-07(RELATÓRIO)O sistema deve realizar relatórios gerenciais, relatórios de vendas diaria, semanais e mensais (Pŕe-condição: Processo de venda realizada), relatorio de produtos mais vendidos e relatorio de clientes mais frequentes (Pŕe-condição: Cadastro de clientes);
- RF-08(SEGURANÇA): O sitema deve realizar autenticação e controle de acesso, com perfis de usuario para atendes e administradores (Pré-condição: cadastro dos colaboradores), permissão para atendentes realizarem vendas e consulta de estoque (Pré-condição: Processo de venda e relatórios de estoque),administradores devem poder cadastrar produtos, gerar relatórios  e visualizar historico completo(Pré-condição: existência do historico);
-  RF-09(CONSULTA): O sistema deve permitir busca no estoque por nome ou código de barras;
-  RF-10(PAGAMENTO): O sistema deve integrar-se com o sistema de pagaeento para processar cartões de crédito ou débito;

## Requisitos não-funcionais
- O sistema deve conseguir realizar vendas simultaneas;
- O sistema deve tolerar guardar uma alta quantidade de clientes e seus dados;
- O sistema deve tolerar guardar uma grande quantidade de produtos;
- O sistema deve acatar as regulações da LGPD;
- O sistema deve tolerar guardar uma alta quantidade de colaboradores;
- O sistema deve realizar as vendas, relatórios, controle de estoque e todas suas funções rapidamente;
- O sistema deve ser seguro  e privado.

# Diagrama de Atividades

![image](https://github.com/user-attachments/assets/f002c093-fc13-4561-977c-39e310bebb69)

# Diagrama de Casos de Uso

*&lt;Diagrama para visualizar o comportamento dos atores&gt;*

# Descrição dos Casos de Uso

*&lt;Descrição do comportamento entre os atores/resquisitos&gt;*

# Diagrama de Sequência

*&lt;Diagrama de ordem e interação dos objetos&gt;*

# Diagrama de Classes

*&lt;Diagrama de relacionamento entre classes para os seus atributos e operações&gt;*

# Diagrama de Estados

*&lt;Diagrama para permite modelar o comportamento interno de um determinado objeto, subsistema ou sistema global&gt;*

# Diagrama de Implantação

*&lt;Diagrama para exibir o relacionamento de hardware e software no projeto&gt;*

# Referências

*&lt;Lista de referências&gt;*
