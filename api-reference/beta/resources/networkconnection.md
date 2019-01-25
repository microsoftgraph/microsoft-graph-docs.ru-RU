---
title: Тип ресурса networkConnection
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: ce7de8d5a0f63c4d924e8092e4e9e05f984ec335
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515358"
---
# <a name="networkconnection-resource-type"></a>Тип ресурса networkConnection

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит информацию о состояниях о сетевое подключение, связанные с оповещение.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управление сетевое подключение (например, Facebook, SMTP, и т.д.).|
|destinationAddress|String|Конечный IP-адрес (сетевое подключение).|
|destinationDomain|String|Часть домена конечный URL-адрес назначения. (например «www.contoso.com»).|
|destinationPort|String|Порт назначения (сетевое подключение).|
|destinationUrl|String|Строка подключения URL-адрес или URI - исключение параметров в сети. (например, «www.contoso.com/products/default.html»)|
|Direction|connectionDirection|Направление подключения к сети. Возможные значения: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Дата регистрации целевом домене. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|localDnsName|String|Локальное разрешение имен DNS как оно отображается в локальном кэше DNS узла (например, в случае подделано файл «hosts»).|
|natDestinationAddress|String|Преобразование адресов конечный IP-адрес в сети.|
|natDestinationPort|String|Конечный порт преобразование адресов в сети.|
|natSourceAddress|String|Преобразование адресов исходный IP-адрес в сети.|
|natSourcePort|String|Порт источника, преобразование адресов сети.|
|protocol|[securityNetworkProtocol](securitynetworkprotocolenumtype.md)|Сетевой протокол. Возможные значения: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|String|Поставщик создан/вычисляется риск показатель для подключения к сети. Рекомендуемое значение диапазона 0-1, который соответствует в процентах.|
|sourceAddress|String|(То есть источник) IP-адрес источника (сетевое подключение).|
|sourcePort|String|Исходный (то есть источник) IP-адрес порт (сетевое подключение).|
|status|connectionStatus|Состояние подключения к сети. Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|String|Параметры (суффикс) URL-адрес назначения.|

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
