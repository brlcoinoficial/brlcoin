Brlcoin integração
================================

http://www.brlcoin.cash

O que é Brlcoin?
----------------

O protocolo do BRLCOIN oferece a liberdade para negociar qualquer ativo de ponta a ponta em tempo real, sem intermediários ou taxas abusivas.

Acreditamos que esta tecnologia, por ser publicamente auditável, possa ajudar a população a cobrar mais dos servidores públicos, colocando assim novamente o poder em mãos de quem deve estar.

Informações
----------------
 
Simbolo: BRLC<br>
Endereços: R<br>
Emissão: 44210526 Coins<br>
Moedas Por Blocos: 25 BRLC<br>
Transações: 3 Confirmações<br>
Algoritmo: Scrypt<br>
Tipo: POW<br>
Maturidade De Bloco: 10 Blocos<br>
Porta RPC:38408<br>
Porta P2P:38407<br>

Instalação
----------------

execute este comando como root

fallocate -l 3G /swapfile<br>
chmod 600 /swapfile<br>
mkswap /swapfile<br>
swapon /swapfile<br>
echo -e “/swapfile none swap sw 0 0 \n” >> /etc/fstab<br><br>

Instale as dependencias

sudo apt-get install git -y && sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils -y && sudo apt-get install libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev -y && sudo apt-get install libboost-all-dev -y && sudo apt-get install software-properties-common -y && sudo add-apt-repository ppa:bitcoin/bitcoin && sudo apt-get update && sudo apt-get install libdb4.8-dev libdb4.8++-dev -y && sudo apt-get install libminiupnpc-dev -y && sudo apt-get install libzmq3-dev -y && sudo apt-get install libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler -y && sudo apt-get install libqt4-dev libprotobuf-dev protobuf-compiler -y

clone nosso repositório

git clone https://github.com/brlcoinoficial/brlcoin.git<br>
cd brlcoin<br>
cd src<br>
mkdir obj<br>
make -f makefile.unix<br>

com isso gera gerado o daemon da moeda
podendo testar com o seguinte comando:

./brlcoind getinfo

