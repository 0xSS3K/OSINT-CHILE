# OSINT Chile: Guía de Recursos 🕵️🇨🇱

https://pastebin.com/rG93B3yM



¡Buenas! Esta es una pequeña recopilación de recursos y dorks para quienes se inician o quieren tener a mano algunos trucos de OSINT enfocados en Chile. No es una biblia, pero seguro te da un buen punto de partida. Igual, debo decir que hacer OSINT no es andar copiando y pegando dorks, links y comandos en un CLI o navegador. El fin de todo esto es lograr unir los puntos y adaptarte a lo que vas recopilando. Acá mostraré una serie de lugares a los que deberías mirar, o como mínimo saber de su existencia (en mi opinión). Y, como se menciona anteriormente, esto es una guía enfocada al OSINT en CHILE, haciendo uso de herramientas CHILENAS.

## 🎯 Usando los dorks de Google

Los dorks son búsquedas avanzadas en Google. Aquí te dejo algunos listos para usar (o casi). Recuerda reemplazar los placeholders como `"nombre apellido"` o `<palabra_clave>`.

### 📄 Dork Genérico para Archivos

Si no sabes por dónde empezar, este one-liner dork busca una variedad de tipos de archivo en un sitio específico relacionados con un nombre.

`site:SITIO_WEB_AQUI "NOMBRE APELLIDO" filetype:pdf OR filetype:xml OR filetype:txt OR filetype:doc OR filetype:docx OR filetype:xlsx OR filetype:odt OR filetype:rtf OR filetype:html OR filetype:htm OR filetype:csv OR filetype:ods OR filetype:mdb OR filetype:accdb OR filetype:sql OR filetype:jpg OR filetype:png OR filetype:jpeg OR filetype:gif OR filetype:mp4 OR filetype:avi OR filetype:mov OR filetype:mp3 OR filetype:wav OR filetype:eml OR filetype:json OR filetype:ini OR filetype:conf OR filetype:log OR filetype:backup OR filetype:zip OR filetype:rar OR filetype:7z` 

**Consejo:** 
Cambia `SITIO_WEB_AQUI` por el dominio que te interese (ej: `gob.cl`). En mi experiencia, este tipo de dorks son geniales para encontrar información de estudiantes :)

### 🎓 Universidades

#### Universidades Tradicionales del CRUCH
(_Las universidades CRUCH son las 30 instituciones de educación superior más reconocidas en Chile, tanto públicas como privadas, que forman parte del Consejo de Rectoras y Rectores de las Universidades Chilenas_)

`(site:uchile.cl OR site:uc.cl OR site:usach.cl OR site:uv.cl OR site:udec.cl OR site:uach.cl OR site:usm.cl OR site:ucn.cl OR site:ucsc.cl OR site:uct.cl OR site:ucm.cl OR site:utalca.cl OR site:ubiobio.cl OR site:ufro.cl OR site:ulagos.cl OR site:umag.cl OR site:uda.cl OR site:userena.cl OR site:upla.cl OR site:umce.cl OR site:utem.cl OR site:unap.cl OR site:uoh.cl OR site:uaysen.cl OR site:uantof.cl) "nombre apellido"`

#### Universidades Privadas Importantes
`(site:uai.cl OR site:udd.cl OR site:uandes.cl OR site:udp.cl OR site:uahurtado.cl OR site:umayor.cl OR site:unab.cl OR site:uss.cl OR site:uft.cl OR site:ucentral.cl OR site:autonoma.cl OR site:ubo.cl OR site:udla.cl OR site:ust.cl OR site:uamericas.cl) "nombre apellido"`

#### Otras Universidades e Instituciones
`(site:academia.cl OR site:usek.cl OR site:unicit.cl OR site:uvirtual.cl OR site:upv.cl OR site:umc.cl OR site:uniacc.cl OR site:ulare.cl OR site:ucab.cl OR site:ucsh.cl OR site:gabrielamistral.cl OR site:ubartolome.cl OR site:ipg.cl OR site:adventista.cl OR site:ubolivariana.cl OR site:uisek.cl OR site:ularepublica.cl OR site:uvina.cl OR site:udesarrollo.cl OR site:ufinisterrae.cl OR site:umartin.cl) "nombre apellido"`

### 📚 Repositorios Universitarios (Tesis y Documentos)

Ideal para encontrar investigaciones, tesis y documentos académicos. Solo remplaza "nombre apellido".

#### Universidades Estatales, CRUCH Tradicionales y Regionales Principales
`(site:repositorio.uchile.cl OR site:cybertesis.uchile.cl OR site:bdigital.uchile.cl OR site:repositorio.uc.cl OR site:repositorio.usach.cl OR site:repositorio.udec.cl OR site:repositorio.uv.cl OR site:cybertesis.uach.cl OR site:repositorio.uach.cl OR site:repositorio.usm.cl OR site:repositorio.ucn.cl OR site:repositorio.ucsc.cl OR site:repositorio.uct.cl OR site:repositorio.ucm.cl OR site:repositorio.utalca.cl OR site:repositorio.ubiobio.cl OR site:repositorio.ufro.cl OR site:repositorio.ulagos.cl OR site:repositorio.umag.cl OR site:repositorio.uda.cl OR site:repositorio.userena.cl OR site:repositorio.upla.cl OR site:repositorio.umce.cl OR site:repositorio.utem.cl OR site:repositorio.uantof.cl OR site:repositorio.uoh.cl OR site:repositorio.uaysen.cl) "nombre apellido" filetype:pdf`

#### Universidades Privadas y Otras Instituciones
`(site:repositorio.uai.cl OR site:repositorio.udd.cl OR site:repositorio.uandes.cl OR site:repositorio.udp.cl OR site:repositorio.uahurtado.cl OR site:repositorio.umayor.cl OR site:repositorio.unab.cl OR site:repositorio.uss.cl OR site:repositorio.uft.cl OR site:repositorio.ucentral.cl OR site:repositorio.autonoma.cl OR site:bibliotecadigital.ubo.cl OR site:repositorio.academia.cl OR site:repositorio.umc.cl OR site:repositorio.ucsh.cl) "nombre apellido" filetype:pdf`

### 🏢 Empresas y Negocios

#### Diario Oficial
Busca constituciones de empresas, modificaciones, etc.

`site:diariooficial.interior.gob.cl "NOMBRE EMPRESA" OR "NOMBRE REPRESENTANTE" OR "RUT EMPRESA"`
**Nota:** Adapta el término de búsqueda según lo que necesites.


### 📸 Redes Sociales

_La verdad es que hay demasiado contenido en internet sobre OSINT a RRSS, por lo que me remetiré a dejarte este único dork que me parece valioso y el cual puedes modificar para cualquier RS :P_

#### Instagram
El típico "aaaaah" dork para Instagram.
`site:instagram.com "NOMBRE APELLIDO" Chile`

### 👣 Huellas Digitales (Noticias, Archivos, Genealogía)

Para rastrear menciones en medios, documentos históricos y árboles genealógicos. Dale una oportunidad. Yo mismo he encontrado cosas sobre mí usando estos dorks que no pensé que estuvieran por ahí...

`site:www.elmercurio.com "nombre apellido"`
`site:www.latercera.com "nombre apellido"`
`site:www.biobiochile.cl "nombre apellido"`
`site:ciperchile.cl "nombre apellido"`
`site:bibliotecanacionaldigital.gob.cl "nombre apellido"`
`site:memoriachilena.gob.cl "nombre apellido"`
`site:archivonacional.gob.cl "nombre apellido"`
`site:documentos.archivonacional.cl "nombre apellido"`
`site:familysearch.org "nombre apellido" Chile`
`site:genealog.cl "nombre apellido"`

### 🏥 Salud y Educación (Gobierno)

Documentos oficiales relacionados con personas en los ministerios.
(site:gob.cl OR site:mineduc.cl OR site:minsal.cl) "NOMBRE APELLIDO" filetype:pdf OR filetype:doc
### 💼 LinkedIn

Perfiles profesionales.
`site:linkedin.com/in OR site:linkedin.com/pub "NOMBRE APELLIDO" "Chile"`

### 🛡️ Fuerzas Armadas
_Este dork es simplemente oro ^^. Aquí metes a la Escuela de Grumetes, la Fuerza Aérea de Chile, al Estado Mayor Conjunto... En fin, úsalo._
`site:*.mil.cl "NOMBRE APELLIDO"`

### 🤫 Información Sensible (¡Con Cuidado!)

Estos dorks `intext:` buscan texto específico dentro de las páginas. Úsalos con responsabilidad (No👿)

`intext:"Rut: EL_RUT_AQUI"intext:"EL_NOMBRE_AQUI"intext:"Contraseña" "NOMBRE APELLIDO" OR "CORREO_ELECTRONICO"intext:"NUMERO_DE_TELEFONO"`

### 🚘 Información vehicular

* **Auto Seguro `https://www.autoseguro.gob.cl/`**: Para consultar si un vehículo tiene encargo por robo 
* **Registro Nacional de Transporte Público `https://apps.mtt.cl/consultaweb/`**: Para verificar la inscripción de vehículos de transporte público, escolar o de carga
* **Consulta Infracciones por Cámaras `http://rrvv.fiscalizacion.cl/`**: Para revisar si un vehículo tiene infracciones captadas por el sistema de cámaras de fiscalización.
* **ChileAtiende `https://www.chileatiende.gob.cl/fichas/3412-certificados-asociados-a-vehiculos-motorizados-y-hoja-de-vida-del-conductor`**: Portal que centraliza la información sobre cómo obtener certificados y realizar trámites vehiculares *(aunque la obtención de los documentos oficiales usualmente tiene un costo)*.
* ☢️ **Volante o Maleta `https://www.volanteomaleta.com/`**: Permite obtener datos básicos del vehículo como marca, modelo, año, número de motor, y el nombre y RUT del propietario actual. ☢️
* **Autofact `https://www.autofact.cl/consultar-patente-auto`**: Ofrece un informe básico y limitado con algunos datos del vehículo.

## 🌐 Sitios Web Útiles

Aquí una lista de páginas que te pueden servir un montón :) (sobre todo las primeras)

* **Registro Civil (`registrocivil.cl`)**: Verificación de identidad, estado vital, lazos familiares, historial legal básico.

* **SERVEL (`servel.cl`, `consulta.servel.cl`)**: Confirmación de registro electoral, vinculación geográfica, historial político/candidaturas, posible fuente de domicilio.
  
* **Poder Judicial (`pjud.cl`)**: Historial de participación en procesos judiciales, identificación de contrapartes, indicadores de disputas o problemas financieros (cobranzas).
  
* **SII (`sii.cl`)**: Verificación de existencia y estado tributario de empresas; vinculación indirecta de individuos a través de roles corporativos.
  
* **Registro de Empresas y Sociedades (`registrodeempresasysociedades.cl`)**: Identificación de propiedad empresarial, roles directivos, estructura societaria. (Usa el link directo: `https://www.registrodeempresasysociedades.cl/BuscarActuaciones2.aspx`)
  
* **ChileCompra / Mercado Público (`chilecompra.cl`, `mercadopublico.cl`, `datos-abiertos.chilecompra.cl`)**: Identificación de actividad como proveedor del Estado, análisis de contratos y montos, identificación de empresas asociadas.
  
* **Búsqueda de Abogados PJUD (`pjud.cl/transparencia/busqueda-de-abogados`)**: Verificación de credenciales legales, estado de habilitación profesional.
  
* **Colegio de Abogados (`colegioabogados.cl`, `archivo.colegioabogados.cl`)**: Identificación de afiliación gremial, posibles contactos y especializaciones.
  
* **Colegio de Ingenieros (`ingenieros.cl/actualiza-tus-datos/`)**: Verificación de credenciales de ingeniería, identificación de expertos.
  
* **Registro Colegiados Arquitectos (`registrocolegiados.cl`)**: Verificación de credenciales y estado de colegiatura. (Ej: `https://registrocolegiados.cl/resultado.php?rut=RUT_AQUI&ica=`)
  
* **Repositorio ANID (`repositorio.anid.cl`)**: Producción científica, áreas de investigación, colaboradores. (Ej: `https://repositorio.anid.cl/search?query=PALABRA_CLAVE`)
  
* **Investigadores ANID (`investigadores.anid.cl/es/public_search/results`)**: Búsqueda de expertos por disciplina, trayectoria y redes.

---

Si tienes dudas o aportes, ¡contáctame! Puedes encontrarme en IG: `_ss3k_`

¡Suerte con tus búsquedas!
