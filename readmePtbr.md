



<span id="magicparlabel-7"></span>Descrição
---------------------------------------------

<span id="magicparlabel-667"></span> Este é um testador de capacidade da bateria bem simples, barato e autonomo. Ele se conecta à bateria e a um resistor de carga é energizado apartir de um conector microUSB (sem comunicações com o computador, apenas alimentação). Ele consome energia da bateria até que seja alcançada uma tensão de fim de descarga predeterminada, por fim é exibida a capacidade da bateria em Ampere-hours (Ah). A descrição do fabricante é difícil de entender, então eu o editei em português (inglês) mais convencional. Todos os erros, portanto, são meus - não tenho certeza sobre os detalhes na seção de calibração, por exemplo.

- Resistor de carga externa (7,5 Ω)
- Tensão de alimentação: DC4.5-6V (interface micro USB)
- Corrente de trabalho: menos de 70mA
- Tensão da bateria medida: 1.00V-15.00V, resolução 0.01V
- Tensão de terminação selecionada automaticamente, dependendo da tensão da célula carregada inicial (faixa: 0.5-11.0V)
- Corrente máxima 3A, resolução 0,001A
- A tensão máxima de erro de medição: 1% + - 0,03V
- O erro máximo de medição da corrente: 2% + - 0,010A
- A faixa máxima de capacidade da bateria: 0,001Ah..9999Ah (valores inferiores a 10Ah são exibidos como X.XXX; os valores entre 10Ah e 99.99Ah são exibidos como XX.XX e assim por diante).
- Tamanho da placa: 50 mm de comprimento por 36 mm de largura, por 17 mm de altura, incluindo espaçadores

<span id="magicparlabel-18"></span>Nota: para melhorar a precisão da medição de tensão, o circuito aplica uma polarização DC. O display pode mostrar um pequeno valor residual, que não afeta a medição real.

<span id="magicparlabel-19"></span>Instruções de uso
-----------------------------------------------------

1.  A bateria a ser medida deve estar totalmente carregada.
2.  Conecte a bateria testada observando a polaridade (terminal + no PCB para o terminal positivo da bateria). ***Inverter a polaridade pode danificar o circuito!*** Conecte a alimentação ao testador através do cabo micro USB. O display deve indicar a tensão da bateria.
 
3.  Inicie o teste pressionando o botão "OK". O testador irá automaticamente ajustar a voltagem de terminação adequada, de acordo com a voltagem de carga total da bateria, e piscar 3 vezes ao iniciar o teste.
    -   ***A tensão final de descarga pode ser alterada em incrementos de 0,1 V após o início do teste, pressionando as teclas "+" ou "-". A tensão final de descarga é exibida com um caractere P inicial.***

4.  Durante o teste, o comutador eletrônico conecta o resistor de carga e os dados de teste são exibidos em seqüência, conforme mostrado pelo indicador LED:
    -   A capacidade acumulada (Ah),
    -   Corrente de descarga instantânea (A)
    -   Tensão atual da bateria (V) 

5.  Quando a tensão da bateria atinge a tensão final de descarga, o testador corta a chave de controle de carga e exibe a capacidade (Ah) e pisca rapidamente o indicador LED correspondente. Pressione "OK" para terminar de piscar. Pressionar o botão "OK" novamente retorna ao estado ligado, para que outra bateria possa ser conectada e testada.

### <span id="magicparlabel-29"></span>Os códigos de erro

**Err1:***  
a tensão da bateria superior a 15V

***Err2:***  
a tensão da bateria é menor que a tensão final de descarga ajustada

***Err3:***  
a bateria não consegue suportar a corrente de descarga de carga (a resistência da bateria interna ou a resistência do conector / cabo é muito alta)

***Err4:***  
a corrente é muito alta (a corrente é maior que 3,1A)

### <span id="magicparlabel-34"></span>Calibração

<span id="magicparlabel-35"></span> Aplique energia USB e pressione simultaneamente todos os três botões para entrar no modo de calibração e executar os seguintes passos


1.  O primeiro passo de calibração após entrar na calibração exibe o ***0u0A***; curto circuitar os terminais de entrada para bateria positivo e negativo e pressione o botão ***"OK"***
2.  Em seguida, o display mostrará ***J10u***; aplique 10.00V DC entre o terminal positivo e negativo na entrada para bateria e pressione o botão ***"OK"*** novamente.
3.  O display mostrará ***J2.0A***; aplique 2,0 A corrente CC entre os terminais de entrada para bateria e pressione o botão ***"OK"*** para completar a calibração.


<span id="magicparlabel-133"></span>Se o testador determinar que os dados de calibração são confiáveis, ele mostrará 4 números de calibração após a conclusão do procedimento; caso contrário, ele ignorará a tentativa de calibração, descartará os dados e sairá do procedimento.

### <span id="magicparlabel-36"></span>Conteúdo:

- 2 x Resistência de 5W 7.5ohm
- 1x placa do verificador da capacidade da bateria (o cabo do USB não é fornecido)

