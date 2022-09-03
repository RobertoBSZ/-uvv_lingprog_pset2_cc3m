# Processamento de Imagens
Este PSET é um algoritmo de processamento de imagens feito em python

## PSET-02
Este trabalho foi criado pelo aluno Roberto Bastos Souza, do curso de Ciência da Computação e turma CC3M da Universidade Vila Velha
Professor: Abrantes

## Questão 01
O output esperado seria (4, 1, [226, 166, 119, 55]). Porque o filtro de inversão reflete os pixels sobre o valor de cinza médio, ou seja, 0 preto se torna 255 branco é vice-versa. Portanto, os parâmetros (4, 1, [29, 89, 136, 200]), quando colocadas no filtro de inversão, a lista de pixels de fica [226, 166, 119, 55], utilizando a fórmula 255-c, sendo C os pixels da imagem original.
## Questão 02
imagens_salvas/peixe.png

## Questão 03
De acordo com a fórmula passada pelo abrantes: 
Ox,y =Ix−1,y−1 × k0,0 + Ix,y−1 × k1,0 + Ix+1,y−1 × k2,0+ (1) 
Ix−1,y × k0,1 + Ix,y × k1,1 + Ix+1,y × k2,1+ (2) 
Ix−1,y+1 × k0,2 + Ix,y+1 × k1,2 + Ix+1,y+1 × k2,2 (3)
Temos o valor:
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
imagens_salvas/porco.png

## Gato desfocado
imagens_salvas/gato.png

## Questão 05
