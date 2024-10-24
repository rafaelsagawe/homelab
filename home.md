O objetivo deste sistema é ser o servidor de aplicação da rede do home lab.

Para os testes iniciais foi usado o netbook da Asus EEEPC com sistema Ubuntu 24.04 LTS

## Mantendo o sistema ligado com a tela abaixada

~~~~shell
# sudo nano /etc/systemd/logind.conf

            HandleLidSwitch=ignore

# systemctl restart systemd-logind.service
~~~~

## Acesando remotamente

Para acessar remotamente as funcionalidades do servido foi instalado o sistema de VPN TailScale

~~~~shell
# curl -fsSL https://tailscale.com/install.sh | sh
~~~~

Para logar na conta foi usado o IP informado pela instalação.

## Aplicação do Servidor

Como sistema de laboratorio foi instalado o CasaOS.

~~~~shell
# curl -fsSL https://get.casaos.io | sudo bash
~~~~

### Aplicações
