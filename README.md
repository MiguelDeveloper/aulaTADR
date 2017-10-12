# aulaTADR

configure terminal

vlan 2

name aluno

exit

vlan 3

name professores

exit

vlan 10

name convidado

exit

interface range fastEthernet 0/5-8

switchport access vlan 2

exit

interface range fastEthernet 0/9-12
switchport access vlan 3
exit
interface range fastEthernet 0/13-24
switchport access vlan 10
exit
interface vlan 1
no shutdown
exit
interface vlan 2
no shutdown
exit
interface vlan 3
no shutdown
exit
interface vlan 10
no shutdown
exit
