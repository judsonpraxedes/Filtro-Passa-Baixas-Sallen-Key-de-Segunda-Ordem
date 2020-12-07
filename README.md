# Filtro-Passa-Baixas-Sallen-Key-de-Segunda-Ordem
Este repositório contém o projeto de um filtro do tipo Sallen Key de Segunda Ordem, para cobrir a Frequência de 455 kHz utilizada em rádio FM broadcast.
O filtro deve ter frequência de corte em 1 MHz, de modo a atender a faixa de frequência supracitada.

# REFERENCIAL TEÓRICO
Através de manipulações matemáticas, sabe-se que a função de transferência de um filtro do tipo Sallen Key se dá através da seguinte Equação:
H(s)=((2πf_c)²)/(s^2+(2πf_c)/Q s+(2πf_c)²)      (1)

E que o fator de qualidade 'Q' do filtro é determinado com base na Eq. 2. 
Q=1/(2πf_c C_1 (R_1+R_2))       (2)

De modo que a frequência de corte pode ser determinada pela Eq. 3.
f_c=1/(2π√(R_1 R_2 C_1 C_2 ))       (3)

Substituindo-se (2) e (3) em (1), tem-se:
H(s)=1/(1 + C_2(R_1+R_2)s+ (C_1 C_2 R_1 R_2)s²)     (4)

Onde o fator de qualidade 'Q' determina o formato da resposta do filtro, e pode ser classificado em 3 tipos:
  Bessel: Q = 0,5;
  Butterworth: Q = 0,707
  Chebyshev: Q > 0,707

[Circuito](https://github.com/judsonpraxedes/Filtro-Passa-Baixas-Sallen-Key-de-Segunda-Ordem/blob/main/Circuito_1.png)
