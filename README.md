# homelab-ops

Writeups de operación y hardening sobre un servidor Ubuntu propio, usado como laboratorio de Blue Team.

Cada writeup documenta un caso real: qué se encontró, cómo se verificó, qué se corrigió y qué quedó pendiente. Los errores y los falsos positivos forman parte del registro, porque son la parte que más enseña.

## Writeups

| # | Tema | Qué muestra |
|---|---|---|
| 02 | [Hermes Agent con mínimo privilegio](docs/02-hermes-agent-instalacion-segura.md) | Aislar un agente de IA con acceso a terminal: escalada vía grupo `lxd`, usuario dedicado, recorte de herramientas y una prueba que demostró que el agente reportaba como guardado algo que no estaba en disco. |

## Criterios

- **Evidencia antes que afirmaciones.** Cada conclusión se apoya en una salida de comando o en el estado real del sistema, no en lo que una herramienta dice que hizo.
- **Pendientes explícitos.** Lo que no se verificó figura como pendiente, no como resuelto.
- **Sin datos de infraestructura.** Hostnames, IPs, usuarios y credenciales se omiten o se tapan en texto y capturas.
- **Solo trabajo personal.** Nada de lo publicado acá proviene de entornos laborales.

## Entorno

- Ubuntu Server sobre hardware reciclado, administrado por SSH.
- Docker (rootless) y Docker Compose para servicios.
