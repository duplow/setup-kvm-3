# setup-kvm-3

**Chaveador KVM** (**K**eyboard **V**ideo **M**ouse) para até 3 PCs/aparelhos diferentes conectados simultaneamente, podendo alternar entre sí.

![KVM Switch Render!](/images/render.png)
_Imagem ilustrativa_

Cada aparelho conectado contará com 3 entradas **HDMI**, 3 entradas **DisplayPort** e 1 entrada **USB 3.0**.

O projeto é montado em cima de um Arduino para fazer o chaveamento entre os aparelhos via teclado, caso opte por um chaveamento apenas via botão fisico o Arduino não será necessário.

O chavemento será feito pelo botão físico no aparelho ou via um teclado USB usando os atalhos:

- `CTRL+SHIFT+NUM+1` para o aparelho número 1
- `CTRL+SHIFT+NUM+2` para o aparelho número 2
- `CTRL+SHIFT+NUM+3` para o aparelho número 3

e assim por diante

---

## Instruções

### Fabricação

 - espessura minima das trilhas (width): 0.2mm
 - espaçamento minimo (min clearance): 0.2mm (usado 0.25m)
 - fotolito: 10.000 DPI

### Módulos

- [Módulo Alimentação](/docs/power-module.md)
- [Módulo Displayport](/docs/displayport-module.md)
- [Módulo USB 3.0 tipo A](/docs/usb-30-module.md)
- [Módulo Controle](/docs/controller-module.md)

### Materiais

Componentes necessários para um KVM de até 3 aparelhos:

- **Arduino** qualquer modelo (opcional)
- 70x Buffers **SN74HC541N** (6 por HDMI, 6 por DisplayPort e 2 por USB)
- 4x Conectores **USB 3.0 DIP** fêmea
- 9x Conectores **HDMI** fêmea [link de venda](https://pt.aliexpress.com/item/1005004321901753.html?spm=a2g0o.productlist.main.3.2f4c4bd4zNbfgg&algo_pvid=e8ba0e93-4177-44cf-a99c-585d2ebb48c4&aem_p4p_detail=202302081917461309186084719520000121513&algo_exp_id=e8ba0e93-4177-44cf-a99c-585d2ebb48c4-1&pdp_ext_f=%7B%22sku_id%22%3A%2212000028751193682%22%7D&pdp_npi=3%40dis%21BRL%2118.99%2116.71%21%21%21%21%21%40211bf48d16759126661676453d06b6%2112000028751193682%21sea%21BR%214164761864&curPageLogUid=yP8cfGhjvAHO&ad_pvid=202302081917461309186084719520000121513_2&ad_pvid=202302081917461309186084719520000121513_2)
- 9x Conectores **DisplayPort DIP** fêmea
- 4x Conectores **P2** de áudio e microfone [link de venda](https://pt.aliexpress.com/item/1005004688929020.html?spm=a2g0o.ppclist.product.16.73faLsI4LsI4iQ&pdp_npi=2%40dis%21BRL%21R%24%205%2C92%21R%24%205%2C92%21%21%21%21%21%402101f6b316766497700243772e69af%2112000030107125153%21btf&_t=pvid%3Ad92d09f6-7fa5-46f7-80e0-bc18aa72a762&afTraceInfo=1005004688929020__pc__pcBridgePPC__xxxxxx__1676649770&gatewayAdapt=glo2bra)

> É possível substituir os buffers `SN74HC541N` por multiplexadores `74HC4052`, porém será necessário muitos deles para fazer o mesmo trabalho, para cada `SN74HC541N` será necessário mais ou menos 4 multiplexadores `74HC4052`.

TODO: Colocar o link para o BOM

### Esquemas

Placa USB
![Placa USB!](/images/PCB-1.PNG)

### Montagem

Em desenvolvimento
