TDE de LFC

Equipe:
Bruno Cattalini
Felipe Mathieu
Lucas Kaniak

Instru��es de uso:
adicionar express�o no arquivo calculo.calc e us�-lo como entrada do programa.
a express�o adicionada precisa estar espa�ada: 1 + 2 + 3 + -4

express�o avaliada por linha sem declara��o � tipada por uma vari�vel default:
#/ calculo.calc
1 + 2 + 3 + 4
var x = 5 + 6

resultado:
Variavel> VALOR_EXPRESSAO
Valor> 10
Variavel> x
Valor> 11

Bugs conhecidos:
n�o est� reconhecendo vari�veis previamente declaradas na �rvore, portanto ela n�o �
avaliada na an�lise sint�tica.
ex:
var y = 2 + 2
var x = y + 4
resultado:
y> 4
x> 4

a preced�ncia dos operadores est� errada:
1 - 2 * 3 + 4 resulta -7