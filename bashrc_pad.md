ip() {
        curl ifconfig.me; echo;
}

sockett() {
    export CARDANO_NODE_SOCKET_PATH=/home/marep/cardano/testnet/db/node.socket
    export TESTNET_MAGIC="--testnet-magic 1097911063"
}

socketr() {
        export CARDANO_NODE_SOCKET_PATH=/tmp/forwarded.socket
}

tipt() {
        cardano-cli query tip --testnet-magic 1 
}

<<comment
cnt() {
  submitArgs=(
   --topology /home/marex/cn/testnet/testnet-topology.json
   --database-path /home/marex/cn/testnet/db
   --socket-path /home/marex/cn/testnet/db/node.socket
   --host-addr 0.0.0.0
   --port 8080
   --config /home/marex/cn/testnet/testnet-config.json
  )
