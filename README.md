# CS380-P7
1. If the first command line argument is makekeys, your program will simply generate a public/private RSA key pair, write their serialized forms to files public.bin and private.bin, then exit.
2. If the first command line argument is server, your program will operate in server mode. In this case, you must include two more command line arguments. The second argument should be the name of the file that contains the private key. The third argument should be the port number the server will listen on.
3. If the first command line argument is client, your program will operate in client mode. In this case, you must include three more command line arguments. The second argument should be the name of the file that contains the public key. The third argument should be the host to connect to (where the server is running). The final argument should be the port number the server is listening on.


Example:

Server

$ java FileTransfer server private.bin 38007

Client

$ java FileTransfer client public.bin localhost 38007
