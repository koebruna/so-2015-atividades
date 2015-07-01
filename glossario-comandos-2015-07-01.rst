======================
Glossário de comandos
======================

:Disciplina: Fundamentos de Sistemas Operacionais
:Professor: Jurandy Soares
:Nome: Paulo de Lima Xavier
:Matrícula: 20121144010419
:Data: 01/07/2015

cat
  Mostra na tela o conteúdo do arquivo. Digite: cat .bash_history + ENTER. Nesse caso, será devolvido o histórico de comandos.


cd
  Muda o diretório para o area inicial. Digite: cd + ENTER. 


cowsay
  É um programa que permite enviar mensagens de uma forma mais lúdica. Digite: cowsay "Uma mensagem qualquer" + ENTER. Para direcionar uma mensagem para outro usuário, digite: cowsay -f kiss "uma mensagem Qualuer" | write nomedocolega + ENTER. Note que é utilizado o comando cowsay conjunto ao write (veja a funcionalidade mais abaixo), e que o trecho "-f kiss" permite alterar a imagem em ASCII, normalmente uma vaca, para a imagem de um beijo.


echo
  É um comando usado normalmente em scripts que permite exibir mensagens na tela ou arquivo, utlizando alguns argumentos. Digite: echo $USER + ENTER. O comando anterior exibe na tela o nome do usário.


env
  Mostra na tela as variáveis de ambiente dispostas. Digite: env + ENTER. 


exit
  Comando reponsável por terminar a sessão. Digite: exit + ENTER.


help
  Exibe na tela os comando internos disponíveis. Digite: help. Caso queira saber informações sobre qualquer comando e as suas funcionalidades, digite: help + comando + ENTER.


HISTTIMEFORMAT="%d/%m/%y"
  Permite que seja adicionado informações a lista do histórico de comandos, como a data de execução dos camandos. Digite: HISTTIMEFORMAT="%d/%m/%y" + ENTER.


hostname
  Mostra na tela o nome da máquina. Digite: hostname + ENTER.


ifconfig
  Exibe o ip da máquina, entre outras informações relacionada. Digite: ifconfig + ENTER.


last
  Exibe informações referentes aos últimos logins efetuados. Digite: last + ENTER.


lastb
  Descrição do comando


ls
  Comando responsável por listar os arquivos do ficheiro atual. Digite: ls + ENTER.


mkdir
  Possui a funcionalidade de criar arquivos. Digite: mkdir + ENTER.


nome="fulano"
  Permite a atribuição do valor 'fulano' a variável nome, dessa forma, a variável pode ser utilizada para realizar alguma rotina interna. Digite nome="fulano" + ENTER.


passswd
  Permite que seja alterado a senha de logon. Digite: passwd + ENTER.


pwd
  Mostra na tela o diretório atual. Digite: pwd + ENTER.


set
  Permite alterar variáveis e funções. Digite: set PATH="/bin:/usr/bin:/usr/sbin:usr/local/bin" + ENTER. Nesse caso, o comando define a variável de ambiente PATH , de modo que o shell irá procurar por arquivos no /bin, /usr/bin, /usr/sbin e no /usr/local/bin, nessa ordem.


tree
  Exibir os diretórios e seus respectivos arquivos e pastas. Digite: tree + ENTER.


tty
  Exibi o terminal de controle da máquina. Digite: tty + ENTER.


vim
  Devolve um editor de text. Digite por exemplo: vim + ENTER.


wait
  


wall
  Permite o envio de mensagens para vários usários de uma única vez. Digite: sudo wall message.txt + ENTER.


which
  Permite encontrar o diretório de arquivos executáveis do sistema. Digite: sudo which -a echo + ENTER. Dessa forma, serão exibiddos todos os diretórios correspondentes ao argumento 'echo' com o auxílio do '-a'.


while
  Um laço de condição que serve para criar scripts. Digite por exemplo:
  
  while true;
	do
		echo "Enchendo o saco" | write nomedoamiguinho
	done
	+ ENTER
  Dessa forma a mensagem "Enchendo o saco" será enviada para o nome do colega, enquanto for verdadeiro (true).

who
  Mostra na tela o nome de todos os usuários logados na rede. Digite por exemplo: who + ENTER.


whoami
  Mostra na tela o nome do usário logado. Digite por exemplo: whoami + ENTER.

write
  Permite enviar mensagens para outros usuários. Digite por exemplo: "Mensagem" | write nomedousuario + ENTER. 

