# ClassApp
script para realização do desafio

Telefone:
Checagem de numero  brasileiro, aceitando xx xxxxxxxx, (xx) xxxxxxxxx , 
ele checa se for numero de celular(9digitos) ou casa (8) após a extração do ddd , e checa se celular comeca com 6-9,
e casa comeca n<6, se não for consistente não é adicionado.

Email: checa se tem o @ e se nao tem espaco depois do arroba(dominio)

Hard Coded elements: para checagem de email e telefone são as tags 'phone', e 'email' nas colunas da tabela, sendo as palavras seguintes 
consideradas tags variaveis.
'see_all' e 'invisible' foram hard coded, para poder usar o valor falso como inicial.

foi considerada a coluna 2 da tabela(tabela[1]) como chave da tabela, mas se quiser mudar a chave , na chamada de função :
ArrumaLinhasRepetidas(obj,pos) é passado parametro pos, que é a posição da chave da tabela e deveria ser unica.

Descrição das funções: 
1)eliminav elimina virgulas em elementos da tabela, substituindo por '/'

2)ArrumaHeaderRepetido: observa o nome das colunas, e se houverem nomes iguais ele junta essas colunas em todas as linhas com '/'

3)ArrumaLinhasRepetidas: verifica a chave passada em pos, e se houver linhas com mesma chave, ele junta as linhas concatenando com '/' os elementos diferentes.

4)Arruma: a função que organiza em formato objeto desejado, ele faz a checagem dos tipos de colunas, e se as linhas são consistentes(email, phone) e organiza o objeto 

5)main: le o arquivo input.csv , realiza o tratamento do arquivo, e salva em output.json
