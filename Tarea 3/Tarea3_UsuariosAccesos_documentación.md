\# Tarea 3: Gestión de Usuarios y Accesos

\*\*Curso:\*\* IT Helpdesk - Generation México  

\*\*Especialista:\*\* \[Jorge Cristian Peralta Pichardo / CrisDotExe]  

\*\*Fecha:\*\* 20 de marzo de 2026



---



\## 1. Escenario Seleccionado

\*\*Caso:\*\* Alta de empleado nuevo (Onboarding)  

\*\*Departamento:\*\* Recursos Humanos (RH)



---



\## 2. Perfil del Usuario (Parte B)

| Atributo | Detalle |

| :--- | :--- |

| \*\*Nombre\*\* | Carlos Adrian |

| \*\*Área / Depto\*\* | Recursos Humanos |

| \*\*Rol\*\* | Generalista de Nóminas |

| \*\*Herramientas\*\* | Outlook, Drive, Office365, Microsoft, Teams, Zoom |



---



\## 3. Flujo de Atención (Parte C)

Como Mesa de Servicio, el proceso seguido fue:



\* \*\*Recepcion de solicitud:\*\* Se recibió el ticket #RH-2026-005 solicitando el alta de acceso para el nuevo colaborador.

\* \*\*Validación / Autorización:\*\* El Director de RH autorizó los permisos de lectura/escritura en la carpeta de "Sueldos y Salarios".

\* \*\*Acción ejecutada:\*\* \* Creación de usuario en Ubuntu.

&nbsp;   \* Asignación de licencia Microsoft 365 Business.

&nbsp;   \* Configuración de \*\*MFA (Autenticación de dos factores)\*\* obligatoria.

\* \*\*Confirmación con usuario:\*\* Se entregaron credenciales temporales vía canal seguro y se verificó el acceso inicial exitoso.

\* \*\*Documentación:\*\* Registro de la bitácora de permisos otorgados y cierre del ticket en el sistema.



---



\## 4. Aplicación del Principio de Mínimo Privilegio

Para garantizar la seguridad de la información sensible de la empresa:

1\. Se otorgó acceso de \*\*Solo Lectura\*\* a los expedientes históricos para evitar modificaciones accidentales.

2\. El acceso al Sistema de Nómina está restringido únicamente al módulo de "Carga de Incidencias".

3\. No se otorgaron permisos de \*\*Administrador Local\*\* en el equipo para evitar la instalación de software no autorizado.



---



\## 5. Evidencia Simulada (Parte D)



\### Checklist de Configuración

\- \[x] Cuenta de correo: `carlsoadrian@empresa.com` creada.

\- \[x] Cifrado de disco (BitLocker) activado en Laptop #RH-02.

\- \[x] Acceso a carpeta compartida `\\\\Servidor\\RH\\Nominas` configurado.

\- \[x] Token de seguridad MFA vinculado al dispositivo móvil.



\### Formato de Ticket (Mockup)

```text

TICKET ID: #RH-2026-005

ESTADO: CERRADO

SOLICITANTE: Director de RH

DESCRIPCIÓN: Alta de usuario "Carlos Adrian". 

NOTAS DE TI: Usuario creado siguiendo la política de seguridad 
de datos sensibles. MFA activo.

