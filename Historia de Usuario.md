Historia de Usuario 
Como estudiante, quiero realizar un simulacro  según el tema que elija, para prepararme mejor para los exámenes.

Happy Paths
1. Iniciar Simulacro correctamente
Dado que el usuario ha iniciado sesión y selecciona un tema, cuando hace clic en “Iniciar Simulacro”, entonces se cargan las preguntas del tema seleccionado y comienza el conteo regresivo.

2. Responder pregunta y avanzar
Dado que el usuario ve una pregunta activa y selecciona una respuesta, cuando hace clic en “Responder”,entonces se envía su respuesta al backend y se carga la siguiente pregunta.

3. Finaliza simulacro y ve resultados
Dado que el usuario ha respondido todas las preguntas, cuando llega al final del simulacro, entonces puede hacer clic en “Ver resultados” y se actualizan sus monedas y experiencia.

4. El simulacro se adapta al tiempo restante
Dado que el usuario está resolviendo el simulacro, cuando el tiempo llega a menos de 30 segundos, entonces el contador se muestra en rojo como advertencia visual.


Unhappy Paths
1. No selecciona tema
Dado que el usuario no ha elegido ningún tema, cuando hace clic en “Iniciar Simulacro”, entonces aparece un mensaje de alerta: "Por favor selecciona un tema" y el simulacro no inicia.

2. Intenta responder sin seleccionar una opción
Dado que el usuario no ha seleccionado ninguna respuesta, cuando hace clic en “Responder”, entonces se muestra una alerta: "Selecciona una respuesta" y no se avanza.

3. El tiempo se agota antes de terminar
Dado que el usuario no ha terminado el simulacro, cuando el tiempo llega a 0 segundos, entonces aparece una alerta "El tiempo ha terminado. Se cerró el simulacro automáticamente." y se bloquea la interacción.














