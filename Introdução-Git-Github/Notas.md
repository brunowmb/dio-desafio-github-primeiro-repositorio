

Gitbash - Terminal extendido para otimizar o uso do Git;

### Comandos Windows:

dir - listar os repositórios
cd - mudar de diretório
mkdir - criar diretório
del - deletar arquivo dentro do diretório
rmdir - deletar o diretório

### Objetos fundamentais internos do Git:

#### Blobs

Onde os arquivos são guardados; Objeto que contém metadados;
Estrutura básica contém o tipo, o tamanho do arquivo, /0 e o SHA1 do arquivo;

#### Trees

Armazenam um ou mais Blobs diferentes;
Apontam para blobs ou outras árvores;
Também é um objeto que contém metadados;
Estrutura básica contém o tipo, o tamanho do , /0, o blob, o SHA1 dela e o nome do arquivo

#### Commits

Objeto mais importante de todos porque junta os outros;
Apontam para trees, para parentes (último commit feito), autor, e para a mensagem;
Também tem um timestamp (informa data, hora de quando foi criado);
Autor e mensagem é que dão o sentido do Commit;
Também possui um SHA1 (hash de 40 caracteres identificador dos metadados).
Se alterar algo de um blob, altera o SHA1 dele, que altera o SHA1 da árvore, que altera o SHA1 do Commit

Por causa dessa estrutura o Git é um sistema distribuído e seguro.

#### Chave SSH

Usada para estabelecer uma conexâo segura e encryptada entre duas máquinas;
Sempre terá uma chave pública (fica no Github para nosso caso) e uma chave privada que é a da minha máquina;

#### Comandos básicos git

git status - saber qual o estado atual e o que precisa ser feito

git init - iniciar o sistema de controle de versão

git add - mover para o stage

git commit - mover para o repositório local

git clone - clonar um repositório vindo do servidor (github ou outro)

git push - empurrar o repositório local para o servidor (github)

git pull - puxar um repositório do servidor para a máquina
