---
title: Перечисление securityNetworkProtocol
description: Возможные значения для сетевого протокола.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b9b4d29bb3af7e52665c00801e5e38e9b208455b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511473"
---
# <a name="securitynetworkprotocol-enum"></a>Перечисление securityNetworkProtocol

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Возможные значения для сетевого протокола.

## <a name="members"></a>Элементы

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|–1|Неизвестный протокол.|
|IP|(0)|Протокол Интернета.|
|ICMP|$1| Протокол ICMP.|
|IGMP|–2| Протокол IGMP.|
|решение GGP|–3| Протокол шлюз-шлюз.|
|IPv4|4| Протокол IP версии 4.|
|TCP|6| Протокол.|
|PUP|1.2| Протокол универсальные пакетов PARC.|
|UDP-порт|1.7| Протокол.|
|IDP|%22| Протокол Интернета.|
|IP версии 6|4.1| Протокол IP версии 6 (ipv6).|
|ipv6RoutingHeader|4.3| Заголовок маршрутизации IPv6.|
|ipv6FragmentHeader|4.4| Заголовок IPv6 фрагмент кода.|
|ipSecEncapsulatingSecurityPayload|50%| Инкапсуляция полезных данных безопасности заголовка IPv6.|
|ipSecAuthenticationHeader|5.1| Заголовок проверки подлинности IPv6.|
|icmpV6|5.8| Протокол ICMP для ipv6.|
|ipv6NoNextHeader|5.9| IPv6 не следующий заголовок.|
|ipv6DestinationOptions|60| Параметры места назначения заголовка IPv6.|
|конец|7.7| NET протокол диска (неофициальный).|
|Raw|255| Необработанные пакетов протокола IP-адресов.|
|протокол IPX|1.0.0.0| Протокол Exchange пакетов.|
|SPX|1256| Протокол виртуализированный пакет Exchange.|
|spxII|1257| Виртуализированный пакет Exchange версии 2 протокола.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/securitynetworkprotocolenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
