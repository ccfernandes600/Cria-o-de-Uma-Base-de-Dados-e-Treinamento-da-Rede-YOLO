# Cria-o-de-Uma-Base-de-Dados-e-Treinamento-da-Rede-YOLO

Para realizar este projeto  utilizei a rede YOLO, disponível em: https://pjreddie.com/darknet/yolo/.
# Passo a passo:
# Detecção usando um modelo pré-treinado
Clonei o resoitório https://github.com/pjreddie/darknet para meu destktop com linux Mint 21.3 com anaconda instalado. Entrei no diretório *darknet* e madei compilar o código clonado com o comando *make*

<div style="border: 1px solid #ddd; padding: 10px; background-color: #f9f9f9;">
<pre><code class="bash">
git clone https://github.com/pjreddie/darknet
cd darknet
make
</code></pre>
</div>






# Baixar o arquivo de peso pré-treinado (237 MB).
<div style="border: 1px solid #ddd; padding: 10px; background-color: #f9f9f9;">
<pre><code class="bash">
wget https://pjreddie.com/media/files/yolov3.weights
</code></pre>
</div>



# Exeutar a detecção

Use uma das figuras que estão no diretório data ou baixe alguma da internet para este diretório e execute o seguinte comando passando o nome da figura a ser analisada
<div style="border: 1px solid #ddd; padding: 10px; background-color: #f9f9f9;">
<pre><code class="bash">
./darknet detect cfg/yolov3.cfg yolov3.weights data/dog.jpg
</code></pre>
</div>


Usei esta figura do cacchoro que já estava disponível no diretório data e baixei mais duas figuras da internet. Uma da av paulista com carros e ônibus e outra de carros e pesssoas e uma maca com uma pessoa provalvelmente morta.

# Resultados
## Fotos de entrada:
1. Fotos da Av Paulista ![Av Paulista](av_paulista.jpg)
2. Foto com Cacchoro e Bicicleta ![Chacacho e Bicicleta ](dog.jpg)
3. Foto de uma morte num Motel ![Morrte no Motel](morte_motel.jpg)


## Fotos processadas pelo yolo v3
1. Fotos da Av Paulista processada ![Av Paulista](av_paulista_predição.jpg)
2. Foto com Cacchoro e Bicicleta processada ![Chacacho e Bicicleta ](dog_predição.jpg)
3. Foto de uma morte num Motel procesada ![Morrte no Motel](motel_predição.jpg)



