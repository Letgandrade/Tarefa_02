Simulação de Semáforo com Raspberry Pi Pico W

Este projeto implementa um semáforo utilizando a placa Raspberry Pi Pico W, simulando o funcionamento de um semáforo real com três LEDs (vermelho, amarelo e verde). A mudança de estado ocorre a cada 3 segundos, utilizando a função add_repeating_timer_ms() da biblioteca Pico SDK.

📌 Objetivos

Simular um semáforo com LEDs e resistores.

Alternar os LEDs seguindo a sequência: Vermelho → Amarelo → Verde.

Utilizar um temporizador periódico para alternar os estados a cada 3 segundos.

Exibir mensagens na porta serial a cada 1 segundo.

Testar o código com o LED RGB nos GPIOs 11, 12 e 13 utilizando o BitDogLab.

🔧 Componentes Utilizados

🖥️ Microcontrolador: Raspberry Pi Pico W

💡 LEDs: 3 LEDs (Vermelho, Amarelo e Verde)

🔌 Resistores: 3 resistores de 330Ω

📜 Fluxo de Funcionamento

O código inicia com o LED vermelho ligado.

A cada 3 segundos, o estado do semáforo muda na seguinte ordem:

🔴 Vermelho → 🟡 Amarelo → 🟢 Verde

A função repeating_timer_callback() controla a mudança dos LEDs.

A cada 1 segundo, uma mensagem é exibida via porta serial.

O experimento também pode ser testado com um LED RGB nos GPIOs 11, 12 e 13.

🚀 Execução no Wokwi

Acesse o Wokwi e configure a simulação conforme a Figura 2 do enunciado.

Utilize os GPIOs 13 (vermelho), 12 (amarelo) e 11 (verde).

Compile e execute o código.

Verifique as mensagens enviadas via porta serial.

🛠 Autor

Projeto desenvolvido por Letícia Andrade no contexto da disciplina de Sistemas Embarcados. 🚀