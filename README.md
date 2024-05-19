# PHP sem nada Xampp e com muito Xdebug no Windows

Uma coisa que já é sabida há um bom tempo é que NÃO precisamos usar o Xampp para montarmos um bom ambiente de desenvolvimento, mas voce pode argumentar que o próprio site oficial do PHP na [Instalação no Windows](https://www.php.net/manual/pt_BR/install.windows.php) recomenda fazer uso dele por ser mais pratico, concordo totalmente com essa afirmativa, mas o problema é que além de PHP são instalados outra ruma de tranqueiras que são desnecessárias. Caso queira entender o motivo dessas ferramentas serem desnecessárias minha sugestão é assistir o video do Vinícius Dias de nome: [XAMPP: Por Que Este Não Deve Ser seu Ambiente de Desenvolvimento](https://www.youtube.com/watch?v=XgJbv1itIOE). Chega de conversa fiada e vamos para a configuração.


# Índice

  - [Instalando O PHP no Windows](#instalando-o-php-no-windows)
  - [Instalando o Xdebug](#instalando-o-xdebug)
  - [VScode e suas extensões](#vscode-e-suas-extensões)
  - [Usando o SQLite](#usando-o-sqlite)


Para instalar o PHP no windows basta somente 3 passos, primeiro que vamos baixar os arquivos zipados no linK: [PHP para windows](https://windows.php.net/download/), importante mencionar que talvez seja necessário instalar o **Visual C++ Redistributable for Visual Studio**, verifique antes no seu windows ele está instalado, caso contrário basta baixar neste link: [Visual C++ Redistributable](https://aka.ms/vs/16/release/VC_redist.x64.exe), instalação padrão do windows, faz *next* até aparecer o *finish*. 

O próprio site explica as diferenças entre as versões disponíveis, para este exemplo vou usar o **PHP 8.2 (8.2.19)** com a versão **VS16 x64 Thread Safe (2024-May-08 07:21:58)**, para a gente vamos somente baixar o arquivo .ZIP como mostrado na figura.

Figura 1


