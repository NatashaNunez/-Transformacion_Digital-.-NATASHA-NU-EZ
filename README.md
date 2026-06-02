# -Transformacion_Digital-.-NATASHA-NU-EZ
El tema es "calcular el promedio de una lista de números". 
def calcular_promedio(numeros):
    """
    Calcula el promedio aritmético de una lista de números.

    Parameters
    ----------
    numeros : list
        Lista de valores numéricos (int o float). 
        No debe estar vacía.

    Returns
    -------
    float
        El promedio aritmético de los elementos de la lista.

    Raises
    ------
    ValueError
        Si la lista está vacía.

    Examples
    --------
    >>> calcular_promedio([10, 20, 30])
    20.0
    >>> calcular_promedio([5, 7, 3, 9])
    6.0
    """
    if not numeros:
        raise ValueError("La lista no puede estar vacía.")
    
    total = sum(numeros)
    cantidad = len(numeros)
    promedio = total / cantidad
    
    return promedio


# --- Ejemplo de uso ---
if __name__ == "__main__":
    datos = [85, 90, 78, 92, 88]
    resultado = calcular_promedio(datos)
    print(f"El promedio de las calificaciones es: {resultado:.2f}")
