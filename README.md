# Raycast
<h1>Amanda e Juliana</h1>
Criação de uma cena com aplicação do conceito de Raycast, Prefabs e Destroy.

# Desenvolvimento

## Conceitos aplicados
Objetivo:

-O código proporciona um controle de movimento para um objeto em um ambiente Unity.

Entradas de Controle:

-Utiliza as entradas do teclado ou de um controle para determinar o movimento horizontal e vertical do objeto.
-Input.GetAxis("Horizontal") é utilizado para movimento horizontal (esquerda e direita).
-Input.GetAxis("Vertical") é utilizado para movimento vertical (para cima e para baixo).

Cálculo de Movimento:

-Um vetor tridimensional (Vector3) é criado com base nas entradas de controle.
-O vetor de movimento é composto pelos componentes horizontal e vertical, juntamente com zero para o eixo Z (profundidade).

Aplicação de Movimento:

-A função Transform.Translate() é usada para mover o objeto.
-O movimento é calculado multiplicando o vetor de movimento pela velocidade e pelo tempo decorrido desde o último quadro (Time.deltaTime).
-Isso assegura que o movimento seja suave e independente da taxa de quadros.
