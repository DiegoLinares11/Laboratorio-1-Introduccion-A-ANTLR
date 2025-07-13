# Laboratorio-1-Introduccion a ANTLR

## Descripción

Este proyecto implementa un analizador sintáctico utilizando ANTLR y Python.  
La gramática se define en `MiniLang.g4` y se prueba con un archivo de entrada `program_test.txt`.

## Estructura

- `MiniLang.g4`: gramática del lenguaje.
- `Driver.py`: archivo principal que ejecuta el analizador.
- `program_test.txt`: archivo de prueba.
- Archivos `.py` generados por ANTLR: `MiniLangLexer.py`, `MiniLangParser.py`, etc.

## Cómo ejecutar

Dentro de la carpeta lab1 correr:
```bash
pip install -r requirements.txt
```

Dirigirte a la carpeta program con
```bash
cd program
```
Luego 
```
java -jar (directorio) -Dlanguage=Python3 MiniLang.g4
```

Ejecutar el analizador
```bash
python Driver.py program_test.txt
```
Si el archivo es válido, muestra el árbol sintáctico.
Si hay errores, ANTLR los imprime en consola.

## Análisis

El archivo .g4 define la gramática del lenguaje con sus tokens y reglas.
El archivo Driver.py lee un archivo de prueba, tokeniza y parsea el contenido usando ANTLR.

## Video de demostración
[Ver video en YouTube](https://youtu.be/33GuEELrwKw)

