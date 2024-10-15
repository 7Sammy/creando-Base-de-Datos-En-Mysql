# creando-Base-de-Datos-En-Mysql
Actividad_03
Este código SQL está diseñado para consultar dos tablas de una base de datos: empleado y departamento. El objetivo es obtener una lista de todos los empleados, incluyendo aquellos que no están asignados a ningún departamento, junto con los nombres de los departamentos a los que pertenecen.
SELECT
    empleado.nombre AS NombreEmpleado,
    empleado.apePaterno AS ApellidoPaterno,
    departamento.nombre AS NombreDepartamento
FROM
    empleado
LEFT JOIN
    departamento ON empleado.codigo_departamento = departamento.codigo;
