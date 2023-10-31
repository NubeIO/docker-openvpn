# HOW TO

## How to build

- docker build . -t openvpn-server-standalone:1.0.0
- docker tag openvpn-server-standalone:1.0.0 nubeio/openvpn-server-standalone:1.0.0
- docker push nubeio/openvpn-server-standalone:1.0.0

## How to run

- docker run -e EASYRSA_BATCH=1 -it --cap-add NET_ADMIN --name openvpn-server-standalone -p "1194:1194/tcp" nubeio/openvpn-server-standalone:1.0.0
- docker rm -f openvpn-server-standalone