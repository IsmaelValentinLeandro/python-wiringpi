## INSTALAR WP
```
# extrair o arquivo zip, copiar na pasta /home/ 
Acessar pasta /home/wiringOP-Python
# cd /home/wiringOP-Python
Atualizar sistema e instalar ferramentas
# sudo apt update
# sudo apt-get install swig python3-dev python3-setuptools
Compilar wiringpi-python
# python3 generate-bindings.py > bindings.i
# sudo python3 setup.py install
import wiringpi

# One of the following MUST be called before using IO functions:
wiringpi.wiringPiSetup()      # For sequential pin numbering
General IO:

wiringpi.pinMode(6, 1)       # Set pin 6 to 1 ( OUTPUT )
wiringpi.digitalWrite(6, 1)  # Write 1 ( HIGH ) to pin 6
wiringpi.digitalRead(6)      # Read pin 6
```
