# Projeto de Software Revenda de Veículos

O objetivo do presente trabalho é projetar um sistema para controle de revenda de Veículos. Mas como funciona uma revenda de Veículos? Os dados do cliente são lançados no sistema, juntamente com o veículo que se deseja vender e as características do automóvel. Cada veículo tem uma marca, um modelo e uma cor, além de seus respectivos atributos e acessórios.

Os clientes que desejam comprar um veículo (“clientes pretendidos”) também são cadastrados no sistema, juntamente com o veículo de sua preferência. Com base nos dados cadastrados, podemos efetuar buscas para localizar um veículo de acordo com características dele.

No final do mês cada vendedor será remunerado de acordo com a quantidade de vendas efetuadas multiplicada pela sua respectiva comissão sobre o valor da mesma. Convencionamos que a comissão do vendedor para qualquer venda é 5% sobre o valor da mesma.

## Entidades envolvidas no projeto:

1. A entidade principal do projeto é o Veículo, que pode ser classificado como Veiculo_Pretendido, Veiculos_Adquirido e Veiculo_Atual. Sendo o Veiculo_Atual aquele que o cliente deseja vender. Veiculos_Pretendido aquele que deseja adquirir e o Veiculo_Adquirido aquele efetivamente adquirido que pode ser ou não o pretendido.
2. Veículos possuem Modelos, que são descritos pelos seus nomes;
3. Modelos possuem Marcas, que são descritas pelos seus nomes.
4. Veículos possuem um conjunto de Acessórios, que são descritos pelos seus nomes.
5. Cliente compra e vende veículos. Desta forma possui um tipo (vendedor, comprador ou vendedor/comprador).
6. O funcionário vendedor será identificado pela sua matrícula e pelo seu nome.
7. Clientes e Funcionários são subclasse da classe Pessoa. Uma pessoa possui nome, CPF, data de nascimento, sexo, endereço, formas de ser contatado como e-mail e telefone.
8. O Endereco é composto do tipo (rua, avenida, alameda, etc), nome, número, complemento, bairro, cep, cidade, estado). O endereço deve ser persistido no sistema, porém os dados devem ser obtidos através de consulta ao WebServices dos Correios. Caso o endereço não exista nos correios, o sistema deve permitir o cadastramento do mesmo.
9. Cada venda efetuada deve informar a data que foi efetuada, o valor, qual o veículo, o cliente_vendedor, o cliente_comprador e o funcionario_vendedor).
10. No final do mês deverá ser gerado: um relatório com o valor da remuneração de cada funcionario_vendedor e um relatório de vendas, classificados por funcionario_vendedor, cliente_vendedor, cliente_comprador.

## No repositório contém as pastas com cada etapa do projeto a ser desenvolvido durante a disciplina de projeto de software.
