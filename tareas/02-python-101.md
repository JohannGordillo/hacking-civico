# Tarea 2 :books:

Para resolver la tarea usé el siguiente script en Python 3:

```
"""
==================================================
>> Autor: Johann Gordillo

>> Email: jgordillo@ciencias.unam.mx

>> Date:  13/09/2020
==================================================
Tarea #2 para el curso de Datos Abiertos y
Hacking Cívico de LAB León.
==================================================
"""

def densidad_poblacional(poblacion, area_ciudad):
    """Función que devuelve la densidad poblacional
    de una ciudad.

    Argumentos:
        poblacion (float): Número de habitantes.
        area_ciudad (float): Área en km^2 de la ciudad.

    Regresa:
        float: Densidad poblacional.
    """
    return poblacion / area_ciudad


def gasto_percapita(poblacion, presupuesto):
    """Cálcula el presupuesto per cápita para un
    sector determinado.

    Args:
        poblacion (float): Número de habitantes.
        presupuesto (float): Presupuesto en MXN.

    Returns:
        float: Presupuesto per cápita.
    """
    return presupuesto / poblacion


def main():
    """Función principal."""
    # Población al 2015 (INEGI).
    pob_mexico = 119938473
    pob_guanajuato = 5853677
    pob_moroleon = 50377

    # Área en km^2.
    area_mexico = 1964375
    area_guanajuato = 30608
    area_moroleon = 165

    # Densidad poblacional de México.
    densidad_mexico = densidad_poblacional(pob_mexico, area_mexico)

    # Densidad poblacional de Guanajuato.
    densidad_guanajuato = densidad_poblacional(pob_guanajuato, area_guanajuato)

    # Densidad poblacional de Moroleón.
    densidad_moroleon = densidad_poblacional(pob_moroleon, area_moroleon)

    print(f"Densidad poblacional de México: {densidad_mexico}\n")
    print(f"Densidad poblacional de Guanajuato: {densidad_guanajuato}\n")
    print(f"Densidad poblacional de Moroleón: {densidad_moroleon}\n")

    # Presupuesto para Vivienda y Servicios en Guanajuato.
    presupuesto = 2775000000

    gasto = gasto_percapita(pob_guanajuato, presupuesto)

    print(f"Presupuesto para Vivienda y Servicios en Guanajuato: ${gasto}\n")


if __name__ == "__main__":
    main()
```

Para resolver esta tarea, investigué en la página del INEGI y en la página de finanzas del Estado de Guanajuato.
