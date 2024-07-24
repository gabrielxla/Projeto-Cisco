CONFIGURAÇÃO DO VTY DO SWITCH E ROUTER

O cara do cabeamento conectou o Switch com o router usando a porta 24 como trunk

PRIMEIRA ETAPA: Configuração das Linhas Virtuais do Switch Cisco Catalyst 3560

!Acessando o modo Exec Privilegiado enable

!Acessar modo de configuração global
configure terminal

!Acessando as linhas virtuais
line vty 0 4
	
	!Habilitando senha do tipo Password Tipo-7
	password 123@senac
	
	!Forçando fazer login com usuário e senha local
	login local 
	
	!Sincronizando os logs na tela
	logging synchronous
	
	!Habilitando o tempo de inatividade do terminal
	exec-timeout 5 30
	
	!Configuração do tipo de protocolo de transporte de entrada
	transport input ssh
	
	!Saindo de todos os níveis
	end
!Salvando as configurações copy running-config startup-config

!Visualizando as configurações show running-config

CONFIGURAÇÃO DO SSH DO SWITCH E DO ROUTER

SEGUNDA ETAPA: Configuração das Linhas Virtuais do Router Cisco 2911

!Acessando o modo Exec Privilegiado enable

!Acessar modo de configuração global
configure terminal

!Acessando as linhas virtuais
line vty 0 4
	
	!Habilitando senha do tipo Password Tipo-7
	password 123@senac
	
	!Forçando fazer login com usuário e senha local
	login local 
	
	!Sincronizando os logs na tela
	logging synchronous
	
	!Habilitando o tempo de inatividade do terminal
	exec-timeout 5 30
	
	!Configuração do tipo de protocolo de transporte de entrada
	transport input ssh
	
	!Saindo de todos os níveis
	end
!Salvando as configurações copy running-config startup-config

!Visualizando as configurações show running-config

PORTAS VLAN DO SWITCH

Porta 2 VLAN 51 Gabriel

Porta 3 VLAN 52 Murillo

Porta 4 VLAN 53 lucas

Porta 5 VLAN 54 Carlos

Porta 6 VLAN 55 Wifi 05

IP DE CADA PC

ip address Gabriel: 172.16.51.254

ip address Murillo: 172.16.52.254

ip address Lucas: 172.16.53.254

ip address Carlos: 172.16.54.254
