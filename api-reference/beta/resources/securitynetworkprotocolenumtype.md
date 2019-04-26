---
title: Перечисление Секуритинетворкпротокол
description: Возможные значения для сетевого протокола.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b9b4d29bb3af7e52665c00801e5e38e9b208455b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572453"
---
# <a name="securitynetworkprotocol-enum"></a>Перечисление Секуритинетворкпротокол

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Возможные значения для сетевого протокола.

## <a name="members"></a>Элементы

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|–1|НеИзвестный протокол.|
|см|нуль|Протокол IP.|
|полученных|1 | Протокол управления сообщениями в Интернете.|
|режимы|2 | Протокол управления группами Интернет.|
|ГГП|3 | Протокол шлюза для шлюза.|
|IPv4|4 | Протокол Интернета версии 4.|
|tcp|6 | Протокол управления передачей.|
|ПУП|12 | Протокол универсальных пакетов парк.|
|протокола|17 | Протокол датаграммы пользователя.|
|IDP|22| Протокол датаграмм через Интернет.|
|поддерживающ|41| Протокол IP версии 6 (IPv6).|
|ipv6RoutingHeader|43| заголовок маршрутизации IPv6.|
|ipv6FragmentHeader|44| заголовок фрагмента IPv6.|
|Ипсеценкапсулатингсекуритипайлоад|50| заголовок полезных данных безопасности, включающий IPv6.|
|Ипсекаусентикатионхеадер|51| заголовок проверки поДлинности IPv6.|
|icmpV6|58| Протокол управления сообщениями в Интернете для IPv6.|
|ipv6NoNextHeader|59| IPv6: следующий заголовок отсутствует.|
|ipv6DestinationOptions|60| заголовок параметров назначения IPv6.|
|этаже|77| Протокол сетевого диска (неофициальный).|
|RAW|255| Протокол IP-пакетов RAW.|
|x|1000| Протокол обмена пакетами в Интернете.|
|возмож|1256| Последовательный протокол обмена пакетами.|
|Спксии|1257| Последовательный протокол обмена пакетами версии 2.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/securitynetworkprotocolenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
