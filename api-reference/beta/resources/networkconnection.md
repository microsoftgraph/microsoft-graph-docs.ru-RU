---
title: Тип ресурса networkConnection
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 6d28149854ed3157473b678db442ee3474e456c6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571921"
---
# <a name="networkconnection-resource-type"></a>Тип ресурса networkConnection

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит информацию о состояниях о сетевое подключение, связанные с оповещение.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управление сетевое подключение (например, Facebook, SMTP, и т.д.).|
|destinationAddress|Строка|Конечный IP-адрес (сетевое подключение).|
|destinationDomain|Строка|Часть домена конечный URL-адрес назначения. (например «www.contoso.com»).|
|destinationPort|Строка|Порт назначения (сетевое подключение).|
|destinationUrl|Строка|Строка подключения URL-адрес или URI - исключение параметров в сети. (например, «www.contoso.com/products/default.html»)|
|Направление|connectionDirection|Направление подключения к сети. Возможные значения: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Дата регистрации целевом домене. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|localDnsName|Строка|Локальное разрешение имен DNS как оно отображается в локальном кэше DNS узла (например, в случае подделано файл «hosts»).|
|natDestinationAddress|Строка|Преобразование адресов конечный IP-адрес в сети.|
|natDestinationPort|Строка|Конечный порт преобразование адресов в сети.|
|natSourceAddress|Строка|Преобразование адресов исходный IP-адрес в сети.|
|natSourcePort|Строка|Порт источника, преобразование адресов сети.|
|protocol| securityNetworkProtocol |Сетевой протокол. Возможные значения: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|Строка|Поставщик создан/вычисляется риск показатель для подключения к сети. Рекомендуемое значение диапазона 0-1, который соответствует в процентах.|
|sourceAddress|Строка|(То есть источник) IP-адрес источника (сетевое подключение).|
|sourcePort|Строка|Исходный (то есть источник) IP-адрес порт (сетевое подключение).|
|status|connectionStatus|Состояние подключения к сети. Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|Строка|Параметры (суффикс) URL-адрес назначения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkConnection"
}-->

```json
{
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "@odata.type: microsoft.graph.connectionDirection",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "@odata.type: microsoft.graph.connectionStatus",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/networkconnection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
