# spanish2datetime

## Description
Python3 script able to turn spanish text into datetime.

## Installation (On work)

If you already have [Python3](http://www.python.org/) on your system you can install the library simply by downloading
the distribution, unpack it and install in the usual fashion:

```bash
python3 setup.py install
```

You can also install it using a popular package manager with

```bash
pip3 install spanish2datetime
```

or

```bash
easy_install spanish2datetime
```

## Dependencies

- There is no dependencies but Python3.

## Quick Start

To get started, simply install spanish2datetime import spanish2datetime and use it:
```python
from spanish2datetime import spanish2datetime

for example in ['Hoy', 'Mañana por la mañana', 'Esta tarde', 'Ayer a las seis y media', 'El viernes '
                'que viene a las ', 'nueve de la noche', 'Dentro de dos semanas y cuatro días a las '
                'ocho y media de la tarde', 'Dentro de', 'Mañana a las cinco de']:
    print(example + ': ' + str(spanish2datetime(example.lower().split(' '))))
    
    

>>> 'Hoy: 2018-05-15 13:51:48'
>>> 'Mañana por la mañana: 2018-05-16 07:00:00'
>>> 'Esta tarde: 2018-05-15 14:00:00'
>>> 'Ayer a las seis y media: 2018-05-14 06:30:00'
>>> 'El viernes que viene a las nueve de la noche: 2018-05-18 21:00:00'
>>> 'Dentro de dos semanas y cuatro días a las ocho y media de la tarde: 2018-06-02 20:30:00'
# Dentro de
>>> TypeError: Error procesando [en/dentro de] [n] [años/año/meses/mes/semanas/semana/días/día/horas/hora
              /minutos/minuto/segundos/segundos]
# Mañana a las cinco de
>>> TypeError: Mañana a las cinco de: Error procesando [de] [la] [mañana/tarde/noche]
```
## Documentation (On work)

https://spanish2datetime.readthedocs.io/en/latest/

## Reporting Issues

If you have suggestions, bugs or other issues specific to this library, file them [here](https://github.com/msolefonte/spanish2datetime/issues). Or just send me a pull request.

## Version

- 1.0 - 15/05/2018 - Initial release.
