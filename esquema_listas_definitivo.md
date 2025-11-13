# Esquema de Listas - Modelo Relacional con Lookups, seleccion y campos de opcion

1. **tab_roles**
Columna (hacer clic para editar)	Tipo	Requerida

rol	Una línea de texto	
pk_id_rol	Número	


2. **tab_roles_usuarios**

Columna (hacer clic para editar)	Tipo	Requerida

id_rol	Número	
correo	Una línea de texto

3. **tab_canales**

Columna (hacer clic para editar)	Tipo	Requerida
canal	Una línea de texto	
id_canal	Número	


4. **tab_segmentos**

Columna (hacer clic para editar)	Tipo	Requerida
segmento	Una línea de texto	
id_segmento	Número	


5. **tab_subsegmentos**

Columna (hacer clic para editar)	Tipo	Requerida

sub_segmento	Una línea de texto	
id_sub_segmento	Número	
fk_id_segmento	Número (id del segmento relacionado)

6. **tab_ciudades**

Columna (hacer clic para editar)	Tipo	Requerida
Departamento	Una línea de texto	
Ciudad	Una línea de texto	


7. **tab_documentos_cliente**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
nombre_documento	Una línea de texto	
tipo_documento	Número (1: Creacion de cliente y 2: Solicitud de credito)
nombre_tipo_documento	Una línea de texto	
cantidad_de_documentos	Número	
nombre_carpeta_documento	Una línea de texto	
mostrar_finanzas	Número (0: false y 1: true)
RequiereAprobacionOfiCumpl	Número (0: false y 1: true)	
RequiereAprobacionBEO	Número (0: false y 1: true)


8. **tab_nombres_maquinas_nesp_corp**

Columna (hacer clic para editar)	Tipo	Requerida
nombre_maquina	Una línea de texto	
id_maquina	Número 
consumo_minimo_maquina	Número	
Descripcion_maquina	Varias líneas de texto

9. **tab_oportunidad**

Columna (hacer clic para editar)	Tipo	Requerida

ID Autogenerado por sherepoint
oportunidad	Una línea de texto	
Descripcion_oport	Una línea de texto	

10.  **tab_estados_negociaciones**

Columna (hacer clic para editar)	Tipo	Requerida
estado_negociacion	Una línea de texto	
id_estado_negociacion	Número	

11.  **tab_estados_maquinas**

Columna (hacer clic para editar)	Tipo	Requerida
estado_maquinas	Una línea de texto	
id_estados_maquinas	Número	


12.  **tab_estados_documentos**

Columna (hacer clic para editar)	Tipo	Requerida
estados_documentos	Una línea de texto	
id_estado_documento	Número	


13.  **tab_tipos_visita**

Columna (hacer clic para editar)	Tipo	Requerida
tipo_Visita	Una línea de texto	
id_tipo_visi	Número	


14.  **tab_canal_por_comercial**

Columna (hacer clic para editar)	Tipo	Requerida
id_canal	Número	(canal relacionado al comercial segun el id tomado de la lista "tab_canales")
canal	Una línea de texto	
correo_comercial Una línea de texto	(correo del comercial asignado al canal)	


15.   **tab_cuentas**

Columna (hacer clic para editar)	Tipo	Requerida

NIT	Una línea de texto	
RazonSocial	Una línea de texto	
Id_nesp-corp	Número	
FechaPasoAProspecto	Fecha y hora	
FechaPasoACliente	Fecha y hora	
NombreContacto	Una línea de texto	
ApellidosContacto	Una línea de texto	
CargoContacto	Una línea de texto	
EmailContacto	Una línea de texto	
ComercialAsignado	Una línea de texto	
ComercialAsignado_Nombre	Una línea de texto	
CupoSolicitado	Moneda	
RequiereCredito	Número	(0: false y 1: true)
PlazoCredito	Elección	
Tarifa	Número	
RequiereDocumentos	Número	(0: false y 1: true)
NombreCarpetaSharePoint	Una línea de texto	
CarpetaCreada	Número	(0: false y 1: true)
DocumentosAprobadosBackOffice	Número	(0: false y 1: true)
DocumentosAprobadosFinanzas	Número	(0: false y 1: true)
FechaCreacionLead	Fecha y hora	
Ultima_actualizacion_cuenta	Fecha y hora	
estado_interes	Una línea de texto	(Puede ser: Interesado, Por definir, Descartado)
EstadoCuenta	Número	(Opciones: 1: Lead 2: Prospecto 3: Cliente)
fk_estado_negociacion	Número	(Relacionado a la lista "tab_estados_negociaciones")
Canal	Una línea de texto	(Relacionado a la lista "tab_canales")
Segmento	Una línea de texto	(Segmento de mercado
Relacionado a la lista "tab_segmentos")
Subsegmento	Una línea de texto (Relacionado a la lista "tab_subsegmentos")	
Ciudad	Una línea de texto	(Relacionado a la lista "tab_ciudades")
Status_cliente	Número	(0: false y 1: true)
EstadoCuenta_Detail	Una línea de texto	(Puede ser: Lead, Prospecto o Cliente)
ModalidadPago	Una línea de texto (Puede ser: Contado o Crédito)
EvaluacionSagrilaft	Número (0: false y 1: true)

16.   **tab_hist_cambioEstd_cuenta**

Columna (hacer clic para editar)	Tipo	Requerida
UsuarioResponsable	Una línea de texto	
UsuarioResponsable_Nombre	Una línea de texto	
DiasDuracionEstadoAnterior	Número	
FechaCambioProspecto	Fecha y hora	
FechaCambioCliente	Fecha y hora	
fk_cuenta	Número	(Relacionado a la lista "tab_cuentas")
Cuenta_RazonSocial	Una línea de texto	
EstadoAnterior	Número	(Puede ser: 1: Lead o 2: Prospecto)
EstadoNuevo	Número (Puede ser: 1: Lead o 2: Prospecto y 3: Cliente)
FechaCreacion	Fecha y hora

17.   **tab_seguimiento_porCuenta**

Columna (hacer clic para editar)	Tipo	Requerida
FechaSeguimiento	Fecha y hora	
ComercialResponsable	Una línea de texto	
ComercialResponsable_Nombre	Una línea de texto	
Anotaciones	Una línea de texto	
Observaciones	Varias líneas de texto	
RequiereAccion	Número	
FechaProximoSeguimiento	Fecha y hora	
EstadoSeguimiento	Número	
fk_cuenta	Número	
Cuenta_RazSoc	Una línea de texto	
EstadoCuentaEnSeguimiento	Número 


18.     **tab_oportunidades_cuenta**

Columna (hacer clic para editar)	Tipo	Requerida
FechaIdentificacion	Fecha y hora	
ComercialIdentifica	Una línea de texto	
ComercialIdentifica_Nombre	Una línea de texto	
Detalle	Una línea de texto	
Construccion_marca	Varias líneas de texto	
fk_cuenta	Número	
Cuenta_RazSoc	Una línea de texto	
EstadoCuentaInicial	Número	
fk_TipoOportunidad	Número


19.  **tab_maquinas_porCuenta**

Columna (hacer clic para editar)	Tipo	Requerida
FechaSolicitud	Fecha y hora	
ComercialSolicitante	Una línea de texto	
ComercialSolicitante_Nombre	Una línea de texto	
ConsumoMinimoSugerido	Número	
MesColocacionEstimado	Elección	
TieneCondicionesEspeciales	Número	
DescripcionCondiciones	Varias líneas de texto	
AprobadoBackOffice	Número	
UsuarioAprobadorBackOffice	Una línea de texto	
FechaAprobacionBackOffice	Fecha y hora	
AprobadoSupply	Número	
FechaAprobacionSupply	Fecha y hora	
UsuarioAprobadorSupply	Una línea de texto	
SerialMaquina	Una línea de texto	
FechaAsignacionSerial	Fecha y hora	
FechaInstalacion	Fecha y hora	
DireccionInstalacion	Varias líneas de texto	
NotasSupply	Varias líneas de texto	
FechaUltimoMantenimiento	Fecha y hora	
ProximoMantenimiento	Fecha y hora	
FechaRetiro	Fecha y hora	
MotivoRetiro	Varias líneas de texto	
fk_cuenta	Una línea de texto	
Cuenta_RazSoc	Una línea de texto	
fk_tipoMaquina	Número	
fk_estadoMaquina	Número	
EstadoCuentaAlSolicitar	Número	
Status_maquina	Número	
EstadoActualCuenta	Número	
maquina	Una línea de texto	
Status_maquina_detail	Una línea de texto


20.  **tab_hist_cambioEstd_maqu**

Columna (hacer clic para editar)	Tipo	Requerida
FechaCambio	Fecha y hora	
UsuarioResponsable	Una línea de texto	
UsuarioResponsable_Nombre	Una línea de texto	
Comentario	Varias líneas de texto	
MaquinaAnterior	Una línea de texto	
MaquinaNueva	Una línea de texto	
ConsumoInicial	Número	
ConsumoNuevo	Número	
FechaRegistroMaquina	Fecha y hora	
Cuenta	Una línea de texto	
fk_cuenta	Número	
StatusMaquina	Número	
fk_EstadoAnterior	Número	
fk_EstadoNuevo	Número	
fk_id_Maquina	Número

21.  **tab_documentos_porCuenta**

Columna (hacer clic para editar)	Tipo	Requerida
URLDocumento	Varias líneas de texto	
FechaCarga	Fecha y hora	
UsuarioCarga	Una línea de texto	
UsuarioCarga_Nombre	Una línea de texto	
AprobadoBackOffice	Número	
FechaAprobacionBackOffice	Fecha y hora	
UsuarioAprobadorBackOffice	Una línea de texto	
AprobadoFinanzas	Número	
FechaAprobacionFinanzas	Fecha y hora	
UsuarioAprobadorFinanzas	Una línea de texto	
AprobacionOficialCumplimiento	Número	
AprobacionBEO	Número	
Nombre_documento	Una línea de texto	
Nombre_carpeta_cliente	Una línea de texto	
fk_cuenta	Número	
fk_tipoDocumento	Número	
tipoDocumento_detail	Una línea de texto	
fk_estadoDocumento	Número

22.   **tab_hist_comentDocumentos**

Columna (hacer clic para editar)	Tipo	Requerida
UsuarioComenta	Una línea de texto	
UsuarioComenta_Nombre	Una línea de texto	
FechaComentario	Fecha y hora	
Comentario	Varias líneas de texto	
fk_id_regisDoc	Número	
fk_cuenta	Número	
fk_rolUsuario	Número	
TipoComentario	Número	
Cuenta_RazSoc	Una línea de texto

23.  **tab_visitas_porCuenta**

Columna (hacer clic para editar)	Tipo	Requerida
Título	Una línea de texto	
Cuenta	Búsqueda	
TipoVisita	Búsqueda	
FechaProgramada	Fecha y hora	
FechaRealizacion	Fecha y hora	
UsuarioResponsable	Una línea de texto	
UsuarioResponsable_Nombre	Una línea de texto	
DireccionVisita	Varias líneas de texto	
EstadoVisita	Elección	
ObservacionesComercial	Varias líneas de texto	
ObservacionesSupply	Varias líneas de texto	
FechaCierre	Fecha y hora	
RequiereAccionCorrectiva	Sí o No	
Modificado	Fecha y hora	
Creado	Fecha y hora	
Creado por	Una línea de texto	
Modificado por	Una línea de texto