O objetivo deste patch é analisar a entrada de áudio (adc)
e colher alguns valores (Freq, Amplitude, Tempo) e a partir 
destes gerar cores.
Também podem ser feitas adaptações para posicionamento de imagens 
ou o que se quiser com os valores de entrada.


Instruções:

1) Instalar a lib aubio no Ubuntu (14.04)

Forma mais fácil:
sudo apt-get install pd-aubio

ou se quiser compilar -> https://aubio.org/pd-aubio/download

Se usar pd-extended adicionar a biblioteca 
a lista em Edit -> Preferences -> New...

2) ao iniciar o pd pela linha de comando, carregue a lib aubio:
luiz@luiz-ubxps:/$ pd -lib aubio

Para evitar problemas de ruído é importante
abrir cada arquivo em uma nova instância do pd.


Obs. Este é um código bem experimental e apresenta muita 
instabilidade. 
Recomenda-se o uso de uma interface de áudio externa 
e também gerenciar o áudio via Jack. (http://www.jackaudio.org/)




