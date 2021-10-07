# \x08

72 - Configure seu handler python (transformado em PE.exe no windows) para quando receber uma requisição via socket contendo a palavra "drop" na porta udp 1337 desligue a máquina windows.

73 - Configure seu código python no kali para fazer a requisição UDP enviando o comando de drop para a máquina windows.

74 - Crie uma função em python que captura um screenshoot da tela (para windows).

75 - Faça com que seu handler ao receber o comando "print" via socket UDP na porta 1337 tire um print da tela, salvando-o em um diretório temporário.

76 - Faça com que o seu handler envie um email para você com o texto "Beco do Exploit" utilizando smtp ao receber o comando "send" via socket UDP na porta 1337.

77 - Faça com que o handler no windows envie para você por email o screenshot que ele capturou ao receber o comando "print" via socket UDP na porta 1337.

78 - Faça com que o seu handler capture as credenciais salvas no chrome ao receber o comando "chrome" via socket UDP na porta 1337 e as envie por email para você.

79 - Crie um servidor linux em outra VM com 256 mb de ram e 2gb de disco utilizando debian netinst + apache e crie um snapshot.

80 - Crie uma função no seu handler windows que requisita 1337 vezes a url http:///index.html e deixe executando até que trave, desligue ou crashe a vm.

81 - Restore o snapshot da vm, então crie uma função no seu handler do windows para que ao receber uma requisição contendo a string "ddos" via socket UDP na porta 1337, inicie as requisições para o host como descrito na atividade 80.
