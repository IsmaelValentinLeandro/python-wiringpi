## 1. INSTALAR WP

## FONTE
https://github.com/orangepi-xunlong/wiringOP-Python/tree/master

### 1.1. extrair o arquivo zip, copiar na pasta /home/wiringOP-Python e acessar
```
cd /home/wiringOP-Python
```
### 1.2. Atualizar sistema e instalar ferramentas
```
sudo apt update
```
```
sudo apt-get install swig python3-dev python3-setuptools
```
### 1.3. Compilar wiringpi-python
```
python3 generate-bindings.py > bindings.i
```
```
sudo python3 setup.py install
```
### 1.4. Testar wiringpi-python
Usage
=====

.. code:: python

    import wiringpi

    # One of the following MUST be called before using IO functions:
    wiringpi.wiringPiSetup()      # For sequential pin numbering

**General IO:**

.. code:: python

    wiringpi.pinMode(6, 1)       # Set pin 6 to 1 ( OUTPUT )
    wiringpi.digitalWrite(6, 1)  # Write 1 ( HIGH ) to pin 6
    wiringpi.digitalRead(6)      # Read pin 6

