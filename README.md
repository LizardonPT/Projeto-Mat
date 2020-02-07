# 1º Commit:
- Após dedicar algum tempo a ler o código e a percebe-lo, apercebemo-nos de que tinhamos que trabalhar no ficheiro mesh.py para alterar-mos o cubo que já estava desenhado.

- Dentro da função "create_cube" entre as linhas 38 e 45 está o código que define as faces do cubo já desenhado, então, decidimos experimentar mexer no código e ao tirar as linhas de código que definem as faces com valores inversos para reduzirmos as faces de 6 para 3. Mas só isso não basta para transformar o cubo numa piramide triângular, tivemos que retirar um vértice de cada face desenhada, para isso apenas tivemos de apagar a linha de código nº57 que retira os valores do "axis0" e do "axis1" à origem do anterior quadrado. Se tivessemos tirado as linhas 38, 41 e 44, tinhamos de tirar a linha que adiciona os valores de "axis0" e "axis1" em vez da que os retira. Com isto desenhamos as nossas 2 pirâmides triângulares, pois a 2ª pirâmide é desenhada em funcão da 1ª.
- O passo seguinte foi introduzir os controlos para o movimento no ficheiro mysample.py que replicamos do sample.py para evitar perder a base do códige caso algo inesperado acontecesse.
- Para dar a ilusão de que a camera se mexe de acordo com os controlos w, a, s, d, intoduzimos condições "if" que movem as pirâmides no sentido oposto da tecla pressionada pelo usuário.
- Para as rotações em torno dos eixos x, y e z, criamos 3 variáveis com valores de vetores unitários ((1,0,0), (0,1,0), (0,0,1)) para introduzir no codigo que faz os calculos para a rotação em função do vetor itroduzido. Juntado esta parte de código com as condições "if" ficou definido as teclas pedidas para a rotação dos objetos.

# 2º Commit:
- Adicionamos um ficheiro chamado FPV.py para fazer o programa estilo "FPS"
- Usamos novamente o codigo já feito no mesh.py para adicionarmos mais uns cubos ao cenário.
- Já se consegue mover a camera pelo cenário através de condições "if" que verificam se as teclas são pressionadas.
- Falta adicionar o movimento da visão da camera que será controlado pelo motion do rato e falta também fazer com que o programa não renderize nada para trás da visão do usuário, pois caso aconteça o programa crasha.