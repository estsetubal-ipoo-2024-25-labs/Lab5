# Lab 5 - Criação de Classes em Java. Documentação.

## Aplicações Java 

:dart: Desenvolva os seguintes programas com recurso ao IDE `IntelliJ IDEA`.

:warning: Crie os diferentes exercícios em projetos separadas.

:warning: Não se esqueça de guardar o seu trabalho!  

## Exercícios :pen:

1. Crie um projeto com uma classe `Product` que representa um produto de uma loja.

   :pencil2: Defina os atributos para armazenar o identificador do produto, a descrição, o preço e a quantidade em stock. 

   ​	:bulb: Todos os identificadores devem ser escritos em inglês.
   
   ​	:bulb: Considere tipos de dados apropriados para cada um dos atributos.
   
   ​	:bulb: Evidencie o conceito de encapsulamento.
   
    :pencil2: Crie um construtor que receba todos os atributos como parâmetro.

    :pencil2: Defina os métodos  `get` e `set` para todos os atributos.

    :pencil2: Deve criar um método `increasePrice (double)` que aumenta o preço do produto.

    :pencil2: Defina um método para vender um produto  `int sell(int)`que diminui a quantidade existente em stock. Caso a quantidade que se pretende vender seja superior à existente em stock, é vendida a quantidade em stock e retornada a quantidade que não foi possível vender. Caso a venda seja efetuada na sua totalidade o método retorna 0.
   
    :pencil2: Defina o método `toString`.
   
   
   
   
   📝Crie uma classe `Program` (método `main`) que:
   
   - Instancie 2 produtos
   - Mostre os produtos instanciados
   - Aumente o preço de um produto
   - Efetue a venda de um produto numa quantidade superior ao stock existente e outra venda, de um outro produto, com quantidade existente em stock para efetuar a totalidade da venda.
   - Mostre o estado atual dos dois produtos criados.
   
   

---

2. A direção da EST Setúbal decidiu criar um sistema informático para que fosse possível saber a informação e a localização dos serviços dentro do edifício da escola. Neste sentido foi necessário identificar  as salas da EST.

    :pencil2: Crie uma classe (`Room`), com os atributos para definir o bloco onde a sala se localiza (representado por uma letra), o piso (representado por um número), o número de sala e, por último, um atributo para saber se a sala é usada para serviços administrativos ou não.

     :pencil2: Crie um construtor que deverá inicializar os atributos (bloco, piso, número) com os valores recebidos . Faça a validação dos valores tendo em conta que o bloco é representado por uma letra entre A e F, o piso por um algarismo entre 1 e 3, o número por um valor entre 0 e 99. O valor do atributo administrativo indica se a sala é usada ou não para serviços administrativos. 
    
    ​	:bulb: Por defeito a sala é criada como não administrativa.
    
    ​	:bulb: Caso a validação falhe deverá ser lançada uma exceção ( `IllegalArgumentException`)
    
    
    
    :pencil2: Defina métodos `get` e `set`para os atributos administrativa e piso.
    
    :pencil2: Defina um método `getNome`. Este método deve retornar um texto com o nome da sala. O nome da sala deve ser construído a partir dos atributos e deve ter o formato <bloco><piso><numero>, ex: F104 para bloco F, piso 1, número 4.
   
   :pushpin: Faça a descrição da classe e do método  `getNome` com recurso ao **JavaDoc**. 
   
   📝Crie uma classe `Program` (método `main`) que:
   
   - Crie uma sala no bloco E, piso 2, com o número 3
   - Mostre a informação da sala no seguinte formato de texto: Sala <nome sala> ( ex: Sala E203 ).
   - Mostre numa outra linha: Sala administrativa ou Não é sala administrativa consoante o caso (faça uso de uma expressão ternária).
   
   

---

3. Crie um novo projeto e adicione  uma classe `CoffeeVendingMachine`. Esta classe irá gerir a venda de
café através de uma máquina de venda automática, bem como o stock dos seus componentes.

:pencil2: Defina atributos para a marca da máquina, para a capacidade máxima do
depósito de café , para o nível atual do depósito , para o número máximo de copos , para o número atual de
copos e para a quantidade de café consumida por copo .
:pencil2: Crie um construtor que recebe a marca da máquina, a capacidade máxima do depósito de café e,
ainda, o número máximo de copos. Inicialize o atributo que define a quantidade de café por copo com
o valor de 30 (ml). Os restantes atributos devem ser inicializados com o valor 0.
:pencil2: Crie métodos `get`para cada um dos atributos da máquina.
:pencil2: Crie um método que possibilite encher o depósito de café (`fillCoffee()`), que coloca o
nível de café igual à capacidade máxima do depósito. 

:pencil2: Crie um outro método que permita encher o stock de copos da máquina (`fillCups()`). Coloca o número de copos da máquina igual ao número máximo de copos.

:pencil2: Crie um método (` showStock()`) que mostre no ecrã as seguintes informações da
máquina:

<pre>Capacidade do depósito:         XXX ml</pre>
<pre>Nível do depósito:              XXX ml</pre>
<pre>Número máximo de copos:         XXX copos</pre>
<pre>Número de copos:                XXX copos</pre>



:pencil2: Crie um método que simule a tiragem de um café (`takeCoffee()`)
		:bulb: Deverá atualizar o nível de café disponível na máquina e decrementar o número total de copos.

:pencil2: Adicione um novo atributo que irá registar o número total de cafés vendidos (**soldCoffee**)
desde a última vez que a máquina foi abastecida, bem como o respetivo método `get`. Atualize o
método construtor para inicializar este atributo com o valor 0.
:pencil2: Adicione um método `resetSoldCoffee()`  que deverá de colocar o contador de cafés vendidos a zero.
:pencil2: Altere o método `takeCoffee()` para que passe a incrementar o número de cafés vendidos aquando da
tiragem de um café.

:pencil2: Adicione um novo atributo que identifica o preço por café (**coffeePrice**) e o seu respetivo
seletor. Atualize o método construtor para inicializar este atributo com o valor 0,40.
:pencil2: Crie um método (`printBalance()`) que imprime no ecrã o total de dinheiro em máquina
desde o último abastecimento.
:pencil2: Crie um método responsável pelo reabastecimento da máquina (`fillMachine()`) que
quando executa, deverá:

- Encher o depósito de café.
- Encher o número máximo de copos.
- Fazer reset ao número de cafés vendidos.



📝Crie uma classe `Program` (método `main`) e teste o código anteriormente criado, com a realização dos seguintes passos:

- Crie uma máquina de vendas, fornecendo a marca, a capacidade máxima do depósito de café e o número máximo de copos
- Encha o depósito do café e de copos
- Retire cafés
- Apresente a informação referente ao stock, após a execução dos passos anteriores
- Teste os restantes métodos, garantindo que todos os atributos são analisados.



---

paula.miranda@estsetubal.ips.pt e bruno.silva@estsetubal.ips.pt
