# PHP sem nada Xampp e com muito Xdebug no Windows

Uma coisa que já é sabida há um bom tempo é que NÃO precisamos usar o Xampp para montarmos um bom ambiente de desenvolvimento, mas voce pode argumentar que o próprio site oficial do PHP na [Instalação no Windows](https://www.php.net/manual/pt_BR/install.windows.php) recomenda fazer uso dele por ser mais pratico, concordo totalmente com essa afirmativa, mas o problema é que além de PHP são instalados outra ruma de tranqueiras que são desnecessárias. Caso queira entender o motivo dessas ferramentas serem desnecessárias minha sugestão é assistir o video do Vinícius Dias de nome: [XAMPP: Por Que Este Não Deve Ser seu Ambiente de Desenvolvimento](https://www.youtube.com/watch?v=XgJbv1itIOE). Chega de conversa fiada e vamos para a configuração.


# Índice

  - [Instalando O PHP no Windows](#instalando-o-php-no-windows)
  - [Instalando o Xdebug](#instalando-o-xdebug)
  - [VScode e suas extensões](#vscode-e-suas-extensões)
  - [Usando o SQLite](#usando-o-sqlite)


Para instalar o PHP no windows basta somente 3 passos, primeiro que vamos baixar os arquivos zipados no linK: [PHP para windows](https://windows.php.net/download/), importante mencionar que talvez seja necessário instalar o **Visual C++ Redistributable for Visual Studio**, verifique antes no seu windows ele está instalado, caso contrário basta baixar neste link: [Visual C++ Redistributable](https://aka.ms/vs/16/release/VC_redist.x64.exe), instalação padrão do windows, faz *next* até aparecer o *finish*. 

O próprio site explica as diferenças entre as versões disponíveis, para este exemplo vou usar o **PHP 8.2 (8.2.19)** com a versão **VS16 x64 Thread Safe (2024-May-08 07:21:58)**, para a gente vamos somente baixar o arquivo .ZIP como mostrado na figura.

![image](versaoPHP-1.png)


Feito isso, vamos agora descompactar a o zip, mas antes crie um diretório na raiz do disco C do windows, vai ficar assim **"C:\php"**. depois da árdua tarefa descompactar um arquivo, agora entre na pasta e encontrará de cara os arquivos ***php.ini-development***  e ***php.ini-production*** , faça uma copia do arquivo ***php.ini-development*** e renomeia para ficar somente **php.ini** o resultado final vai ser como o da imagem.

![image](PHP%20Local-2.png)

Estamos quase lá, falta agora nossas variáveis de ambiente, pesquise no menu iniciar do windows por *Editar as variáveis de ambiente*.

![image](variaveis%20de%20ambiente-3.png)

Agora clicando em *variáveis de ambiente*, vamos ter a seguinte tela.

![image](PATH-4.png)

Edite a variável **Path** e nela coloque o caminho da pasta do php: **"C:\php"**, seu PHP está instalado no windows, para verificar de fato se deu bom na instalação abra seu terminal e digite: ***php -v*** e o resultado é para ser.

![image](PHP%20terminal-5.png)

Com isso você já pode fazer fazer seus programas com o PHP, mas aqui a gente quer colocar um ambiente de desenvolvimento arretado, então vamos configurar o gerenciador de pendencias do PHP o [commposer](https://getcomposer.org) e nossa ferramenta de debug o [Xdebug](https://xdebug.org).





