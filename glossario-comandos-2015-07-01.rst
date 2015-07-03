======================
Glossário de comandos
======================

:Disciplina: Fundamentos de Sistemas Operacionais
:Professor: Jurandy Soares
:Nome: Paulo de Lima Xavier
:Matrícula: 20121144010419
:Data: 01/07/2015

cat
  Com este comando é possível mostrar na tela o conteúdo do arquivo, digite: cat .bash_history + ENTER. Nesse caso, será devolvido o histórico de comandos;
  
  Com este mesmo comando também é possível escrever em um arquivo, digite: cat > arquivo + ENTER. Logo após, o prompt ficará oculto, e haverá um espaço para ser digitado o coteúdo desejado do arquivo. Para sair do modo edição digite: Ctrl + D;
  
  O camando 'cat' possui a funcionalidade de importar dados de um arquivo para outro, digite: cat arquivo1 > arquivo2 + ENTER. Assim, o conteúdo do arquivo1 irá sobreescrever o conteúdo do arquivo2.



cd
  Tem a funcionalidade de mudar o diretório para o area inicial, digite: cd + ENTER;
  
  Com o 'cd' também é possível acessar pastar, bas digitar: cd /pasta1 + ENTER ou cd /pasta1/pasta2/pasta3... + ENTER;
  
  Caso o seu diretório atual seja a 'pasta2', por exemplo '$:~/pasta1/past2', e seja necessário voltar para a pasta anterior ('pasta1'), basta digitar: cd - + ENTER.   



cowsay
  É um programa que permite enviar mensagens de uma forma mais lúdica, digite: cowsay "Uma mensagem qualquer" + ENTER. Já para direcionar uma mensagem para outro usuário, digite: cowsay -f kiss "uma mensagem Qualquer" | write nomedocolega + ENTER. Note que é utilizado o comando cowsay conjunto ao write (veja a funcionalidade mais abaixo), e que o trecho "-f kiss" permite alterar a imagem em ASCII, normalmente uma vaca, para a imagem de um beijo.



echo
  É um comando usado normalmente em scripts que permite exibir mensagens na tela ou arquivo, utlizando alguns argumentos, digite: echo $USER + ENTER. O comando anterior exibe na tela o nome do usário;
  
  Com ele também é possível listar todos os arquivos de um diretório, digite: echo * + ENTER;
  
  Podemos saber a quantidade de arquivos de um determinado diretório, basta digitar: echo * | wc -w + ENTER.



env
  Mostra na tela as variáveis de ambiente dispostas, digite: env + ENTER;
  
  Para saber a quantidade de variáveis de ambiente, digite: env | wc -l + ENTER.



exit
  Comando reponsável por terminar a sessão, digite: exit + ENTER.



help
  Exibe na tela os comando internos disponíveis, digite: help + ENTER;
  
  Caso queira saber informações sobre um comando específico, digite: help + comando + ENTER.



HISTTIMEFORMAT="%d/%m/%y"
  Este comando realiza a formatação do histórico de comandos ('history + ENTER'), assim, permite que seja adicionado informações a lista do histórico de comandos, nesse caso a data de execução dos camandos. Onde: '%d' representa o dia; '%m' representa o mês; e, '%y' representa o ano, para isso, basta digitar: HISTTIMEFORMAT="%d/%m/%y " + ENTER.
  
  Caso queira adicionar o horário de execução do comando, onde '%T' representa o horário, basta digitar: HISTTIMEFORMAT="%d/%m/%y %T " + ENTER.
  
  Para deixar essas configurações salvas permanentemente, basta digitar: export HISTTIMEFORMAT="%d/%m/%y %T " + ENTER. E, posteriormente, digite: source ~/.bashrc + ENTER. Assim, mesmo que a sessão seja fechada e torne a iniciar, digitando o comando 'history + ENTER', será apresentado o histórico de comandos com data e horário de execução.
  
  Observação: é possível perceber que há espaços entre '%d/%m/%y e %T', e um espaço logo após ao '%T', isso ocorre devido a concatenação, ou seja, se não houvesse espaços entre as informações de data, hora e a informação posterior a hora, esses atributos estariam "colados", dessa forma, para questões de organização utiliza-se os espaços.
  



hostname
  Mostra na tela o nome da máquina, digite: hostname + ENTER.



ifconfig
  Exibe as configurações de rede e de um adaptador Ethernet, detalhando as interfaces ativas no momento. Digite: ifconfig + ENTER;
 
  É possível desativar é ativar uma interface, digitando, respectivamente: ifconfig eth0 down + ENTER e ifconfig up + ENTER.



last
  Exibe informações referentes aos últimos logins efetuados, digite: last + ENTER.



lastb
  Exibe uma lista de recentes tentativas de logins errados, digite: lastb + ENTER.



ls
  Comando responsável por listar os arquivos/diretórios do ficheiro atual, digite: ls + ENTER.
  Para visualizar arquivos ocultus em um diretório, digite: ls -a + ENTER;
 
  Para visualizar arquivo ou diretório, tamanho, data e horário de modificação, nome do arquivo, entre outras informações, digite: ls -l + ENTER;
 
  Para listar os arquivos/diretórios ordenamente em uma única coluna, digite: ls -F1 + ENTER.



mkdir
  Possui a funcionalidade de criar arquivos, digite: mkdir + ENTER.



nome="fulano"
  Permite a atribuição do valor 'fulano' a variável nome, dessa forma, a variável pode ser utilizada para realizar alguma rotina interna, digite nome="fulano" + ENTER.



passswd
  Permite que seja alterado a senha de logon, a senha deve conter de 6 a 8 caracteres, possuir letras minúsculas, digitos de 0 a 9, e sinais de pontuação, digite: passwd + ENTER.



pwd
  Devolve na tela o diretório atual, digite: pwd + ENTER.



set
  Permite alterar variáveis e funções, digite: set PATH="/bin:/usr/bin:/usr/sbin:usr/local/bin" + ENTER. Nesse caso, o comando define a variável de ambiente PATH, de modo que o shell irá procurar por arquivos no /bin, /usr/bin, /usr/sbin e no /usr/local/bin, nessa ordem.



tree
  Exibir os ficheiros e seus respectivos arquivos e pastas na forma de árvore, digite: tree + ENTER;
 
  Para listar em forma de árvore os arquivos e suas respectivas permissões, digite: tree -p.



tty
  Exibi o terminal de controle da máquina, digite: tty + ENTER.



vim
 É um programa para editar texto, para entrar no editor, digite: vim + ENTER;
 
 Caso queira editar um arquivo do seu ficheiro, digite: vim arquivo + ENTER;
 
 Para começar a editar o arquivo, digite: a;
 
 Para salvar as alterações, digite: ESC + :x + ENTER;
 
 Para desfazer as alterações, digite: ESC + :u + ENTER;
 
 Para sair do vim, digite: ESC + :q! + ENTER.



wait
  


wall
  Permite o envio de mensagens para vários usários de uma única vez, digite: sudo wall message.txt + ENTER. Nesse caso, estamos enviando o conteúdo de um arquivo.



which
  Permite encontrar o diretório de arquivos executáveis do sistema. Digite: sudo which -a echo + ENTER. Dessa forma, serão exibiddos todos os diretórios correspondentes ao argumento 'echo' com o auxílio do '-a'.



while
  Um laço de condição que serve para criar scripts.
 
  Digite por exemplo:
  	while true; + ENTER
		do + ENTER
			echo "Uma Mensagem qualquer" | write nomedousuario + ENTER
	done + ENTER
 
  Dessa forma a mensagem será enviada para o nome do usuário, enquanto for verdadeiro (true).



who
  Mostra na tela o nome de todos os usuários logados na rede. Digite por exemplo: who + ENTER.



whoami
  Mostra na tela o nome do usário logado. Digite por exemplo: whoami + ENTER.



write
  Permite enviar mensagens para outros usuários. Digite por exemplo: "Mensagem" | write nomedousuario + ENTER. 
  
 
 
Ctrl + L
  Comando responsável por limpar a tela, posicionando o prompt no canto superior esquerdo, para isso, digite: ctrl + l.
  
  
git
  Comando reponsável por informar todos os comandos referentes ao GitHub no terminal. Para visualizar os comandos disponível, digite: git + ENTER.
  
 
 
ssh
  É um programa que permite fazer login e executar comandos em uma máquina remoto. Para logar a uma máquina através de seu 'ip', por exemplo, digite: ssh seunome@ip + ENTER.
  
  
type
  Comando usado para descobrir se o comando é arquivo binário interno ou externo, digite: type comando + ENTER;
  
  
cp
  Comando responsávelo por arquivos e diretórios. Por exemplo, você possui um arquivo chamado 'imagem1.jpg' e deseja duplicalo, basta digitar: cp imagem1.jpg imagem2.jpg + ENTER. Assim, será criada uma cópia chamada 'imagem2.jpg'.
  Caso seja necessário duplicar uma arquivo para diretórios diferentes, digire: cp ~/Web/Historico/historico.txt ~/Web + ENTER. Nesse caso, o arquivo 'historico.txt', que está no diretório '/Web/Historico', será copiado para o diretório '/Web'.
  Também é possível copiar, por exemplo, vários arquivos de uma mesma extensão, digite: cp ~/pictures/picture-*.jpg ~/picture-backup + ENTER. Nesse caso, todos os arquivos 'picture-' de extensão '.jpg' serão copiados de '/pictures' para '/picture-backup'.
  
  
  
wc -l
  Com este comando é possível contar o número de linhas de um determinado arquivo, digite: wc -l arquivo + ENTER.
  
 
 
pstree
  Comando responsável por mostrar a árvore de processos de um determinado usuário, digite: pstree nomeusuario + ENTER.
  


gunzip
  Comando responsável por descompactar um arquivo, por exemplo, um diretório possui um arquivo compactado 'arquivo.txt.gz' para descompacta-lo, digite: gunzip arquivo.txt.gz + ENTER. Então, será criado um novo arquivo descompactado no diretório denominado: arquivo.txt.
  
  
rm
  Comando responsável por excluir um ou mais arquivos.
  
  Argumentos:
  
  -d, --directory
  
  Remova diretórios, mesmo que eles não estão vazias. Disponível apenas para um usuário privilegiado.

  -f, --force
  
  Remover arquivos protegidos contra gravação sem avisar.

  --help
  
  Imprimir uma mensagem de ajuda e depois sai.

  -i, --interactive
  
  Solicitar y (remover o arquivo) ou n (não remover o arquivo).

  -no-preserve-root
  
  Não trate raiz (/) especialmente. Este é o padrão.

  --preserve-root
  
  Não opere de forma recursiva na raiz (/).

  -r, -R, --recursive
  
  Se arquivo for um diretório, remover todo o diretório e todo o seu conteúdo, incluindo subdiretórios. Seja avisado: o uso desta opção pode ser perigoso.

  -v, --verbose
  
  O modo detalhado (imprimir o nome de cada arquivo antes de removê-lo).

  --version
  
  Informação sobre a versão e depois sai.

  -
  
  Marcar o fim de opções. Utilize esta opção quando você precisa fornecer um nome de arquivo que começa com -.
  


sort
  Comando reponsável por organizar linhas de comandos de arquivos.
  
  Argumentos:
  
  -d, --dictionary-order
  
  Classificar em ordem dicionário.
  
  -n
  
  Classificar em ordem aritmética.
  
  -g, --general-numeric-sort
  
  Classificar em ordem numérica geral.
  
  -u, --unique
  
  Linhas idênticas no arquivo de entrada aparecer apenas uma vez na saída.
  
  Exemplos:

  Listar os arquivos por número decrescente de linhas:
  wc -l * | sort -r

  Alfabetizar uma lista de palavras, remova duplicatas, e imprimir a freqüência de cada palavra:
  sort -fd wordlist | uniq -c

  Organizar o arquivo de senha numericamente pelo terceiro campo (ID do usuário):
  sort -nk3,4 -t: /etc/passwd
  
  
awk
  É um utilitário responsável por processar arquivos de texto. 
  
  Exemplos:
  
  Cria um arquivo com argumentos concatenados no formato 'string + comando', a partir das informações de histórico armazenadas em outro arquivo.
  
  awk '{print "Comando: " $2}' historico.txt | sort -u > historico2.txt  + ENTER.
  
  Utlizia o mesmo princípio anterior, no entanto, adicionando títulos as colunas de cada argumento.
  
  awk 'BEGIN {printf "%-10s %s\n", "Name", "Number" 
  printf "%-10s %s\n", "----", "------"} 
  {printf "%-10s %s\n", $1, $2}' historico.txt > historico2.txt + ENTER.
  
  
id
  Comando responsável por mostrar o identificador de usuário na máquina(UID) e o GID(Grupo), digite: id + ENTER.
  
  

