# Makefile

# Tarea 1: Compilar y ejecutar el código
run:
	gcc -o hello2 hello2.c
	./hello2

# Tarea 2: Obtener la salida de la etapa de pre-procesado
preprocess:
	gcc -E hello2.c -o hello2.i

# Tarea 3: Verificar qué ocurrió con la "llamada a min()" en hello2.i
check_min:
	grep "min(" hello2.i || true

# Tarea 4: Verificar el efecto de la directiva #include <stdio.h>
check_include:
	grep "#include <stdio.h>" hello2.i || true

# Realizar todas las tareas anteriores
all_tasks: run preprocess check_min check_include

# Limpiarlo todo
clean:
	rm -rf hello2 hello2.i
