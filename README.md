def saludar(nombre):
    print(f"\nHola {nombre}, ¡bienvenida al sistema!")

def verificar_edad(edad):
    if edad >= 18:
        print("Eres mayor de edad ✅")
    else:
        print("Eres menor de edad ❌")

def contar_hasta_edad(edad):
    print(f"\nContando del 1 al {edad}:")
    for i in range(1, edad + 1):
        print(i)

def años_para_100(edad):
    return 100 - edad

# Aquí empieza el ciclo
while True:
    nombre = input("\n¿Cómo te llamas? ")
    edad = int(input("¿Cuántos años tienes? "))

    saludar(nombre)
    verificar_edad(edad)
    contar_hasta_edad(edad)

    faltan = años_para_100(edad)
    print(f"Te faltan {faltan} años para llegar a los 100 🎉")

    repetir = input("\n¿Quieres volver a intentarlo? (sí/no): ").lower()
    if repetir != "sí":
        print("¡Hasta luego, crack! 👋")
        break

