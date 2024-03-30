# Raycast
<h1>Amanda e Juliana</h1>
Criação de uma cena com aplicação do conceito de Raycast, Prefabs e Destroy.

# Desenvolvimento

## Conceitos aplicados
**Objetivo:**

- O código proporciona um controle de movimento para um objeto em um ambiente Unity.

**Entradas de Controle:**

- Utiliza as entradas do teclado ou de um controle para determinar o movimento horizontal e vertical do objeto.
- Input.GetAxis("Horizontal") é utilizado para movimento horizontal (esquerda e direita).
- Input.GetAxis("Vertical") é utilizado para movimento vertical (para cima e para baixo).

**Cálculo de Movimento:**

- Um vetor tridimensional (Vector3) é criado com base nas entradas de controle.
- O vetor de movimento é composto pelos componentes horizontal e vertical, juntamente com zero para o eixo Z (profundidade).

**Aplicação de Movimento:**

- A função Transform.Translate() é usada para mover o objeto.
- O movimento é calculado multiplicando o vetor de movimento pela velocidade e pelo tempo decorrido desde o último quadro (Time.deltaTime).
- Isso assegura que o movimento seja suave e independente da taxa de quadros.

![WhatsApp Image 2024-03-29 at 19 31 58](https://github.com/Amanda-Meneghin/Raycast/assets/127872372/3dff6387-c53b-4718-a7b1-5edbf9552ab3)

***

**Objetivo:**

- O código permite ao jogador destruir objetos em uma determinada camada ao clicar com o botão esquerdo do mouse.

**Controles:**

- O jogador deve clicar com o botão esquerdo do mouse para destruir objetos.

**Funcionalidade:**

- Um raio é lançado a partir da posição da câmera na direção do cursor do mouse.
- Se o raio atingir um objeto que pertença a uma camada específica (definida pela variável cubeLayer) dentro de uma distância especificada, o objeto é destruído.

**Variáveis Personalizáveis:**

- cubeLayer: Determina a camada dos objetos que podem ser destruídos pelo jogador.
- raycastDistance: Define a distância máxima para o raio de colisão.

![WhatsApp Image 2024-03-29 at 19 31 58 (1)](https://github.com/Amanda-Meneghin/Raycast/assets/127872372/405aec4c-9aa7-4bc0-895f-d62533c2b01f)

***

**Objetivo:**

- O código permite a destruição de um objeto no Unity quando clicado com o mouse.

**Funcionalidade:**

- O método OnMouseDown() é chamado automaticamente pelo Unity quando o usuário clica no objeto com o mouse.
- Dentro do método, a função Destroy(gameObject) é chamada, o que resulta na destruição do objeto ao qual o script está anexado.

![WhatsApp Image 2024-03-29 at 19 31 58 (2)](https://github.com/Amanda-Meneghin/Raycast/assets/127872372/dd4f7a6a-4507-45b2-bc10-73e6f5ee6ba4)
