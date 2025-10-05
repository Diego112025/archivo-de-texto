# Escritura de Archivo de Texto

# Abrimos el archivo en modo escritura ('w') -> crea el archivo si no existe
archivo = open('my_notes.txt', 'w')

# Escribimos al menos tres líneas de notas personales en el archivo
archivo.write("Primera nota: Recordar estudiar para el examen de matemáticas.\n")
archivo.write("Segunda nota: Comprar frutas y verduras el sábado.\n")
archivo.write("Tercera nota: Llamar a María para confirmar la reunión.\n")

# Cerramos el archivo después de escribir
archivo.close()

# Lectura de Archivo de Texto

# Abrimos el archivo en modo lectura ('r')
archivo = open('my_notes.txt', 'r')

# Leemos línea por línea utilizando readline() y mostramos cada línea
print("Contenido del archivo my_notes.txt:")
linea = archivo.readline()  # Lee la primera línea

# Bucle para leer hasta que no haya más líneas (cuando readline devuelve '')
while linea != '':
    print(linea.strip())  # strip() elimina el salto de línea para imprimir más limpio
    linea = archivo.readline()  # Lee la siguiente línea

# Cerramos el archivo después de leer
archivo.close()
