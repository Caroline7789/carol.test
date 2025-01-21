# carol.test
convenção de cor
import cv2

#Abrir a imagem
caminho_imagem = "test.png"
imagem = cv2.imread(caminho_imagem)

#Converter para tons de Cinza
imagem_convertida = cv2.cvtColor( imagem, cv2COLOR_BGR2GRAY )

#Guardar a Imagem
caminho_saida = caminho_imagem.replace(".png", "_cinza.png")
cv2.imwrite(caminho_saida, imagem_convertida)
     

import cv2

#Abrir a imagem
caminho_imagem = "test.png"
imagem_convertida = cv2.imread(caminho_imagem, cv2.IMREAD_GRAYSCALE)

#Guardar a Imagem
caminho_saida = caminho_imagem.replace(".png", "_cinza2.png")
cv2.imwrite(caminho_saida, imagem_convertida)
     
