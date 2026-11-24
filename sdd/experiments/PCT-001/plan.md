# Plan técnico
Python 3.12 como propuesta inicial, pytest, datos JSON/CSV y CLI; sin dependencias de IA necesarias. Mantener UI fuera del MVP.
Módulos: world (transiciones puras), agent (contrato común), oracle (BFS sobre estado ampliado), metrics, runner, report.
Presupuesto: pasos del entorno, operaciones de planificación y memoria registrados y limitados; mismo límite por agente. Emparejar semillas y mundos.
Diseño: mundos estáticos y cambiantes; separar desarrollo y confirmación por semillas y recetas. Piloto para estimar varianza y fijar tamaño muestral y umbral de efecto antes del análisis confirmatorio. Reportar diferencias emparejadas, intervalos y fallos.
Pruebas: determinismo, invariantes de recursos, recetas inválidas, alcance del oráculo en mapas manuales, equidad de presupuesto, ausencia de filtraciones entre entrenamiento y prueba. Ablación de ajuste de estrategia y baseline de exploración competitivo.
Salida: config, seeds, commit SHA, logs, resultados crudos, informe y limitaciones.
