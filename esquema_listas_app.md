Anteriormente el modelo relacion del sitio de sharepoint estaba compuesto de las siguientes listas:

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

pero para que exista una trazabilidad adecuada y mas clara entre los cambios que suceden durante el proceso se opto por estructurar y crear nuevas listas que permitieran un mejor manejo de la informacion y una mayor facilidad al momento de realizar consultas o actualizaciones a los datos que puedes ver a continuacion las listas que se actualizaron y las que se crearon para reemplzar algunas de las listas existentes para bien

1. **tab_roles**
Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
rol	Una línea de texto	
pk_id_rol	Número	
id_rol_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

2. **tab_roles_usuarios**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
correo	Una línea de texto	
id_rol	Número	
rol_designado	Búsqueda	
usuario	Persona o grupo	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

3. **tab_canales**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
canal	Una línea de texto	
id_canal	Número	
id_canal_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

4. **tab_segmentos**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
segmento	Una línea de texto	
id_segmento	Número	
id_segmento_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

5. **tab_subsegmentos**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
sub_segmento	Una línea de texto	
id_sub_segmento	Número	
id_segmento_relacionado	Búsqueda	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

6. **tab_ciudades**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
Departamento	Una línea de texto	
Ciudad	Una línea de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

7. **tab_documentos_cliente**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
nombre_documento	Una línea de texto	
tipo_documento	Número	
nombre_tipo_documento	Una línea de texto	
cantidad_de_documentos	Número	
nombre_carpeta_documento	Una línea de texto	
mostrar_finanzas	Número	
tipo_doc	Elección	
RequiereAprobacionBackOffice	Sí o No	
RequiereAprobacionFinanzas	Sí o No	
Visible_para	Elección	
RequiereAprobacionOfiCumpl	Sí o No	
RequiereAprobacionBEO	Sí o No	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

8. **tab_nombres_maquinas_nesp_corp**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
nombre_maquina	Una línea de texto	
id_maquina	Número	
consumo_minimo_maquina	Número	
Descripcion_maquina	Varias líneas de texto	
id_maquina_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

9. **tab_oportunidad**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
oportunidad	Una línea de texto	
Descripcion_oport	Una línea de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

10. **tab_estados_negociaciones**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
estado_negociacion	Una línea de texto	
id_estado_negociacion	Número	
id_estadoNeg_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

11. **tab_estados_maquinas**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
estado_maquinas	Una línea de texto	
id_estados_maquinas	Número	
id_statusMaqu_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

12. **tab_estados_documentos**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
estados_documentos	Una línea de texto	
id_estado_documento	Número	
id_statusDoc_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

13. **tab_tipos_visita**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
tipo_Visita	Una línea de texto	
id_tipo_visi	Número	
id_tipoVist_concat	Calculado (cálculo basado en otras columnas)	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

14. **tab_canal_por_comercial**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
correo_comercial	Una línea de texto	
id_canal	Número	
canal	Una línea de texto	
comercial_designado	Persona o grupo	
canal_relacionado	Búsqueda	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

15. **tab_cuentas**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
Created	Fecha y hora	
NIT	Una línea de texto	
RazonSocial	Una línea de texto	
Id_nesp-corp	Número	
EstadoCuenta	Elección	
FechaPasoAProspecto	Fecha y hora	
FechaPasoACliente	Fecha y hora	
EstadoNegociacion	Búsqueda	
Canal	Búsqueda	
Segmento	Búsqueda	
Subsegmento	Búsqueda	
Ciudad	Búsqueda	
NombreContacto	Una línea de texto	
ApellidosContacto	Una línea de texto	
CargoContacto	Una línea de texto	
EmailContacto	Una línea de texto	
ComercialAsignado	Persona o grupo	
CupoSolicitado	Moneda	
RequiereCredito	Sí o No	
PlazoCredito	Elección	
ModalidadPago	Elección	
Tarifa	Número	
EvaluacionSagrilaft	Elección	
RequiereDocumentos	Sí o No	
NombreCarpetaSharePoint	Una línea de texto	
CarpetaCreada	Sí o No	
DocumentosAprobadosBackOffice	Sí o No	
DocumentosAprobadosFinanzas	Sí o No	
Status_cuenta	Elección	
estado_interes	Elección	
FechaCreacionLead	Fecha y hora	
Ultima_actualizacion_cuenta	Fecha y hora

16. **tab_hist_cambioEstd_cuenta**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
Cuenta	Búsqueda	
EstadoAnterior	Elección	
EstadoNuevo	Elección	
FechaCambio	Fecha y hora	
UsuarioResponsable	Persona o grupo	
Motivo	Una línea de texto	
DiasDuracionEstadoAnterior	Número	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

17. **tab_oportunidades_cuenta**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
Cuenta	Búsqueda	
TipoOportunidad	Búsqueda	
EstadoCuentaAlCrear	Elección	
FechaIdentificacion	Fecha y hora	
ComercialIdentifica	Persona o grupo	
Descripcion	Varias líneas de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

18. **tab_maquinas_porCuenta**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
Cuenta	Búsqueda	
TipoMaquina	Búsqueda	
EstadoMaquina	Búsqueda	
EstadoCuentaAlSolicitar	Elección	
FechaSolicitud	Fecha y hora	
ComercialSolicitante	Persona o grupo	
ConsumoMinimoSugerido	Número	
MesColocacionEstimado	Elección	
TieneCondicionesEspeciales	Sí o No	
DescripcionCondiciones	Varias líneas de texto	
AprobadoBackOffice	Sí o No	
UsuarioAprobadorBackOffice	Persona o grupo	
FechaAprobacionBackOffice	Fecha y hora	
AprobadoSupply	Sí o No	
FechaAprobacionSupply	Fecha y hora	
UsuarioAprobadorSupply	Persona o grupo	
SerialMaquina	Una línea de texto	
FechaAsignacionSerial	Fecha y hora	
FechaInstalacion	Fecha y hora	
DireccionInstalacion	Varias líneas de texto	
NotasSupply	Varias líneas de texto	
FechaUltimoMantenimiento	Fecha y hora	
ProximoMantenimiento	Fecha y hora	
FechaRetiro	Fecha y hora	
MotivoRetiro	Varias líneas de texto	
Status_maquina	Elección	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

19. **tab_hist_cambioEstd_maqu**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
Maquina	Búsqueda	
EstadoAnterior	Búsqueda	
EstadoNuevo	Búsqueda	
FechaCambio	Fecha y hora	
UsuarioResponsable	Persona o grupo	
Comentario	Varias líneas de texto	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

20. **tab_documentos_porCuenta**

Columna (hacer clic para editar)	Tipo	Requerida

Cuenta	Búsqueda	
TipoDocumento	Búsqueda	
EstadoDocumento	Búsqueda	
URLDocumento	Varias líneas de texto	
FechaCarga	Fecha y hora	
UsuarioCarga	Persona o grupo	
AprobadoBackOffice	Sí o No	
FechaAprobacionBackOffice	Fecha y hora	
UsuarioAprobadorBackOffice	Persona o grupo	
AprobadoFinanzas	Sí o No	
FechaAprobacionFinanzas	Fecha y hora	
UsuarioAprobadorFinanzas	Persona o grupo	
Version	Número	
EsVersionActual	Sí o No	
AprobacionOficialCumplimiento	Sí o No	
FechaAprobacionOficCumpli	Fecha y hora	
AprobacionBEO	Sí o No	
FechaAprobacionBEO	Fecha y hora	
Nombre_documento	Una línea de texto	
Nombre_carpeta_cliente	Una línea de texto

21.  **tab_hist_comentDocumentos**

Columna (hacer clic para editar)	Tipo	Requerida
Documento	Búsqueda	
Cuenta	Búsqueda	
UsuarioComenta	Persona o grupo	
RolUsuario	Búsqueda	
FechaComentario	Fecha y hora	
TipoComentario	Elección	
Comentario	Varias líneas de texto

22.  **tab_seguimiento_porCuenta**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
Cuenta	Búsqueda	
FechaSeguimiento	Fecha y hora	
EstadoCuentaEnSeguimiento	Elección	
ComercialResponsable	Persona o grupo	
TipoSeguimiento	Elección	
EstadoSeguimiento	Búsqueda	
Anotaciones	Una línea de texto	
Observaciones	Varias líneas de texto	
RequiereAccion	Sí o No	
FechaProximoSeguimiento	Fecha y hora	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

23. **tab_visitas_porCuenta**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
Cuenta	Búsqueda	
TipoVisita	Búsqueda	
FechaProgramada	Fecha y hora	
FechaRealizacion	Fecha y hora	
UsuarioResponsable	Persona o grupo	
DireccionVisita	Varias líneas de texto	
EstadoVisita	Elección	
ObservacionesComercial	Varias líneas de texto	
ObservacionesSupply	Varias líneas de texto	
FechaCierre	Fecha y hora	
RequiereAccionCorrectiva	Sí o No	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Persona o grupo	
Modificado por	Persona o grupo

las cuales a comparacion del anterior modelo relacional he definido para una mejor trazabilidad segun el tipo de lista que puedes analizar en el siguiente estructura

## Mapeo de Transformación de Listas - Modelo Relacional

| LISTA ORIGINAL | LISTA CREADO A REEMPLAZO | DEPENDENCIA | UTILIDAD | TIPO_LISTA |
|---|---|---|---|---|
| tab_ciudades | - | LISTA IND | CATALOGO | INICIAL |
| roles | - | LISTA IND | CATALOGO | INICIAL |
| tab_canales | - | LISTA IND | CATALOGO | INICIAL |
| tab_estados_negociaciones | - | LISTA IND | CATALOGO | INICIAL |
| tab_estados_maquinas | - | LISTA IND | CATALOGO | INICIAL |
| tab_estados_documentos | - | LISTA IND | CATALOGO | INICIAL |
| tab_segmentos | - | LISTA IND | CATALOGO | INICIAL |
| tab_oportunidad | - | LISTA IND | CATALOGO | INICIAL |
| tab_documentos_cliente | - | LISTA IND | CATALOGO | INICIAL |
| tab_nombres_maquinas_nesp_corp | - | LISTA IND | CATALOGO | INICIAL |
| tab_roles_usuarios | - | LISTA DEP | CATALOGO | INICIAL |
| tab_canal_por_comercial | - | LISTA DEP | CATALOGO | INICIAL |
| tab_subsegmentos | - | LISTA DEP | CATALOGO | INICIAL |
| tab_leads | tab_cuentas | LISTA DEP | CON_TRAZABILIDAD | BASE |
| tab_visitas_por_cliente | tab_visitas_porCuenta | - | CON_TRAZABILIDAD | BASE |
| tab_seguimiento | tab_seguimiento_porCuenta | - | CON_TRAZABILIDAD | BASE |
| tab_cliente | tab_cuentas | - | CON_TRAZABILIDAD | BASE |
| tab_maquinas_por_cliente | tab_maquinas_porCuenta | - | CON_TRAZABILIDAD | BASE |
| tab_comentarios_maquinas | - | - | POR_VALIDAR | BASE |
| tab_documentos_por_cliente | tab_documentos_porCuenta | - | CON_TRAZABILIDAD | BASE |
| tab_registro_ventas | - | - | CON_TRAZABILIDAD | BASE |
| tab_ventas_por_cliente | - | - | CON_TRAZABILIDAD | BASE |
| tab_indicadores_comerciales | - | - | CON_TRAZABILIDAD | BASE |
| - | tab_oportunidades_cuenta | - | CON_TRAZABILIDAD | BASE |
| tab_comentarios_documentos | tab_hist_comentDocumentos | - | CON_TRAZABILIDAD | HISTORICA |
| - | tab_hist_cambioEstd_cuenta | - | CON_TRAZABILIDAD | HISTORICA |
| - | tab_hist_cambioEstd_maqu | - | CON_TRAZABILIDAD | HISTORICA |
| tab_pantallas | - | ELIMINAR | ELIMINAR | ELIMINAR |
| tab_maquinas_nesp_corp | - | ELIMINAR | ELIMINAR | ELIMINAR |
| tbl_meses | - | ELIMINAR | ELIMINAR | ELIMINAR |
| tab_tipo_cliente | - | ELIMINAR | ELIMINAR | ELIMINAR |