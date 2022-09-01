# Treinando--Python-
Treinando comandos básicos do Python(Leia o README para explicações)
Para treinar, pesquisei alguns comandos extras e em conjunto, para assimilar melhor, tenho o hábito de digitar na terceira pessoa, como se estivesse alguém me explicando. 
É uma mania, minha. Assim, vou colocar abaixo todos os comentários que fiz para aprendizado e entendimento do funcionamento. 

Lembrando que os comentários estão em ordem para melhor assimilar a leitura com a visualização do código.


 # No Python podemos criar um sorteio de números usando o comando RANDOM, onde nele definiremos uma condicional de sorteio máximo até 100, ficando assim:
        #random()*100
    # para usar o RANDOM, precisamos na primeira linha efetuar o "import random"
    #Porém, o RANDOM sorteia números de todos os tipos, seja INT ou FLOAT. Aí, usaremos em conjunto da chamada a palavra ROUND - também poderíamos usar INT e seria
    # indiferente -, mas optamos apenas por usar o ROUND, ficando assim:
        #numero_secreto = round(random. random() * 100)
    # AGORA, para facilitar e não precisar efetuar a chamada com ROUND, podemos usar outro comando do RANDOM que é o RANDOM.RANDRANGE que ele
    #sorteia números inteiros de 0 a 100. No comando devemos colocar de 1 a 101, conforme determinação da documentação do Python.
        #RESULTADO: numero_secreto = random.randrange(1, 101)

# Agora, modificaremos um pouco o jogo e daremos ao usuário a escolha de 3 níveis: fácil, médio, difícil, e de acordo com a escolha do usuário, ele terá
    # 20 tentativas, 10 tentativas e 5 tentativas em fácil, médio e difícil, respectivamente.
    #Para registro deste input, transformaremos ele em inteiro, na variável NIVEL
    # Como faremos uma condição para esta escolha do usuário, denominaremos que o valor da variável total_de_tentativas é 0 e ela mudará conforme as condições que daremos

    # rodada = 1

    # para comentar é só apertar CTRL + /kbd INPUT é para o usuário digitar o número-chave. Assim, criamos a variável
    # chute com o comando de INPUT e logo abaixo, aparecerá a mensagem com o número chutado pelo usuário
    # Precisamos transformar a variável chute em chute_str, uma vez que o python dará erro, no momento de comparação, mesmo que o usuário digite o número correto,
    # visto que o 42 é um "int" e o digito de input é "string"
    #Criamos a variável TOTAL_DE_TENTATIVAS para executar o comando WHILE e com ele limitar quantidade de chutes.
    # Criamos a variável RODADA para informar ao usuário a rodada que ele está jogando e também somar ao final do ELIF  a RODADA + 1 e o programa
    #  o WHILE permanecerá rodando enquanto o número de rodadas for menor do que o total_de_tentativas
    # Faremos uma STRING INTERPOLATION: que é adicionar o comando ".format" no primeiro PRINT após o WHILE, para que ele automatize a contagem do número
    # de rodadas e do total_de_tentativas. Assim, chamaremos estas variáveis através de colchetes {}

    # NOVA SITUAÇÃO: inicialmente o exemplo dado fora para usar o WHILE. Contudo, também podemos usar o FOR. Assim, comentaremos o WHILE abaixo e substituiremos
    # por uma chamada em FOR
    # ANTES: Agora que usaremos FOR a variável rodada, acima, não será mais necessária, uma vez que o comando for começará pelo comando RANGE que dará uma condição de
    # contagem.
    # SOBRE O RANGE: podemos determiná-lo com uma chamada de contagem de 1 a 10, por exemplo, ou podemos também adicionar uma condição de contagem de 1, 10, 2, por exemplo
    # onde os números de contagem começam no 1 e acabam no 10, mas será uma contagem de 2 em 2 números. Aí ficaria: 1, 3, 5, 7, 9
    # Também apagaremos o comando bem abaixo (deixarei comentado)     rodada = rodada + 1, uma vez que o FOR já faz este laço de repetição para nós, quando determinamos
    # no "rodada in range" que ele fará rodagem de 1 em 1.
    # LEMBRANDO: adicionamos o total_de_tentativas + 1, uma vez que teríamos apenas duas rodadas. Aí com o FOR daremos que ele rodará o total_de_tentativas + uma rodada
    # COMO ERA O WHILE: while( rodada <= total_de_tentativas):
    # AGORA COM O FOR:

#Agora, criamos uma variável CHUTE e informamos ao python que o chute é igual ao número inteiro, informado na string chutr_str. Ou seja, fizemos uma conversão
    # criamos um IF para que o usuário digite apenas um número entre 1 e 100 e que caso ele digite, o jogo não elimine uma jogada. Assim, haverá a mensagem
    #informando o erro e logo em seguida o CONTINUE fará com que o FOR prossiga com sua repetição normal
    #Para condição de análise, o python usa OR e AND, ao invés de || e &&
    # Condicional para comparar se o número digitado é o correspondente da variável numero_secreto todo IF t em um ELSE.
    #  Contudo, poderá existir apenas um ELSE. Assim, no ELSE, em caso de existência de novas verificações de
    #  condicionais podemos usar o comando ELIF. Assim, adicionamos um IF dentro do ELSE e por fim adicionamos um ELIF,
    #  sendo ele um novo ELSE. Repare que também criamos três variáveis com o com os comandos de verificação do chute,
    #  se ele é igual, maior ou menor do que o numero_secreto
    # O BREAK é para quebrar o laço de repetição quando o IF for verdadeiro e impedir que o jogo fique rodando + 2 rodadas, mesmo acertando
     # Trabalharemos com pontuação para interagir mais com o usuário. Assim, a cada chute errado, o usuário terá um início com 1000 pontos (criamos a variável pontos)
    # A cada chute errado, o usuário terá a diminuição dos seus pontos, com o valor da distância do chute até o número correto.
    # Como poderíamos ter casos em que o usuário poderia chutar 60 e o número fosse 40, ficaria como 60 + 40 = 20, ele teria um acréscimo de pontuação. Então
    # para evitar isso, usaremos o comando ABS que é um cálculo ABSOLUTO e impede um número negativo.
    # No final, quando o usuário acertar/se acertar, terá o final uma mensagem informando quantos pontos ele fez no total.
