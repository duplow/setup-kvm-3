# setup-kvm-3

**Chaveador KVM** (**K**eyboard **V**ideo **M**ouse) para até 4 PCs/aparelhos diferentes conectados simultaneamente, podendo alternar entre sí.

![KVM Switch Example!](/images/kvm-switch-example.jpg)
*Imagem ilustrativa*

Cada aparelho conectado contará com 3 entradas **HDMI**, 3 entradas **DisplayPort** e 1 entrada **USB 3.0**.

O projeto é montado em cima de um Arduino para fazer o chaveamento entre os aparelhos via teclado, caso opte por um chaveamento apenas via botão fisico o Arduino não será necessário.

O chavemento será feito pelo botão físico no aparelho ou via um teclado USB usando os atalhos:

  * `CTRL+SHIFT+NUM+1` para o aparelho número 1
  * `CTRL+SHIFT+NUM+2` para o aparelho número 2 e assim por diante

-------

## Instruções

Em desenvolvimento

### Materiais

Componentes necessários para um KVM de até 3 aparelhos:

* **Arduino** qualquer modelo (opcional)
* 70x Buffers **SN74HC541N** (6 por HDMI, 6 por DisplayPort e 2 por USB)
* 4x Conectores **USB 3.0 DIP** Fêmea
* 9x Conectores **HDMI DIP** Fêmea
* 9x Conectores **DisplayPort DIP** Fêmea

> É possível substituir os buffers `SN74HC541N` por multiplexadores `74HC4052`, porém será necessário muitos deles para fazer o mesmo trabalho, para cada `SN74HC541N` será necessário mais ou menos 4 multiplexadores `74HC4052`.


### Esquemas

Placa USB
![Placa USB!](/images/PCB-1.PNG)

### Montagem

Em desenvolvimento
