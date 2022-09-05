# Processamento de Imagens
&nbsp; &nbsp; Este PSET é um algoritmo de processamento de imagens feito em python.

## PSET-02
&nbsp; &nbsp; Este trabalho foi criado pelo aluno Roberto Bastos Souza, do curso de Ciência da Computação e turma CC3M da Universidade Vila Velha.
Professor: Abrantes

## Questão 01
&nbsp; &nbsp; O output esperado seria (4, 1, [226, 166, 119, 55]). Porque o filtro de inversão reflete os pixels sobre o valor de cinza médio, ou seja, 0 preto se torna 255 branco é vice-versa. Portanto, os parâmetros (4, 1, [29, 89, 136, 200]), quando colocadas no filtro de inversão, a lista de pixels de fica [226, 166, 119, 55], utilizando a fórmula 255-c, sendo C os pixels da imagem original.

## Questão 02
### Imagem do peixe invertido, utilizando a função "def invertido"
![peixe](https://user-images.githubusercontent.com/103335050/188286813-f38ab579-f87b-4120-907f-c4a5268588e7.png)
### Imagem do peixe original
![peixe](https://user-images.githubusercontent.com/103335050/188497482-4fe5a3de-5b33-4612-8fda-0c8426a9bf27.png)

## Questão 03
&nbsp; &nbsp; De acordo com a fórmula passada pelo abrantes:

    Ox,y =Ix−1,y−1 × k0,0 + Ix,y−1 × k1,0 + Ix+1,y−1 × k2,0+ (1) 
    Ix−1,y × k0,1 + Ix,y × k1,1 + Ix+1,y × k2,1+ (2) 
    Ix−1,y+1 × k0,2 + Ix,y+1 × k1,2 + Ix+1,y+1 × k2,2 (3)

&nbsp; &nbsp; Temos o valor:

0.00 x 80 = 0
-0,07 x 53 = -3, 71
0.00 x 99 = 0
-0.45 x 129 = -58.05
1.20 x 127 = 152.4
-0.25 x 148 = -37
0.00 x 175 = 0
-0.12 x 174 = -20.88
0.00 x 193 = 0

0 + (-3, 71) + 0 + (-58.05) + 152.4 + -37 + 0 + -20.88 + 0 = 32.76.

## Questão 04
### Imagem do porco empurrada para a diagonal inferior direita, utilizando a função "def correlation"
![porco](https://user-images.githubusercontent.com/103335050/188286769-4a112d5d-97f6-48b1-96e0-6e77da612572.png)
### Imagem do porco original
![porco](https://user-images.githubusercontent.com/103335050/188497580-90e691a4-17d5-463e-88cf-0a1a4652168a.png)

## Foto do gato desfocado
![gato](https://user-images.githubusercontent.com/103335050/188286781-42256b28-41a7-45db-8ebe-123f56fdb83c.png)
### Foto do gato normal
![gato](https://user-images.githubusercontent.com/103335050/188497636-5d323ee5-aae6-4f03-bea1-9f392e196234.png)

## Questão 05
### Questão escrita
&nbsp; &nbsp; Caso houvesse a necessidade de usar uma versão desfocada B que foi feita com um kernel de desfoque de 3 x 3, o cálculo seria

kn_1 = [[0, 0, 0],  
	      [0, 2, 0],  
	      [0, 0, 0]]
        
operação (-)
        
kn_2 = [[1/9, 1/9, 1/9],  
	      [1/9, 1/9, 1/9],  
	      [1/9, 1/9, 1/9]]
	           
&nbsp; &nbsp; Agora, subtraindo os pixels do kernel 1 (kn_1) pelos pixels do kernel 2 (kn_2) pelas suas respectivas posições, o resultado será 
 
 kn = [[-1/9, -1/9, -1/9],  
        [-1/9, 17/9, -1/9],  
        [-1/9, -1/9, -1/9]].
### Imagem da cobra nítida, utilizando a função de nitidez "def focado"
![python](https://user-images.githubusercontent.com/103335050/188286787-0c23e1b5-4ac2-48a4-8f03-492b4a458838.png)
### Imagem da cobra normal
![python](https://user-images.githubusercontent.com/103335050/188497659-00c9082b-5808-42ac-a50b-3d63800dc4a6.png)
## Questão 06
### Questão escrita
&nbsp; &nbsp; O Kernel Kx detecta as bordas pela horizontal, enquanto o Ky detecta as bordas pela vertical.

### Imagem da obra com detecção das bordas, utilizando a função "def bordas"
![obra](https://user-images.githubusercontent.com/103335050/188286817-7d03e458-4bdf-4abd-9ebb-cb6d26789506.png)

#### Imagem da obra com detecção das bordas pela horizontal 
![obra kx](https://user-images.githubusercontent.com/103335050/188499080-98d7cffc-6976-4b66-b878-883d1f61c5db.png)
#### Imagem da obra com detecção das bordas pela horizontal 
![obra ky](https://user-images.githubusercontent.com/103335050/188499105-e5aa9565-afd1-4f9a-b20c-41c882cfa00f.png)


