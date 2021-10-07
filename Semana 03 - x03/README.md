# \x03

16 - Inicie o servidor SSH no kali, então na VM linux, crie um script python utilizando paramiko para que seja estabelecida uma conexão via SSH entre as duas máquinas (crie o server ssh com paramiko). Faça um client no Windows para se conectar no Kali, após a conexão com sucesso, finalize. Então faça um server SSH no Windows com paramiko e se conecte com o ssh nativo do Kali no Windows.

17 - leia RFC 1918 e também sobre protocólos e serviços de rede.

18 - Crie um script em python no seu kali que realiza um banner grabbing nas portas 80 , 22 e 3306 na VM linux (não utilize bibliotecas prontas, realize a conexão via socket, receba o banner e printe o resultado).

19 - Crie um script em python que realiza um discover de portas no IP da VM linux, seu script precisa percorrer 65535 portas e retornar a saída " [porta] OPEN " e não deve printar as portas que não respondem.

20 - Crie um script em python que verifica se o IP está respondendo utilizando ICMP. Utilize a biblioteca icmplib e crie uma função que executa o ping para o host retornando true se o mesmo estiver vivo.

21 - Leia sobre mascara de subrede.

22 - Crie uma script em python que retorna a quantidade de IPs que cabe dentro de cada barramento, exemplo: /9 = 8388606 Hosts /30 = 2 Hosts e etc... (dica utilize variáveis fixas, não precisa consumir procesamento para isso).

23 - Pesquise a diferença entre classe, função e método em programação.

24 - Crie uma lista chamada hosts.txt contendo 10 endereços IP (um em cada linha, da mesma maneira que você faria uma wordlist), dentre eles insira IPs válidos da sua estrutura, então crie um script python que le o arquivo hosts.txt e informa quais dos IPs do arquivo estão vivos na rede.

24 - Crie um Script em python que identifica qual é o endereço IP da máquina em que o mesmo está sendo executado. Desenvolva este programa para ser executado no windows, o programa precisa printar na tela qual é o IP e a máscara de subrede da máquina que o executou.

25 - Crie um programa em python com as seguintes específicações, e após a conclusão crie um executável de windows para o mesmo.

- Especificações:

  O programa precisa identificar qual é o endereço de rede do host que está o executando, para isso ele precisa receber o IP e a Máscara de Subrede do host. Então o programa fará um scan de discovery neste endereço de rede. Após encontrar os IPs vivos, o mesmo irá realizar um scan de portas, então realizará um banner grabbing nas portas abertas e mostrará os resultados na tela seguindo as seguintes especificações:

    (Exemplo) Rede: 192.168.1.0/24

      ```sh
      [ - ] 192.168.1.22
      80 --- OPEN
      80 --- OPEN
      22 --- OPEN
      3306 --- OPEN
      [ - ] 192.168.1.28
      80 --- OPEN
      22 --- OPEN
      ```

Não mostre na tela os IPs que não retornaram portas abertas. Uma dica, crie uma função que utiliza ICMP para validar se o host está vivo antes de escanear todas as portas. (não utilize bibliotecas prontas ou funções de sistema como system(ping ip) por exemplo.). Faça com que o "-" seja printado com a cor verde claro o "[]" seja branco e o endereço IP seja branco. "---" vermelho e O "OPEN" azul claro.
