# Reto 10 - Seguridad operacional con Fail2Ban

Proyecto integrador de Sistemas Operacionales (12997), Universidad El Bosque, 2026-2.
Autor: Cristian Vargas.

## Que contiene
- `configs/jail.local`: jails sshd y nginx-http-auth, whitelist 10.0.2.1, banaction ufw.
- `configs/99-hardening.conf`: PermitRootLogin no y MaxAuthTries 3.
- `configs/nginx-default-extracto.conf`: dos niveles de acceso (lector1 y admin1).
- `evidencias/`: capturas de pantalla numeradas (ver informe tecnico).

## Entorno
- 2 VMs Ubuntu Server 26.04.1 LTS en VirtualBox, Red NAT 10.0.2.0/24.
- f2b-servidor 10.0.2.7 (SSH, Nginx, Fail2Ban, UFW) y f2b-atacante 10.0.2.8.

