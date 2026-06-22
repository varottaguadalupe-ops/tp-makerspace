visitas = []

def solicitar_datos():
    nombre = input("Ingrese el nombre del estudiante: ")
    curso = input("Ingrese el curso: ")
    motivo = input("Ingrese el motivo de la visita: ")

    visita = {
        "nombre": nombre,
        "curso": curso,
        "motivo": motivo
    }

    return visita


def mostrar_visitas(visitas):
    print("\n===== LISTA DE VISITAS =====")

    for estudiante in visitas:
        print("\nNombre:", estudiante["nombre"])
        print("Curso:", estudiante["curso"])
        print("Motivo:", estudiante["motivo"])


def contar_cursos(visitas):
    cursos = {}

    for estudiante in visitas:
        curso = estudiante["curso"]

        if curso in cursos:
            cursos[curso] += 1
        else:
            cursos[curso] = 1

    print("\n===== VISITAS POR CURSO =====")

    for curso in cursos:
        print(curso, ":", cursos[curso], "visita/s")


def mostrar_primer_estudiante(visitas):
    if len(visitas) > 0:
        print("\nPrimer estudiante registrado:")
        print(visitas[0]["nombre"])


for i in range(3):
    print("\nRegistro", i + 1)
    visitas.append(solicitar_datos())

mostrar_visitas(visitas)
contar_cursos(visitas)
mostrar_primer_estudiante(visitas)

