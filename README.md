# HashingWord
Desenvolvido em: Python3.6
Dependências: Hashlib

<pre>
 _   _           _     _           __        __            _
| | | | __ _ ___| |__ (_)_ __   __ \ \      / /__  _ __ __| |
| |_| |/ _` / __| '_ \| | '_ \ / _` \ \ /\ / / _ \| '__/ _` |
|  _  | (_| \__ \ | | | | | | | (_| |\ V  V / (_) | | | (_| |
|_| |_|\__,_|___/_| |_|_|_| |_|\__, | \_/\_/ \___/|_|  \__,_|
                               |___/
</pre>
Opções de uso:

#### hashing [typehash] [opção] [path/string]
#### Tipos de algoritmos de hash suportados:
##### ->md5 ->sha1 ->sha224 ->sha256 ->sha384->sha512 ->sha3_224 ->sha3_256 ->sha3_384 ->sha3_512

Parâmetros:

#### Parâmetro Único:
-s || --single: tira a hash da string informada
hashing md5 -s "Ciranda cirandinha"
hashing sha3_384 --single "vamos todos cirandar"

#### Parâmetro Múltiplos:
-m || --mults: processo recursivo de hashs através do input
-> será criado um arquivo em /tmp com o nome: hashing_log
Informe um espaço vazio para encerrar o loop
hashing sha256 --mults
0 -fce35d7cd57f33eba84165844183a55d31419de0bec602694476fcec98e0c09f
	>_ senha123
1 - 55a5e9e78207b4df8699d60886fa070079463547b095d1a05bc719bb4e6cd251

#### Parâmetro Wordlist:
 -w || --wordlist: informa a hash de todas as linhas de uma wordlist
hashing sha512 --wordlist senhas.txt
-> será criado um arquivo em /tmp com o nome: hashing_log
Será exibido todo o conteúdo de hashs do arquivo senhas.txt, porém
este será armazenado em /tmp/hashing_log



