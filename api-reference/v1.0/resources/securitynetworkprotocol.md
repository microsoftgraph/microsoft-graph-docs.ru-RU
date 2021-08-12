---
title: тип enum securityNetworkProtocol
description: Возможные значения для сетевого протокола.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: enumPageType
ms.openlocfilehash: 657d13f25707baa7f351622700700aa16a5d277b0d5dd1019843661af3491cb9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126293"
---
# <a name="securitynetworkprotocol-enum-type"></a>тип enum securityNetworkProtocol

Пространство имен: microsoft.graph

Возможные значения для сетевого протокола.

## <a name="members"></a>Элементы

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|-1|Неизвестный протокол.|
|IP|0|Протокол Интернета.|
|icmp|1| Протокол сообщений управления Интернетом.|
|igmp|2| Протокол управления интернет-группой.|
|ggp|3| Протокол Gateway to Gateway.|
|ipv4|4 | Версия 4 протокола Интернета.|
|tcp|6 | Протокол управления передачей.|
|pup|12 | Универсальный протокол пакетов PARC.|
|udp|17 | Протокол пользовательской datagram.|
|idp|22| Протокол Internet Datagram.|
|ipv6|41| Версия 6 протокола Интернета (ipv6).|
|ipv6RoutingHeader|43| загодер маршрутивки ipv6.|
|ipv6FragmentHeader|44| Заглавная часть ipv6.|
|ipSecEncapsulatingSecurityPayload|50| ipv6 Encapsulating Security Payload header.|
|ipSecAuthenticationHeader|51| загона проверки подлинности ipv6.|
|icmpV6|58| Протокол сообщения управления Интернетом для ipv6.|
|ipv6NoNextHeader|59| ipv6 Нет следующего загона.|
|ipv6DestinationOptions|60| заглавная головка вариантов назначения ipv6.|
|nd|77| Протокол чистого диска (неофициальный).|
|raw|255| Необработанные протоколы пакетов IP.|
|ipx|1000| Протокол пакета Exchange.|
|spx|1256| Секвенсорный Exchange пакетов.|
|spxII|1257| Последовательное пакет Exchange версии 2 протокола.|

