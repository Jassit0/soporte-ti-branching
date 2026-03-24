# Tarea 4: Soporte a infraestructura y conectividad (hardware/red)

**ID de Incidente:** #HR-2026-0324  
**Fecha:** 24 de marzo de 2026  
**Técnico:** Soporte IT (Jorge Cristian Peralta)  
**Departamento:** Recursos Humanos  

---

## 1. Descripción del Problema

El departamento de Recursos Humanos reportó una degradación significativa en la velocidad de navegación y latencia en las aplicaciones internas, afectando la productividad del área.

---

## 2. Diagnóstico y Acciones Realizadas

### A. Revisión Física y Reemplazo de Hardware

Se realizó una inspección visual de la infraestructura de red en el sitio. Se detectó que el cable Ethernet de la estación principal presentaba desgaste físico y una categoría insuficiente para la demanda actual de datos.

**Acción:** Se reemplazó el cableado Categoría 5e por un cable Categoría 6 para asegurar una mejor integridad de señal y soporte de mayores velocidades.

---

### B. Análisis de Red y Latencia

Se ejecutó un script de diagnóstico de red personalizado para medir los tiempos de respuesta y la pérdida de paquetes.

**Hallazgo:** Los resultados del script indicaron una latencia inestable. El análisis de espectro mostró que el Access Point (AP) de la zona estaba operando en un canal saturado por interferencias de oficinas colindantes.

**Acción:** Reconfiguración del canal del AP a un canal menos congestionado (canal de menor interferencia identificado por el escáner de red).

---

### C. Optimización de Software (Ancho de Banda)

Se identificó que procesos en segundo plano consumían gran parte del tráfico de subida y bajada de manera intermitente.

**Acción:** Se configuraron las Directivas de Grupo (GPO) para desactivar las actualizaciones automáticas de Windows durante el horario laboral (08:00 - 18:00). Las actualizaciones se programaron para ejecutarse exclusivamente en horario nocturno.

---

## 3. Resultados de las Pruebas Finales

| Parámetro               | Estado Previo              | Estado Final        |
|------------------------|---------------------------|---------------------|
| Velocidad de Descarga  | Inestable (15-20 Mbps)    | Estable (95+ Mbps)  |
| Latencia (Ping)        | >150 ms (con picos)       | <20 ms (constante)  |
| Interferencia Wi-Fi    | Alta (Canal 6)            | Baja (Canal 11)     |

> **Nota:** La conexión se reporta como **"Óptima"**. Se recomienda al personal de RR.HH. priorizar la conexión vía Ethernet siempre que sea posible.

---

## 4. Recomendaciones

- Realizar una limpieza periódica de los puntos de red físicos para evitar daños por tracción en los cables.  
- Monitorear el rendimiento del canal Wi-Fi mensualmente debido a la alta densidad de redes en el edificio.
