# Invade-if-you-can
Este estudo abrange uma análise detalhada das vulnerabilidades de sistemas por meio das plataformas TryHackMe e HackerOne. Utilizando ambientes simulados e desafios práticos, exploramos uma ampla gama de técnicas e abordagens para identificar e explorar vulnerabilidades em sistemas operacionais, aplicativos e redes. Desde análises de código e configurações até explorações de falhas e testes de penetração, este estudo oferece uma visão abrangente sobre como identificar, explorar e mitigar vulnerabilidades de segurança. Ao combinar os recursos educacionais do TryHackMe com os desafios do HackerOne, buscamos aprimorar nossas habilidades em segurança da informação e nos preparar para enfrentar ameaças cada vez mais sofisticadas no mundo digital.


## Instalação
A maioria das empresas terá uma página de portal de administração, dando à sua equipe acesso a controles administrativos básicos para as operações diárias. Para um banco, um funcionário pode precisar transferir dinheiro de e para contas de clientes. Muitas vezes, essas páginas não são privadas, permitindo que os invasores encontrem páginas ocultas que mostram ou dão acesso a controles administrativos ou dados confidenciais.

Digite o seguinte comando no terminal para encontrar páginas potencialmente ocultas no site do FakeBank usando GoBuster (um aplicativo de segurança de linha de comando).
```shell
gobuster -u http://fakebank.com -w wordlist.txt dir
```
```
ubuntu@tryhackme:~/Desktop$ gobuster -u http://fakebank.com -w wordlist.txt dir
=====================================================
Gobuster v2.0.1
=====================================================
[+] Mode         : dir
[+] Url/Domain   : http://fakebank.com/
[+] Threads      : 10
[+] Wordlist     : wordlist.txt
[+] Status codes : 200,204,301,302,307,403
[+] Timeout      : 10s
=====================================================
2022/04/11 18:23:28 Starting gobuster
=====================================================
/images (Status: 301)
/DIRECTORY_NAME_OUTPUT (Status: 200)
=====================================================
2022/04/11 18:23:38 Finished
=====================================================
```
