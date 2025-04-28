# Repo para EIEC – DevOps – UNIR

Este repositorio sirve para demostrar el uso de Git y pull-requests en la asignatura de EIEC. Incluye un script en Python que ordena listas de palabras y, opcionalmente, elimina duplicados.

---

## Contenido

- `main.py` : script principal en Python.  
- `Makefile` : atajos para ejecutar el script (con y sin Docker).  
- `words.txt` : ejemplo de lista de palabras (una por línea).

---

## Requisitos

- Python 3.6+  
- (Opcional) Docker  
- `make` en Linux/MacOS (en Windows, adapta los comandos o usa WSL)

---

## Uso

```bash
python3 main.py <filename> <remove_duplicates> <order>


filename	Ruta al fichero de texto con la lista de palabras (una por línea).
remove_duplicates	yes → elimina duplicados; no → conserva duplicados.
order	asc → orden ascendente; desc → orden descendente.

Ejecución de ejemplo

Con Docker (Makefile):
make run
# Ejecuta: python3 main.py words.txt yes asc



Directamente con Python:

python3 main.py words.txt yes desc



Salida esperada:

['gryffindor', 'hufflepuff', 'ravenclaw', 'slytherin']