# sistemaagua_esp32
Sistema de Monitoramento de Água com ESP32



# Sistema de Monitoramento de Água com ESP32

Adaptei o sistema para utilizar a placa ESP32, aproveitando seus recursos avançados para criar um sistema de monitoramento de água mais poderoso e conectado.

## Principais Melhorias para ESP32

### 1. Conectividade WiFi

- **Monitoramento remoto**: Acesse os dados do sistema de qualquer lugar através de uma interface web
- **Configuração via navegador**: Ajuste capacidades das caixas d'água e alertas remotamente
- **API JSON**: Integração com outros sistemas e aplicativos


### 2. Interface Web Responsiva

- **Dashboard em tempo real**: Visualize níveis de água, consumo e alertas
- **Gráficos interativos**: Acompanhe tendências de consumo
- **Configuração amigável**: Interface intuitiva para ajustar parâmetros do sistema


### 3. Suporte para Múltiplas Caixas

- **Monitoramento simultâneo**: Acompanhe até 3 caixas d'água diferentes
- **Detecção de transferência**: O sistema identifica quando água está sendo transferida entre caixas
- **Configuração independente**: Cada caixa pode ter capacidade e alertas personalizados


### 4. Armazenamento Persistente

- **Preferences API**: Utiliza o sistema de armazenamento persistente do ESP32
- **Maior confiabilidade**: Dados salvos mesmo após quedas de energia
- **Mais espaço**: Armazena configurações detalhadas para múltiplas caixas


### 5. Recursos Avançados do ESP32

- **Processador mais potente**: Resposta mais rápida e cálculos mais precisos
- **Mais pinos GPIO**: Suporte para sensores adicionais
- **Interrupções de hardware**: Medição de fluxo mais precisa com a função IRAM_ATTR


## Como Configurar

1. **Conexão WiFi**:

1. Edite as variáveis `ssid` e `password` com os dados da sua rede WiFi
2. O sistema exibirá o endereço IP no LCD após a conexão
3. Acesse o sistema pelo navegador usando o IP mostrado



2. **Configuração de Hardware**:

1. Conecte o sensor de fluxo ao pino GPIO 4
2. Conecte o sensor ultrassônico principal aos pinos GPIO 5 (TRIG) e 18 (ECHO)
3. Para caixas adicionais, use os pinos definidos nos arrays TRIG_PINS e ECHO_PINS
4. Botões de navegação nos pinos 19, 21, 22 e 23



3. **Interface Web**:

1. Página principal: http://[IP-do-ESP32]/
2. Configuração de caixas: http://[IP-do-ESP32]/tank
3. API JSON: http://[IP-do-ESP32]/api





## Benefícios do ESP32

1. **Monitoramento Remoto**:

1. Acompanhe o sistema pelo celular ou computador
2. Receba alertas em tempo real
3. Configure o sistema sem precisar acessar fisicamente o dispositivo



2. **Maior Precisão**:

1. Processador mais rápido para cálculos mais precisos
2. Melhor tratamento de interrupções para medição de fluxo
3. Mais memória para armazenar históricos detalhados



3. **Expansibilidade**:

1. Adicione mais sensores facilmente
2. Integre com sistemas de automação residencial
3. Possibilidade de enviar dados para serviços na nuvem





Esta implementação para ESP32 transforma o sistema em uma solução IoT completa, permitindo monitoramento remoto e oferecendo muito mais recursos que a versão original para Arduino.
