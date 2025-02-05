# Atividade 2: Temporizador de um Disparo (One Shot)

## Descrição
Este projeto utiliza a função `add_alarm_in_ms()` do **Pico SDK** para criar um sistema de temporização que controla o acionamento de LEDs a partir do clique em um **botão (pushbutton)**. Os LEDs acendem de forma sequencial após a pressão do botão, com temporização de **3 segundos** entre as transições.

## Componentes Utilizados
- **Microcontrolador:** Raspberry Pi Pico W
- **LEDs:** 3 LEDs (Azul, Vermelho e Verde)
- **Resistores:** 3 resistores de 330 Ω
- **Botão (Pushbutton)**

## Requisitos
1. **Acionamento sequencial dos LEDs:**
   - Ao pressionar o botão, todos os LEDs são ligados.
   - Após 3 segundos, apenas dois LEDs permanecem ligados.
   - Após mais 3 segundos, apenas um LED permanece ligado.
   - Finalmente, todos os LEDs são desligados.

2. **Controle de temporização:**
   - A função `add_alarm_in_ms()` é utilizada para definir um atraso de **3 segundos** entre cada estado dos LEDs.

3. **Callback para controle dos LEDs:**
   - O estado dos LEDs é modificado dentro das **funções de call-back** do temporizador, como `turn_off_callback()`.

4. **Prevenção de ativação prematura:**
   - O botão **não pode iniciar uma nova sequência de LEDs enquanto a anterior não tiver finalizado**.

5. **Teste na Ferramenta Educacional BitDogLab:**
   - O experimento deve ser testado utilizando:
     - **LED RGB nos GPIOs 11, 12 e 13**
     - **Botão A no GPIO 05**

6. **(Opcional) Implementação de Software Debounce:**
   - Criar uma rotina para evitar o efeito bouncing no botão.

## Configuração e Execução
1. Conectar os componentes de acordo com a simulação proposta.
2. Subir o código no Raspberry Pi Pico W.
3. Testar a resposta dos LEDs pressionando o botão.
4. Ajustar os tempos de atraso se necessário.

## Simulação no Wokwi
Para visualizar a simulação sugerida, acesse o link abaixo:
[Ver simulação](https://www.dropbox.com/scl/fi/7faa7ib6bjrxncr2dxnf7/2025-01-26-14-01-54.mkv?rlkey=wqvef7zpxpuwvz2joj6qucasd&dl=0)

---
**Autor:** Leticia Galvao Andrade 
**Data:** 2025


