---
title: Desligando sistemas embarcados corretamente
subtitle: Raspberry, Arduino, ESP8266, ESP32 e outros
description: Seja para não corromper dados em placas com sistema operacional
  embarcado ou para gerenciar melhor a energia para microcontroladores, vamos
  aprender como montar soluções para ligar/ desligar as plaquinhas
  adequadamente.
date: 2020-06-02T21:00:04.798Z
author: Alexandre Alvaro
image: /img/upload/20200602-desligando-sistemas-embarcados-corretamente-capa.jpg
thumbnail: /img/upload/20200602-desligando-sistemas-embarcados-corretamente-thumb.jpg
categories:
  - Arduino
  - Raspberry
tags:
  - arduino
  - raspberry
  - tutorial
  - intermediário
  - prototipação
  - eletrônica
  - iot
  - soft power button
  - energia
---


# Introdução

Uma chave que simplesmente corta a energia abruptamente pode trazer sérios problemas para equipamentos com sistema operacional. Nos PCs com Windows nos anos 90 além de dar o comando de desligamento, precisávamos pressionar o botão de desligamento ao ver esta tela:  
![](/img/upload/20200602-pc-tela-desligar.jpg)  

Assim como o propósito das fontes ATX nos PCs, nós precisamos de algo para evitar corromper ou perder dados ao desligar dispositivos com sistema operacional embarcado, como o Raspberry Pi e similares. Da mesma forma em dispositivos microcontroladores utilizados em soluções IoT como os arduinos, nodeMCU (ESP8266, ESP32) muitas vezes precisam de um controle de energia mais otimizado para uso com baterias.

Então vou te mostrar algumas soluções que podem auxiliar na hora de bolar o hardware do nosso dispositivo.

# Raspberry Pi

Com base em alguns scripts que venho usando nos últimos anos bolei um jeito extremamente simples (1 linha de comando) para configurar um botão ligado ao Raspberry Pi com Raspbian para desligar e ligar o sistema suavemente, fechando tudo q precisa antes de cortar a energia.

## Requisitos

* Raspberry Pi com Raspbian
* Push-button (com ou sem LED)

> Se ainda não tiver o Raspbian instalado, não passe trabalho desnecessariamente. Utilize a ferramenta oficial pra gravar o Raspbian no cartão SD. E depois ligue o Raspberry Pi em um monitor com teclado e mouse pra configurar a instalação. 😊

# Microcontroladores

{{< rawhtml >}}

<iframe width="100%" height="453" src="https://www.tinkercad.com/embed/3beWFrFBNGm?editbtn=1" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"></iframe>
{{< /rawhtml >}}