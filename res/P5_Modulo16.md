# Parte 5 modulo 16

# Autenticación (AuthN).
La autenticación es el proceso de establecimiento de la identidad de una persona o servicio que quiere acceder a un recurso. Implica el acto de solicitar a un usuario credenciales legítimas y proporciona la base para la creación de una entidad de seguridad para el control de identidad y de acceso. Determina si el usuario es quien dicen ser.

# Autorización (AuthZ)
La autenticación establece la identidad del usuario, pero la autorización es el proceso de establecer el nivel de acceso que tiene una persona o un servicio autenticados. Especifica a qué datos puede acceder y qué puede hacer con ellos.

![image](https://user-images.githubusercontent.com/86896526/126702702-76dc7371-4f70-4bae-a1a3-aeb1d3b3cdc3.png)

# ¿Diferencias entre Azure Active Directory y Azure AD?
Microsoft presentó Active Directory en Windows 2000 para ofrecer a las empresas la capacidad de administrar varios sistemas y componentes de la infraestructura local mediante una única identidad por usuario.
Azure AD es un servicio de administración de acceso e identidades basado en la nube de Microsoft.
Si protege las identidades de forma local con Active Directory, Microsoft no supervisa los intentos de inicio de sesión. Si conecta Active Directory con Azure AD, Microsoft puede detectar intentos de inicio de sesión sospechosos para ayudarle a proteger su entorno sin costo adicional. 


## Azure AD
### ¿Quien lo puede usar?
- Administradores de TI
Los administradores pueden usar Azure AD para controlar el acceso a las aplicaciones y los recursos en función de sus requisitos empresariales.

- Desarrolladores de aplicaciones
Con Azure AD, los desarrolladores pueden agregar funcionalidad a las aplicaciones que compilan mediante un enfoque basado en estándares. Por ejemplo, pueden agregar funcionalidad de SSO a una aplicación o habilitar una aplicación para que funcione con las credenciales existentes de un usuario.

- Usuarios
Los usuarios pueden administrar sus identidades. Por ejemplo, el autoservicio de restablecimiento de contraseña permite a los usuarios cambiar o restablecer su contraseña sin intervención de un administrador de TI ni del departamento de soporte técnico.

- Suscriptores de servicios en línea
Los suscriptores de Microsoft 365, Microsoft Office 365, Azure y Microsoft Dynamics CRM Online ya usan Azure AD.

Un inquilino es la representación de una organización. Suele estar separado de otros inquilinos y tiene su propia identidad.

Cada inquilino de Microsoft 365, Office 365, Azure y Dynamics CRM Online es automáticamente un inquilino de Azure AD.

### ¿Qué servicios proporciona?

- Autenticación
Esto incluye la comprobación de la identidad para acceder a aplicaciones y recursos. 

- Inicio de sesión único
Gracias al SSO, los usuarios tienen que recordar un solo identificador y una sola contraseña para acceder a varias aplicaciones. Una sola identidad está asociada a un usuario, lo que simplifica el modelo de seguridad.

- Administración de aplicaciones
puede administrar las aplicaciones en la nube y locales.

### ¿Qué tipos de recursos se pueden proteger con Azure AD?
Azure AD ayuda a los usuarios a acceder a recursos tanto internos como externos.

Los recursos externos podrían ser Microsoft Office 365, Azure Portal y miles de aplicaciones de software como servicio (SaaS).

Los recursos internos podrían ser aplicaciones de la red corporativa y la intranet, junto con las aplicaciones en la nube desarrolladas por la organización.

# ¿Qué es el inicio de sesión único?
El inicio de sesión único permite a los usuarios iniciar sesión una vez y utilizar esa credencial para acceder a varios recursos y aplicaciones de distintos proveedores.
Con SSO, tan solo debe recordar un ID y una contraseña. El acceso a todas las aplicaciones se concede a una única identidad que está asociada a un usuario, lo que simplifica el modelo de seguridad. A medida que los usuarios cambian los roles o dejan una organización, el acceso está asociado a una única identidad. Este cambio reduce considerablemente el esfuerzo necesario para cambiar o deshabilitar cuentas. Usar SSO en las cuentas permite a los usuarios administrar más fácilmente su identidad y aumenta la capacidad en términos de seguridad.

## ¿Cómo se puede conectar Active Directory con Azure AD?
Azure AD Connect sincroniza las identidades de usuario entre la instalación local de Active Directory y Azure AD. Azure AD Connect sincroniza los cambios entre ambos sistemas de identidades, para que pueda usar características como SSO, la autenticación multifactor y el autoservicio de restablecimiento de contraseña en ambos sistemas. El autoservicio de restablecimiento de contraseña impide que los usuarios utilicen contraseñas cuya peligrosidad es conocida.
![image](https://user-images.githubusercontent.com/86896526/126704955-1b555238-35af-477d-9ddd-b65ecccab247.png)


# ¿Qué es la autenticación multifactor?
La autenticación multifactor es un proceso en el que durante el inicio de sesión de un usuario se le solicita una forma adicional de identificación. Entre los ejemplos se incluye un código en su teléfono móvil o un examen de las huellas dactilares.
La autenticación multifactor proporciona seguridad adicional a las identidades, ya que se requieren dos o más elementos para una autenticación completa.
- Algo que el usuario conoce
Se podría tratar de una dirección de correo electrónico y una contraseña.
- Algo que el usuario tiene
Se podría tratar de un código que se envía al teléfono móvil del usuario.
- Algo que el usuario es
Suele ser algún tipo de propiedad biométrica, como la huella dactilar o el escaneo facial utilizados en muchos dispositivos móviles.


## ¿Qué es Azure AD Multi-Factor Authentication?
Azure AD Multi-Factor Authentication es un servicio de Microsoft que proporciona funcionalidades de autenticación multifactor. Azure AD Multi-Factor Authentication permite a los usuarios elegir una forma adicional de autenticación durante el inicio de sesión, como una llamada de teléfono o una notificación de aplicación móvil.

- Azure Active Directory
La edición gratuita de Azure Active Directory habilita Azure AD Multi-Factor Authentication para los administradores con el nivel de acceso de Administrador global, a través de la aplicación Microsoft Authenticator, una llamada de teléfono o un código por SMS. También puede aplicar Azure AD Multi-Factor Authentication a todos los usuarios solo a través de la aplicación Microsoft Authenticator. Para ello, se deben habilitar los valores predeterminados de seguridad en el inquilino de Azure AD.
Azure Active Directory Premium (licencias P1 o P2) permite una configuración exhaustiva y detallada de Azure AD Multi-Factor Authentication a través de directivas de acceso condicional (como se explicará en breve).

- Autenticación multifactor para Office 365
La suscripción a Office 365 incluye un subconjunto de funcionalidades de Azure AD Multi-Factor Authentication.

# ¿Qué es el acceso condicional?
El acceso condicional es una herramienta que usa Azure Active Directory para permitir (o denegar) el acceso a los recursos en función de señales de identidad. Estas señales incluyen quién es el usuario, dónde se encuentra y desde qué dispositivo solicita el acceso.

Con el acceso condicional, los administradores de TI pueden:
- permitir a los usuarios ser productivos en cualquier momento y lugar;
- proteger los recursos de la organización.

## ¿Cuándo se puede usar el acceso condicional?
El acceso condicional resulta útil en los casos siguientes:

- Requerir la autenticación multifactor para acceder a una aplicación.
Puede configurar si todos los usuarios necesitan la autenticación multifactor o solo algunos, como los administradores.
También puede configurar si la autenticación multifactor se aplica al acceso desde todas las redes o solo desde redes que no son de confianza.

- Para requerir el acceso a los servicios solo a través de aplicaciones cliente aprobadas.
Por ejemplo, podría permitir que los usuarios accedan a los servicios de Office 365 desde un dispositivo móvil siempre que usen aplicaciones cliente aprobadas, como Outlook Mobile.

- Exija que los usuarios accedan a la aplicación solo desde dispositivos administrados.
Un dispositivo administrado es un dispositivo que cumple los estándares de seguridad y cumplimiento normativo.

- Para bloquear el acceso desde orígenes que no son de confianza, como ubicaciones desconocidas o inesperadas. 


# Extra
- La autenticación (AuthN) establece la identidad del usuario.
- La autorización (AuthZ) establece el nivel de acceso que tiene un usuario autenticado.
- El inicio de sesión único (SSO) permite a los usuarios iniciar sesión una vez y utilizar esa credencial para acceder a varios recursos y aplicaciones.
- Azure Active Directory (Azure AD) es un servicio de administración de acceso e identidades basado en la nube. Azure AD permite a una organización controlar el acceso a las aplicaciones y los recursos en función de sus requisitos empresariales.
- Azure AD Multi-Factor Authentication proporciona seguridad adicional para las identidades, ya que se requieren dos o más elementos para una autenticación completa. En general, la autenticación multifactor puede incluir algo que el usuario sabe, algo que tiene y algo que es.
- El acceso condicional es una herramienta que Azure AD usa para permitir o denegar el acceso a los recursos en función de señales de identidad, como la ubicación del usuario.
