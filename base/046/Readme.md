# L2 - Soma dos nós e Menor valor
<!--TOC_BEGIN-->
- [Descrição](https://raw.githubusercontent.com/qxcodeed/moodle/master/base/046/#descrição)
- [Testes](https://raw.githubusercontent.com/qxcodeed/moodle/master/base/046/#testes)
- [Código base](https://raw.githubusercontent.com/qxcodeed/moodle/master/base/046/#código-base)
<!--TOC_END-->

![](https://raw.githubusercontent.com/qxcodeed/moodle/master/base/046/__capa.jpg)

## Descrição
Leia a árvore a partir do serial utilizando o método da atividade `@044` e implemente os seguintes métodos para calcular a soma de todos os elementos e o valor do menor elemento.

```cpp
int sum(Node * root);

int min(Node * root);
```

- Entrada
    - Serial de uma árvore
- Saída
    - Soma dos valores da árvore, menor valor da árvore.

## Testes

```
>>>>>>>> 01 um
4 # # 
========
4 4
<<<<<<<<

>>>>>>>> 02 dois
1 # 0 # # 
========
1 0
<<<<<<<<

>>>>>>>> 03 tres
4 # 8 2 # # # 
========
14 2
<<<<<<<<

>>>>>>>> 04 quatro
0 9 4 # # # 5 # # 
========
18 0
<<<<<<<<

>>>>>>>> 05 cinco
0 4 # # 2 0 # # -3 # # 
========
3 -3
<<<<<<<<

>>>>>>>> 06 seis
2 0 5 # # # 3 # 7 # -9 # # 
========
8 -9
<<<<<<<<

>>>>>>>> 07 dez
1 8 7 # # 4 # 6 # # 5 0 # # 9 # 3 2 # # # 
========
45 0
<<<<<<<<
```

## Código base

Utilize a árvore dos exercícios anteriores

```cpp
int main(){
    string line;
    getline(cin, line);
    BTree bt(line);
    getline(cin, line);
    cout << bt.sum() << " " << bt.min() << "\n";
}
```