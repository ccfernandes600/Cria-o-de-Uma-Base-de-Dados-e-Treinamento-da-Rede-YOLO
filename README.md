# Cria-o-de-Uma-Base-de-Dados-e-Treinamento-da-Rede-YOLO

Para realizar este projeto  utilizei a rede YOLO, disponível em: https://pjreddie.com/darknet/yolo/.
# Passo a passo:
# Detecção usando um modelo pré-treinado
Clonei o resoitório https://github.com/pjreddie/darknet para meu destktop com linux Mint 21.3 com anaconda instalado. Entrei no diretório *darknet* e madei compilar o código clonado com o comando *make*

git clone https://github.com/pjreddie/darknet
cd darknet
make


# Baixar o arquivo de peso pré-treinado (237 MB).

wget https://pjreddie.com/media/files/yolov3.weights


# Exeutar a detecção

Use uma das figuras que estão no diretório data ou baixe alguma da internet para este diretório e execute o seguinte comando passando o nome da figura a ser analisada

./darknet detect cfg/yolov3.cfg yolov3.weights data/dog.jpg


Usei esta figura do cacchoro que já estava disponível no diretório data e baixei mais duas figuras da internet. Uma da av paulista com carros e ônibus e outra de carros e pesssoas e uma maca com uma pessoa provalvelmente morta.

# Resultados


