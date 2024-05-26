# 7.3 Tareas

1-Las funcionalidades que presenta el compilador las busque mediente el comando "gcc --help". Las relacionadas a la limitacion del inicio y fin de las fases de traducción son las siguientes:

     -E                       Preprocess only; do not compile, assemble or link.
     -S                       Compile only; do not assemble or link.
     -c                       Compile and assemble, but do not link.

# 7.3.1. Secuencia de Pasos


1- B- Comando utilizado : "gcc .\hello2.c -E -o hello2.i"

    Resultado:
        Se genero el archivo "hello2.i"

    Error:
        Ninguno

    Analisis
        Si bien el archivo tiene escrita la funcion "prontf" que no se encuentra definida, se puede precompilar. A la hora de precompilar la funcion "prontf" se mantiene y no se reemplaza por nada. No se detecta el error de la falta del "}" al final del codigo. Se agrega al codigo las lineas correspondientes al "#include <stdio.h>"
    