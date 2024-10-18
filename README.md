# CODIGO 1 DE LA PR4 DEL 2DO PARCIAL. CREADO POR RAMIREZ TORRES ANGEL MANUEL DE 3°W NUMERO DE CONTROL: 1206
- Crear un diccionario vacío y lo vaya llenado con información sobre una persona (por ejemplo nombre, edad, sexo, teléfono, correo electrónico, etc.) que se le pida al usuario. Cada vez que se añada un nuevo dato debe imprimirse el contenido del diccionario.


print(" ")#crear un espacio entre lineas 
print("Ramirez Torres Angel Manuel")#Muestra el nombre de quen lo creo 
print("NUMERO DE CONTOL: 1206")#Muestra su numero de control 
print("-INSTRUCCIONES-")#Muestra las instrucciones siguientes 
print("Crear un diccionario vacío y lo vaya llenado con información sobre una persona (por ejemplo")
print("nombre, edad, sexo, teléfono, correo electrónico, etc.) que se le pida al usuario. Cada vez que se")
print("añada un nuevo dato debe imprimirse el contenido del diccionario.")
print(" ")#crear un espacio entre lineas 


# Crear un diccionario vacío 
persona = {}

# Solicitar y añadir el nombre
nombre = input("Introduce el nombre: ")  #introduzca su nombre
persona['nombre'] = nombre  #nombre al diccionario
print("Contenido del diccionario:", persona)  # Muestra el contenido

print(" ")#crear un espacio entre lineas 

# Solicitar y añadir la edad
edad = input("Introduce la edad: ")  # Pide que introduzca su edad
persona['edad'] = edad  # Añade la edad al diccionario
print("Contenido del diccionario:", persona)  # Muestra el contenido

print(" ")#crear un espacio entre lineas 

# Solicitar y añadir el sexo
sexo = input("Introduce el sexo: ")  # Pide que introduzca su sexo
persona['sexo'] = sexo  # Añade el sexo al diccionario
print("Contenido del diccionario:", persona)  # Muestra el contenido 

print(" ")#crear un espacio entre lineas 

# Solicitar y añadir el teléfono
telefono = input("Introduce el teléfono: ")  # Pide que introduzca su teléfono
persona['telefono'] = telefono  # Añade el teléfono al diccionario
print("Contenido del diccionario:", persona)  # Muestra el contenido

print(" ")#crear un espacio entre lineas 

# Solicitar y añadir el correo electrónico
correo = input("Introduce el correo electrónico: ")  # Pide que introduzca su correo
persona['correo'] = correo  # Añade el correo al diccionario
print("Contenido del diccionario:", persona)  # Muestra el contenido 

print(" ")#crear un espacio entre lineas 

#muestra toda la información 
print("Información final de la persona:", persona)

![image](https://github.com/user-attachments/assets/3091c9ff-fb36-4116-82e6-fdb6b9f215fa)
![image](https://github.com/user-attachments/assets/dc2f52de-98d5-4bb2-81cc-398afbf8dac0)
![image](https://github.com/user-attachments/assets/55c17605-ff30-469a-ba25-175a6e807140)



# CODIGO 2 DE LA PR4 DEL 2DO PARCIAL. CREADO POR RAMIREZ TORRES ANGEL MANUEL DE 3°W NUMERO DE CONTROL: 1206
- Hacer un diccionario de traducción español-inglés, se van a introducir las palabras en español e inglés separadas por dos puntos, y cada par <palabra>:<traducción> separados por comas. El programa debe crear un diccionario con las palabras y sus traducciones. Después pedirá una frase en español y utilizará el diccionario para traducirla palabra a palabra. Si una palabra no está en el diccionario debe dejarla sin traducir.



print(" ")#crear un espacio entre lineas 
print("Ramirez Torres Angel Manuel")#Muestra el nombre de quen lo creo 
print("NUMERO DE CONTOL: 1206")#Muestra su numero de control 
print("-INSTRUCCIONES-")#Muestra las instrucciones siguientes 
print("Hacer un diccionario de traducción español-inglés, se van a introducir las palabras en español e inglés separadas")
print("por dos puntos, y cada par <palabra>:<traducción> separados por comas. El programa debe crear un diccionario con")
print("las palabras y sus traducciones. Después pedirá una frase en español y utilizará el diccionario para traducirla palabra a")
print("palabra. Si una palabra no está en el diccionario debe dejarla sin traducir.")
print(" ")#crear un espacio entre lineas 




#Se crea el diccionario
def crear_diccionario(entrada):
    diccionario = {}
    for par in entrada.split(','):
        esp, eng = par.split(':')
        diccionario[esp.strip()] = eng.strip()
    return diccionario

#Aqui se traducira una frase 
def traducir_frase(diccionario, frase):
    palabras = frase.split()
    #Traduce las palabras mentras usa el diccionario 
    traduccion = []
    for palabra in palabras:
        # Si la palabra está en el diccionario, la traduce si no se deja igual 
        traduccion.append(diccionario.get(palabra, palabra))
    return ' '.join(traduccion)
    

#pide al usuario que introuzca una frase 
frase = input("Introduce una frase en español: ")
traduccion = traducir_frase(diccionario, frase)  #Traduce la frase
print("Traducción:", traduccion)  #Mostrar la traducción


![image](https://github.com/user-attachments/assets/322a7a70-8d51-4fab-8a1a-6d77c9460514)
![image](https://github.com/user-attachments/assets/e0fca0c9-1b8c-4029-8033-5ecbd542900c)
![image](https://github.com/user-attachments/assets/f5545d62-e789-4a8a-a4c7-7aaf4e9d8806)
