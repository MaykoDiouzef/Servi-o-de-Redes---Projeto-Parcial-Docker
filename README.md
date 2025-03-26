Projeto Parcial
Implementação de Serviços de Gestão de Redes de Computadores em Docker

Professor: Roitier campos Gonçalves
Semestre: 2025/01
Turma: Serviços de Redes de Computadores - 5° Período
Valor: 5 Pontos
Grupo: 3 Pessoas
Data da Entrega: 29/04/2025
Objetivo  
Implementar uma infraestrutura de rede corporativa básica, integrando serviços essenciais como DNS, DHCP, Firewall, LDAP, SAMBA, FTP, Apache/NGINX, além de outros serviços complementares para gestão e segurança.

Escopo do Projeto  
1. Serviços Básicos de Rede  
- DNS (Bind9 ou dnsmasq)  
  - Configurar um servidor DNS interno para resolução de nomes local e encaminhamento externo.  
  - Criar zonas (forward e reverse) para domínios internos.  

- DHCP (ISC DHCP ou dhcpd)  
  - Configurar um servidor DHCP para atribuição automática de IPs.  
  - Reservar IPs para servidores e dispositivos críticos.  

- Firewall (iptables/nftables ou UFW)  
  - Implementar regras de filtro para proteger a rede.  
  - Permitir apenas tráfego necessário (SSH, HTTP, HTTPS, LDAP, etc.).  

- LDAP (OpenLDAP ou 389 Directory Server)  
  - Configurar um servidor LDAP para autenticação centralizada.  
  - Criar usuários e grupos para acesso a serviços.  

- SAMBA  
  - Configurar compartilhamento de arquivos em rede (Windows/Linux).  
  - Integrar com LDAP para autenticação unificada.  

- FTP (vsftpd ou ProFTPD)  
  - Configurar um servidor FTP seguro (SFTP/FTPS).  
  - Definir acesso restrito a usuários autorizados.  

- Web Server (Apache ou NGINX)  
  - Hospedar um site interno (página de boas-vindas).  
  - Configurar Virtual Hosts para múltiplos serviços.  

Requisitos Técnicos  
- Implementar em Docker
- Topologia de Rede:  
  - Pelo menos 2 sub-redes (ex: 192.168.1.0/24 para servidores e 192.168.2.0/24 para clientes).  
  - Um container roteador funcionando como entrada/saida para a rede de containers
Dica: Use Ansible para otimizar a configuração
Etapas de Implementação  
1. Planejamento  
   - Definir endereçamento IP, nomes de domínio e estrutura de usuários.  
   - Documentar a topologia da rede.  

2. Configuração dos Serviços  
   - Instalar e configurar cada serviço seguindo boas práticas de segurança.  

3. Testes e Integração  
   - Verificar comunicação entre servidores e clientes.  
   - Testar autenticação LDAP, acesso a compartilhamentos e resolução DNS.  

4. Documentação Final  
   - Relatório detalhado com configurações, problemas enfrentados e soluções.  
   - Diagrama de rede e instruções de uso.  

Entrega do Projeto  
Relatório Técnico no GitHub  
- Descrição da infraestrutura.  
- Configurações principais (ex: arquivos de configuração importantes).  
- Screenshots de testes funcionando.  
- Scripts de automação para facilitar a implantação.  
- Apresentação: Explicação do projeto em execução. O projeto deve ser executado com apenas 1 comando. 
