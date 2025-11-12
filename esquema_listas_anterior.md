# Esquema de Listas - Modelo Relacional sin Lookups, selecciones y campos de opcion

1. **tab_pantallas**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
pantallas	Una línea de texto	
vista_escritorio	Número	
fk_id_rol	Número	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

2. **tab_leads**

Columna (hacer clic para editar) Tipo	Requerida
fecha_creacion_lead	Fecha y hora	
ultima_actualizacion	Fecha y hora	
estatus_cuenta	Una línea de texto	
id_nesp_corp_nit	Número	
nombre_comercial_prospecto	Una línea de texto	
razon_social_prospecto	Una línea de texto	
ciudad	Una línea de texto	
segmento	Una línea de texto	
subsegmento	Una línea de texto	
nombre_contacto	Una línea de texto	
apellidos_contacto	Una línea de texto	
cargo	Una línea de texto	
email	Una línea de texto	
op_modelo_comercial	Una línea de texto	
op_detalle_op_comercial	Una línea de texto	
op_op_construccion_marca	Una línea de texto	
mc_maquinas	Una línea de texto	
mc_mes_de_colocacion	Una línea de texto	
mc_consumo_minimo	Una línea de texto	
estado_interese	Una línea de texto	
correo_comercial_creador	Una línea de texto	
nombre_carpeta	Una línea de texto	
carpeta_creada	Número	
documentos_aprobados	Número	
cliente_con_credito	Número	
cupo_solicitado	Número	
id_estado_negociacion	Número	
aprobacion_back_office	Número	
aprobacion_finanzas	Número	
payment_mode	Una línea de texto	
tarifa	Número	
sagrilaft	Una línea de texto	
canal	Una línea de texto	
requiere_documentos	Número	
plazo_credito	Número	
fecha_paso_a_prospecto	Fecha y hora	
fecha_paso_a_cliente	Fecha y hora	
estado_interes	Elección	
ciudad_relacionada	Búsqueda	
op_modelo_comercial_lead	Elección	
op_modelo_comercial_prospect	Elección	
statusNegociacion_relacionado	Búsqueda	
status_usuario	Elección	
segmento_rel	Búsqueda	
subsegmento_rel	Búsqueda	
canal_relacionado	Búsqueda	



1. **tab_seguimiento**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
fecha_seguimiento	Fecha y hora	
anotaciones	Una línea de texto	
estado_seguimiento	Número	
observaciones	Varias líneas de texto	
fk_id_lead	Número	
correo_responsable	Una línea de texto	
nombre_comercial	Una línea de texto	
fk_tipo_cliente	Número	
status_seguimiento	Elección	
comercial_responsable	Persona o grupo	
lead_relacionado	Búsqueda	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo	

4. **tab_cliente**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
nombre	Una línea de texto	
fecha_creacion	Fecha y hora	
correo	Una línea de texto	
estado	Una línea de texto	
id_nesp_corp	Número	
n_maquinas	Número	
canal	Una línea de texto	
ciudad	Una línea de texto	
segmento	Una línea de texto	
subsegmento	Una línea de texto	
nombre_contacto	Una línea de texto	
apellido_contacto	Una línea de texto	
cargo	Una línea de texto	
email	Una línea de texto	
payment_mode	Una línea de texto	
tarifa	Una línea de texto	
sagrilatf	Una línea de texto	
cliente_con_credito	Número	
cupo_solicitado	Número	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

5. **tab_ciudades**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
Departamento	Una línea de texto	
Ciudad	Una línea de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

6. **tab_visitas_por_cliente** 
Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
fecha_visitas	Fecha y hora	
tipo_visita	Una línea de texto	
correo	Una línea de texto	
nombre	Una línea de texto	
fk_id_nesp_corp	Número	
nombre_cliente	Una línea de texto	
estado_visita	Número	
observaciones	Varias líneas de texto	
observaciones_supply	Varias líneas de texto	
fecha_cierre_visita	Fecha y hora	
direccion_cliente	Varias líneas de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

7. **roles**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
rol	Una línea de texto	
pk_id_rol	Número	
id_rol_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

8. **tab_roles_usuarios**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
correo	Una línea de texto	
id_rol	Número	
rol_designado	Búsqueda	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

9. **tab_documentos_cliente**

Columna (hacer clic para editar)	Tipo	Requerida

nombre_documento	Una línea de texto	
tipo_documento	Número	
nombre_tipo_documento	Una línea de texto	
cantidad_de_documentos	Número	
nombre_carpeta_documento	Una línea de texto	
mostrar_finanzas	Número	

1. **tab_maquinas_por_cliente**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
maquina	Una línea de texto	
consumo_minimo	Número	
mes_colocacion	Una línea de texto	
estado_maquina	Número	
fk_id_cliente_nesp_corp	Número	
serial_maquina	Número	
tiene_condiciones_especiales	Número	
descripcion_condiciones	Varias líneas de texto	
aprobacion_back_office	Número	
id_nesp_corp_cliente	Número	
razon_social	Una línea de texto	
correo_solicitante	Una línea de texto	
fecha_solicitud	Fecha y hora	
fecha_aprobacion	Fecha y hora	
notas_supply	Varias líneas de texto	
direccion_cliente	Varias líneas de texto	
notas_supply2	Varias líneas de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

10. **tab_documentos_por_cliente**

Columna (hacer clic para editar)	Tipo	Requerida

fk_id_nesp_corp_cliente	Número	
estado_documento	Una línea de texto	
comentarios_documento	Varias líneas de texto	
fk_id_documento_sharepoint	Número	
data_uri	Varias líneas de texto	
nombre_documento	Una línea de texto	
fk_id_lead	Número	
fk_id_doc	Número	
nompre_tipo_de_documento	Una línea de texto	
nombre_carpeta_cliente	Una línea de texto	
aprobado_back_office	Número	
aprobado_finanzas	Número	


1.  **tab_tipo_cliente**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
tipo	Una línea de texto	
id_tipo	Número	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

12. **tab_canales**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
canal	Una línea de texto	
id_canal	Una línea de texto	
id_canal_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

13. **tab_canal_por_comercial**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
correo_comercial	Una línea de texto	
id_canal	Número	
canal	Una línea de texto	
comercial_designado	Persona o grupo	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

14. **tab_registro_ventas** 

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
razon_social	Una línea de texto	
id_nesp_corp	Número	
fecha_carga	Fecha y hora	
correo_carga	Una línea de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

15. **tab_ventas_por_cliente** 

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
tipo_producto	Una línea de texto	
cantidad	Número	
valor	Número	
fecha	Fecha y hora	
id_cliente_nesp_corp	Número	
razon_social	Una línea de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

16. **tab_estados_negociaciones** 

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
estado_negociacion	Una línea de texto	
id_estado_negociacion	Número	
id_estadoNeg_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

17. **tab_comentarios_documentos** 

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
comentarios	Varias líneas de texto	
fk_id_lead	Número	
correo_quien_comenta	Una línea de texto	
fk_rol_quien_comenta	Número	
fk_id_documento	Número	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

18. **tab_estados_maquinas**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
estado_maquinas	Una línea de texto	
id_estados_maquinas	Número	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

19. **tab_estados_documentos**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
estados_documentos	Una línea de texto	
id_estado_documento	Número	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

20. **tab_maquinas_nesp_corp**  

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

21. **tab_nombres_maquinas_nesp_corp** 

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
nombre_maquina	Una línea de texto	
id_maquina	Número	
consumo_minimo_maquina	Número	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

22. **tab_indicadores_comerciales**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
canal	Una línea de texto	
id_canal	Número	
nns	Número	
maquinas	Número	
capsulas	Número	
fecha	Fecha y hora	
periodicidad	Una línea de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

23. **tab_segmentos**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
segmento	Una línea de texto	
id_segmento	Número	
id_segmento_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

24. **tab_subsegmentos**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
sub_segmento	Una línea de texto	
id_sub_segmento	Número	
id_segmento_relacionado	Búsqueda	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

25. **tab_comentarios_maquinas**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
fk_id_solicitud_maquina	Número	
fk_id_estado_maquina	Número	
correo	Una línea de texto	
comentario	Varias líneas de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

26. **tbl_meses**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
mes	Una línea de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

27. **tab_oportunidad**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
oportunidad	Una línea de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo