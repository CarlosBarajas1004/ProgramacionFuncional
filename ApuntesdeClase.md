# Barajas Cortes Carlos Alejandro, Semestre 3 grupo B, Facultad de Ingenieria Mecanica y Electrica, Ingenieria en computacion inteligente, Universidad de Colima
## Apuntes realizados en clases de Programacion funcional en lenguaje python
### Operadores logicos
```python
True
False
if 5 > 4:
    print(True)
print(5>7)
 
received: bool = False
not received
```

```python
nombre: str = 'hugo'
print(nombre)
print(type(nombre))
nombre.capitalize()
nombre.upper()
```
```python
num: int = 10
pi: float = 3.14
es_alumno: bool = True
name: str = 'Hugo'
print(f'{num}--{pi}--{es_alumno}--{name.upper()}')
```
```python
print(True and False)
print(True or False)
print(not False)
````

### Operadores Aritmeticos
```python
print(5+4)
print(5-4)
print(5*4)
print(5/4)
print(5//4) # division entera
print(5%4) # modulo o residuo
print(5**4) # x a la y
```

### Condicionales
```python
n1: int = 30
n2: int = 20
if n1>n2:
    print(f'{n1} > {n2}')
```
```python

n1=10
if n1>n2:
    print(f'{n1} > {n2}')
else:
    print(f'{n2} > {n1}')
```

```python
edad: int = 18
if edad > 18:
    print('mayor de edad')
elif edad == 18:
    print('acabas de llegar a la mayoria de edad')
else:
    print('eres menor de edad')
```

```python
match True:
    case 18:
        print('acabas de llegar a la mayoria de edad')
        case edad
```
### Tipos de datos
```python
mensaje: str = "Hola"             #Las mayusculas estan designadas para las clases
numero: float = 3.1416
otro_numero: int = 15    
apellido_paterno = " "
apellidoPaterno = "Asi no se hace nunca en python"
```

```python
#num = ""
n = int(input("Dame un numero entero positivo"))
if n%2 == 0:
    num = "Par"
else:
    num = "Impar"
    
num
```

```python
n = int(input("Dame un numero entero positivo"))
(num := "Par" if n%2 == 0 else "Impar")
num
```

```python
(num := "par" if int(input("dame un numero entero posaitivo"))%2 == 0 else "impar")
num
```

```
suma = a+b
```

```python
#Casting
#conversion de tipos
num_str = "3"
num_int = int(num_str)
print(f"num_int: {num_int}") #fstrings

num_float = 3.14
num_int = int(num_float)
print(f"num_int: {num_int}")

def res():
    num_str = "3"
    num_int = 10
    return (num_str, num_int)

num_str = str(num_float)
res_tupla = (num_str, num_int)
print(f"num_str: {res()}")
print(f"res: %s %d" % res())
num_str

a, b = res()
print(f"res: {a} {b}")
```
### Logicos Bool
```python
True
False
if 5 > 4:
    print("True")
    
print(5>7)

received: bool = False
not received
```

### Cadena String
```python
nombre: str = "alex" #Python es un lenguaje interpretado
nombre #Compilados manejan mejor la memoria
print(type(nombre)) #Todas las clases tienen propiedades y tienen objetos
nombre.capitalize()
nombre.upper()
```

```python
num: int = 10
pi:float = 3.14
es_alumno: bool = True
name:str = "Alex"

print(f"{num}-{pi}-{es_alumno}-{name}")
```

### Listas
```python
# Listas 
# Colecciones (colections)

def suma(a, b):
    return a + b 
def resta(a, b):
    return a - b
def multiplicacion(a, b):
    return a * b
def division(a, b):
    return a / b

operaciones = [suma, resta, multiplicacion, division]
print(operaciones[0](5,4))
print(operaciones[1](5,4))
print(operaciones[2](5,4))
print(operaciones[3](5,4))

for operacion in operaciones:
    print(operacion(5, 4))

Lista = [1, 2, 3, 4, 5, True, 4.5, "hola", [1, 2, 3]]
```
```python
# La lista es indexable osea que todos los valores tienen posicion y son mutables y pueden contener cualquier tipo de dato
Lista[8]
```

```python
Lista[8]="Hola mundo"
Lista
```
```python
#slices
print(Lista)
print(Lista[:])
```

```python
print(Lista[0:])
```

```python
print(Lista[:-1])
```

```python
def suma(a, b): #una funcion siempre debe de retornar algo, una caracteristicas de las listas
    pass

print(suma(3, 4))
```

```python
def operaciones(a, b):
    return [a+b, a-b, a*b, a/b]

respuestas = operaciones(5, 4)
print(respuestas)
w, x, y, z = operaciones(5, 4)
print(w)
```

```python
res_suma,_,_,_ = operaciones(5, 4)
res_suma
```

```python
lista = [3, 6, 7, 40, 34, 67, 89]
max(lista)
```

```python
sum(lista)
min(lista)
sorted(lista)
lista.sort()
lista
print(lista.sort())
lista.sort(reverse=True)
lista
```

### Set
```python
# set conjuntos en python asi podemos eliminar los elementos repetidos en orden 1

mi_set = {1, 2, 3, 3, 3, 3, 3}
mi_set
```

### Data
```python
data = [15, 14, 13, 12, 11, 10, 1, 2, 3, 4, 5, 6, 7, 8, 9, 1, 2, 1, 2, 1, 2, 1, 2, 1, 2]

set(data) #datos no repetidos en una misma linea en orden 1
```

```python
data2 = {1, 56, 57, 58}

mi_set.union(data2)
```

### Diccionarios
```python
# diccionarios
mi_dict = {"llave": "valor"}
mi_dict["llave"]
```

```python
mi_dict.keys()
```

```python
mi_dict.values()
```

```python
do a dict
```

### Tuplas
# Tuplas tuple son inmutables, no puedes cambiarle los datos
```python
tupla_funciones = (suma, resta , multiplicacion, division)
print(tupla_funciones[1](5, 4))

tupla = (1, 2, 3, 4, 5, True, 4.5, "hola" , [1, 2, 3])
```

```python
Lista.append[10]
Lista

```
```python
tupla.__add__((10,10))
tupla[0].__mod__(2)
```

```python
def suma(a: int, b: int) -> int:
    return a + b 

def operacion(a: int, b: int) -> (int, int):
    return (a+b, a-b)

(a, b) = operacion(5, 6)
a,b = operacion(6, 5)
print(a, b)
```

### Uso de range
```python
#range

numeros = range(10)
print(numeros)
```

```python
for i in numeros:
    print(i, end="")
```

```python
numeros = range(5, 10)
```

```python
for i in numeros:
    print(i, end=",")
```

```python
numeros_pares = range (2,11,2)
for par in numeros_pares:
    print(par, end=" ")
```

```python
for item in range(2,11,2):
    print(item, end=" ")
```

### Funcion suma y resta
```python
def suma(a: int, b: int)->int: #pistas
    return a + b

if __name__== "__main__":
    print(suma(5,6))
    
```

```python
def resta(a: int, b: int)-> int:
    return a + b

if __name__== "__main__":
    print(resta(8,4))
```
#### Importamos la carpeta en la que se encuentran ambas funciones
```python
""" import milibreria.suma as lib
import milibreria.resta as lib """
""" import milibreria as lib """
from milibreria import suma, resta

def suma1(a: float, b:float)->float:
    return a + b

def suma2(a: float, b:float)->float:
    return a + b

def suma(a: int|float, b:int|float)-> int|float:
    return a + b

if __name__== "__main__":
    print(suma(5,6.5))
    print(suma1(5,6))
    print(suma2(5.3,6.4))
```

### Uso de streamlit en python
#### Uso de @dataclass
#### Agenda hecha en python usando streamlit
```python
# funcion decorador se utiliza para modificar el comportamiento de otra funcion

from dataclasses import dataclass

@dataclass #decorators
class User:
    id: str
    name: str
    age: int

    def show_data(self):
        return f"ID: {self.id}\nNOMBRE: {self.name}\nAÑO: {self.age}"

if __name__ == "__main__":
    usuario1 = User("1","CARLOS",25)
    usuario2 = User("2","ALEJANDRO",25)
    usuario3 = User("3","BARAJAS",25)
    usuario4 = User("4","CORTES",25)
    usuarios = [usuario1,usuario2,usuario3,usuario4]
    for usuario in usuarios:
        print(usuario.show_data())
```
#### Calculadora hecha en python haciendo uso de streamlit
```python
import streamlit as st
st.sidebar.title("CALCULADORA ICI")

def pedir_valores():
    name = st.text_input("NOMBRE: ")
    n1 = st.number_input("NUMERO 1")
    n2 = st.number_input("NUMERO 2")

    if st.button("SUMAR"):
        st.success(f"HOLA {name}")
        st.write(f"{n1} + {n2} = {n1+n2}")
    elif st.button("RESTAR"):
        st.success(f"HOLA {name}")
        st.write(f"{n1} - {n2} = {n1-n2}")
    

opcion = st.sidebar.selectbox("opciones:",[
    "SUMA","RESTA","MULTIPLICACION","DIVISION","ACERCA DE"
])

match opcion:
    case "SUMA":
        st.write("ESTA ES LA SUMA DE...")
        pedir_valores()
    case "RESTA":
        st.write("ESTA ES LA RESTA DE...")
        pedir_valores()
    case "MULTIPLICACION":
        st.write("ESTA ES LA MULTIPLICACION DE...")
    case "DIVISION":
        st.write("ESTA ES LA DIVISION DE...")
    case "ACERCA DE":
        st.write("DERECHOS RESERVADOS")
        st.write("UCOL-FIME-ICI")
```

### Proyecto de parcial en el cual se pidio realizar una base de datos en streamlit en la que se almacenen estudiantes, profesores y directivos en el cual se puedan realizar las operaciones crud (create, read, update and delete)
```python
import streamlit as st
import pickle

# Definición de la clase base para personas en la escuela
class Escuela:
    def __init__(self, nombre, edad, correo):
        self.nombre = nombre
        self.edad = edad
        self.correo = correo
        
       
        
    def get_nombre(self):
        return self.nombre

    def set_nombre(self, nuevo_nombre):
        self.nombre = nuevo_nombre

    def get_edad(self):
        return self.edad

    def set_edad(self, nueva_edad):
        self.edad = nueva_edad

# Definición de la clase para estudiantes que hereda de Escuela
class Estudiante(Escuela):
    def __init__(self, nombre, edad, correo, carrera):
        super().__init__(nombre, edad, correo)
        self.carrera = carrera

# Definición de la clase para profesores que hereda de Escuela
class Profesor(Escuela):
    def __init__(self, nombre, edad, correo, area):
        super().__init__(nombre, edad, correo)
        self.area = area

# Definición de la clase para directivos que hereda de Escuela
class Directivo(Escuela):
    def __init__(self, nombre, edad, correo, cargo):
        super().__init__(nombre, edad, correo)
        self.cargo = cargo

# Función para cargar los datos desde un archivo pickle
def cargar_datos():
    try:
        with open('datos.pkl', 'rb') as file:
            datos = pickle.load(file)
        return datos
    except (FileNotFoundError, EOFError):
        return {'estudiantes': [], 'profesores': [], 'directivos': []}

# Función para guardar los datos en un archivo pickle
def guardar_datos(datos):
    with open('datos.pkl', 'wb') as file:
        pickle.dump(datos, file)

# Función principal
def main():
    datos = cargar_datos()
    estudiantes = datos['estudiantes']
    profesores = datos['profesores']
    directivos = datos['directivos']

    # Variable de estado para controlar la selección
    seleccion = st.sidebar.radio('Selecciona una opción:',
                                  ('Registrar Alumno', 'Registrar Profesor', 'Registrar Directivo', 'Mostrar Alumnos', 'Mostrar Profesores', 'Mostrar Directivos', 'Borrar registro de Alumno', 'Borrar registro de Profesor', 'Borrar registro de Directivo'))

    if seleccion == 'Registrar Alumno':
        agregar_estudiante(estudiantes)
    elif seleccion == 'Registrar Profesor':
        agregar_profesor(profesores)
    elif seleccion == 'Registrar Directivo':
        agregar_directivo(directivos)
    elif seleccion == 'Mostrar Alumnos':
        mostrar_estudiantes(estudiantes)
    elif seleccion == 'Mostrar Profesores':
        mostrar_profesores(profesores)
    elif seleccion == 'Mostrar Directivos':
        mostrar_directivos(directivos)
    elif seleccion == 'Borrar registro de Alumno':
        eliminar_estudiante(estudiantes)
    elif seleccion == 'Borrar registro de Profesor':
        eliminar_profesor(profesores)
    elif seleccion == 'Borrar registro de Directivo':
        eliminar_directivo(directivos)

  # Al final de la función principal, guardar los datos antes de salir
    datos = {'estudiantes': estudiantes, 'profesores': profesores, 'directivos': directivos}
    guardar_datos(datos)

# Función para agregar un estudiante a la base de datos
def agregar_estudiante(estudiantes):
    st.header('Registrar Alumno')
    nombre = st.text_input('Nombre:')
    edad = st.number_input('Edad:', min_value=0)
    correo = st.text_input('Correo:')
    carrera = st.text_input('Carrera:')

    if st.button('Registrar Alumno'):
        nuevo_estudiante = Estudiante(nombre, edad, correo, carrera)
        estudiantes.append(nuevo_estudiante)
        st.write('El alumno ha sido registrado exitosamente.')

# Función para agregar un profesor a la base de datos
def agregar_profesor(profesores):
    st.header('Registrar Profesor')
    nombre = st.text_input('Nombre:')
    edad = st.number_input('Edad:', min_value=0)
    correo = st.text_input('Correo:')
    
    
    area = st.text_input('Área:')

    if st.button('Registrar Profesor'):
        nuevo_profesor = Profesor(nombre, edad, correo, area)
        profesores.append(nuevo_profesor)
        st.write('El profesor ha sido registrado exitosamente.')

# Función para agregar un directivo a la base de datos
def agregar_directivo(directivos):
    st.header('Registrar Directivo')
    nombre = st.text_input('Nombre:')
    edad = st.number_input('Edad:', min_value=0)
    correo = st.text_input('Correo:')
    cargo = st.text_input('Cargo:')

    if st.button('Registrar Directivo'):
        nuevo_directivo = Directivo(nombre, edad, correo, cargo)
        directivos.append(nuevo_directivo)
        st.write('El directivo ha sido registrado exitosamente.')

# Función para mostrar la lista de estudiantes en la base de datos
def mostrar_estudiantes(estudiantes):
    st.header('Listado de Alumnos')
    if not estudiantes:
        st.write('No se encontraron alumnos registrados.')
    else:
        for i, estudiante in enumerate(estudiantes):
            st.write(f'ID: {i}')
            st.write(f'Nombre: {estudiante.get_nombre()}')
            st.write(f'Edad: {estudiante.get_edad()}')
            st.write(f'Correo: {estudiante.correo}')
            st.write(f'Carrera: {estudiante.carrera}')
            st.write('---')

# Función para mostrar la lista de profesores en la base de datos
def mostrar_profesores(profesores):
    st.header('Listado de Profesores')
    if not profesores:
        st.write('No se encontraron profesores registrados.')
    else:
        for i, profesor in enumerate(profesores):
            st.write(f'ID: {i}')
            st.write(f'Nombre: {profesor.get_nombre()}')
            st.write(f'Edad: {profesor.get_edad()}')
            st.write(f'Correo: {profesor.correo}')
            st.write(f'Área: {profesor.area}')
            st.write('---')

# Función para mostrar la lista de directivos en la base de datos
def mostrar_directivos(directivos):
    st.header('Listado de Directivos')
    if not directivos:
        st.write('No se encontraron directivos registrados.')
    else:
        for i, directivo in enumerate(directivos):
            st.write(f'ID: {i}')
            st.write(f'Nombre: {directivo.get_nombre()}')
            st.write(f'Edad: {directivo.get_edad()}')
            st.write(f'Correo: {directivo.correo}')
            st.write(f'Cargo: {directivo.cargo}')
            st.write('---')

# Función para eliminar un estudiante de la base de datos
def eliminar_estudiante(estudiantes):
    st.header('Eliminar registro de Alumno')
    mostrar_estudiantes(estudiantes)
    if not estudiantes:
        st.write('No hay alumnos para eliminar.')
        return

    id_eliminar = st.number_input('Ingrese el ID del alumno a eliminar:', min_value=0, max_value=len(estudiantes)-1)
    if st.button('Eliminar Alumno'):
        if 0 <= id_eliminar < len(estudiantes):
            estudiantes.pop(id_eliminar)
            st.write(f'Alumno con ID {id_eliminar} ha sido eliminado exitosamente.')
        else:
            st.write('ID de alumno no válido.')

# Función para eliminar un profesor de la base de datos
def eliminar_profesor(profesores):
    st.header('Eliminar registro de Profesor')
    mostrar_profesores(profesores)
    if not profesores:
        st.write('No hay profesores para eliminar.')
        return

    id_eliminar = st.number_input('Ingrese el ID del profesor a eliminar:', min_value=0, max_value=len(profesores)-1)
    if st.button('Eliminar Profesor'):
        if 0 <= id_eliminar < len(profesores):
            profesores.pop(id_eliminar)
            st.write(f'Profesor con ID {id_eliminar} ha sido eliminado exitosamente.')
        else:
            st.write('ID de profesor no válido.')

# Función para eliminar un directivo de la base de datos
def eliminar_directivo(directivos):
    st.header('Eliminar registro de Directivo')
    mostrar_directivos(directivos)
    if not directivos:
        st.write('No hay directivos para eliminar.')
        return

    id_eliminar = st.number_input('Ingrese el ID del directivo a eliminar:', min_value=0, max_value=len(directivos)-1)
    if st.button('Eliminar Directivo'):
        if 0 <= id_eliminar < len(directivos):
            directivos.pop(id_eliminar)
            st.write(f'Directivo con ID {id_eliminar} ha sido eliminado exitosamente.')
        else:
            st.write('ID de directivo no válido.')



if __name__ == '__main__':
    main()
```
