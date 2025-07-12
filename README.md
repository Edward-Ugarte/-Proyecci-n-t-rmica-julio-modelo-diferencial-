# Proyeccion-termica-julio-modelo-diferencial
README - Proyección térmica diferenciada en Gretl (Julio)

Autor:  Econ. Edward Ugarte
Versión: 1.0
Software requerido: Gretl 2025b

Descripción:
Este módulo calcula proyecciones diarias de temperaturas mínimas, máximas, medias y sensación térmica (Wind Chill) para el mes de julio, usando como base empírica los primeros 30 días de junio.

Variables proyectadas:
- temp_max : Temperatura mínima
- temp_min : Temperatura máxima
- temp_media : Temperatura media
- st_min  : Sensación térmica (Wind Chill Index)



Metodología:
1. Aplicación de diferenciación temporal: ΔX = X[t] - X[t-1]
2. Proyección sobre rango 31–61 (todo julio)
3. Cálculo perceptual diario de sensación térmica usando Wind Chill Index:

   ST = 13.12 + 0.6215*T - 11.37*V^0.16 + 0.3965*T*V^0.16

Visualización:




Las etiquetas del gráfico deben editarse manualmente:
- Serie 1: Tmin proyectada
- Serie 2: Tmax proyectada
- Serie 3: Tmedia proyectada
- Serie 4: Sensación térmica


Aplicaciones:
- Estudios de confort climático
- Boletines térmicos diarios
- Validación perceptual para eventos fríos extremos
- Enseñanza de modelos econométricos físicos diferenciados
