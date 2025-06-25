# 🚗 Sistema de Cancela Automática com Arduino

Um projeto simples que abre e fecha uma cancela automaticamente quando detecta um veículo.

## Componentes Necessários
- Arduino Uno
- Sensor ultrassônico HC-SR04
- Servo motor (para a cancela)
- 1 LED verde e 1 LED vermelho
- Resistores (220Ω para os LEDs)
- Fios e protoboard

## Como Funciona
1. O sensor mede a distância continuamente
2. Quando algo chega a menos de 15cm:
   - Acende o LED vermelho
   - Abre a cancela (servo gira para 90°)
3. Espera 3 segundos
4. Fecha a cancela e volta ao normal:
   - Apaga o LED vermelho
   - Acende o LED verde

## Conexões
| Arduino | Componente |
|---------|------------|
| Pino 9  | HC-SR04 Trig |
| Pino 10 | HC-SR04 Echo |
| Pino 6  | LED Vermelho |
| Pino 7  | LED Verde |
| Pino 3  | Servo |

## Como Usar
1. Baixe o arquivo `.ino`
2. Abra na IDE Arduino
3. Conecte os componentes como na tabela acima
4. Carregue o código para o Arduino

## Personalização
Você pode alterar no código:
- Distância de ativação (15cm)
- Tempo que a cancela fica aberta (3 segundos)
- Pinos usados

---

Feito por Matheus Ferreira.  
✉ Contato: matheushollifer@gmail.com
