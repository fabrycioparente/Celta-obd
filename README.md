# Celta OBD — leitor OBD2 no navegador

Web app para ler os dados de um **Chevrolet Celta 1.0 LT 2013** (motor VHC-E 8V flex) com um adaptador **ELM327 Bluetooth LE**, sem instalar aplicativo nativo.

## Funções
- Conta-giros (faixa vermelha a partir de 6.400 rpm) e velocímetro
- Consumo instantâneo em km/l e L/h, estimado por rotação, pressão do coletor e temperatura do ar, com escolha de gasolina ou etanol e ajuste fino de calibração
- Computador de viagem: distância, média, litros gastos e tempo de motor
- Alertas de temperatura do motor e de bateria/alternador
- Leitura e limpeza de códigos de falha (DTC) com descrição em português
- Chassi (VIN), protocolo, versão do adaptador e tensão da bateria
- Terminal para enviar comandos AT/OBD direto ao ELM327
- Modo demonstração, que funciona sem o carro

## Como usar
1. Abra o site por **HTTPS** num navegador com Web Bluetooth:
   - **iPhone:** app [Bluefy](https://apps.apple.com/app/id1492822055) (o Safari não tem Web Bluetooth)
   - **Android / computador:** Chrome ou Edge
2. Feche outros apps OBD, porque o adaptador aceita uma conexão por vez.
3. Ligue a ignição, toque em **Conectar** e escolha o adaptador.

## Observações
- Só funciona com adaptadores **BLE**. ELM327 Bluetooth clássico não conecta no iPhone, e os modelos Wi-Fi não funcionam em navegadores.
- O consumo é uma estimativa. Calibre na aba **Info** comparando com o abastecimento.
- Apagar códigos de falha não conserta o defeito, só apaga a luz.

Tudo num único arquivo, `index.html`, sem dependências.
