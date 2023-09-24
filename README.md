# Obtener la palabra o frase y la letra a ocultar desde el usuario
palabra_frase = input("Ingrese una palabra o frase: ")
letra = input("Ingrese la letra que desea ocultar: ")

# Inicializar una cadena vacía para almacenar el resultado
resultado = ""

# Iterar a través de cada letra en la palabra o frase
for caracter in palabra_frase:
    # Comprobar si el caracter actual es igual a la letra a ocultar (ignorando mayúsculas/minúsculas)
    if caracter.lower() == letra.lower():
        resultado += '*'  # Si es igual, añadir un asterisco al resultado
    else:
        resultado += caracter  # Si no es igual, añadir el caracter original al resultado

# Mostrar el resultado
print("Resultado:", resultado)
