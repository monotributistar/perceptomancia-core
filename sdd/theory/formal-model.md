# Modelo formal v0.1
Sea X un espacio finito de estados del mundo, A(x,c) las acciones habilitadas por capacidades c, T(x,a) una transición y O(x) una observación. Incluir recursos y capacidades en el estado ampliado z=(x,c,b) para que la transición sea bien definida. Presupuesto B, horizonte k y proyección común q de resultados funcionales.
H_k(z;B) = { q(x') : existe una trayectoria factible de longitud <= k desde z, costo <= B }.
Medida exploratoria P_k = log2 |H_k| (incluye estado inicial; H no vacío). Es cardinalidad logarítmica, no empowerment ni medida de conciencia.
Ganancias G=H_after\\H_before; pérdidas L=H_before\\H_after. Reportar ambas con igual presupuesto restante y horizonte; no asumir monotonicidad.
Distinguir horizonte verdadero en entorno finito (oráculo), estimación del agente y conjunto efectivamente visitado. Un modelo puede imaginar estados imposibles. Comparar precisión/recall con oráculo cuando sea factible.
En entornos estocásticos, definir umbral de probabilidad y política antes del análisis; no comparar cardinalidades de espacios continuos sin discretización explícita.
Ejemplo: una herramienta habilita una acción antes inválida, pero consume recursos; el horizonte neto podría disminuir.
