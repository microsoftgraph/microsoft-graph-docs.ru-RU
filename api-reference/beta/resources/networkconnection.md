---
title: Тип ресурса networkConnection
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: ce7de8d5a0f63c4d924e8092e4e9e05f984ec335
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570724"
---
# <a name="networkconnection-resource-type"></a>Тип ресурса networkConnection

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о состоянии сетевого подключения, связанного с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т. д.).|
|Дестинатионаддресс|String|Конечный IP-адрес (сетевого подключения).|
|Дестинатиондомаин|String|Часть конечного домена, в которой находится конечный URL-адрес. (например, "www.contoso.com").|
|Дестинатионпорт|String|Порт назначения (для сетевого подключения).|
|Дестинатионурл|String|URL-адрес сетевого подключения/URI-строка — без параметров. (например, "www.contoso.com/products/Default.HTML")|
|direction|connectionDirection|Направление сетевого подключения. Возможные значения: `unknown`, `inbound`, `outbound`.|
|Домаинрегистереддатетиме|DateTimeOffset|Дата регистрации конечного домена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Локалднснаме|String|Локальное разрешение DNS-имен, отображаемое в локальном кэше DNS узла (например, на случай, если файл hosts был подделан).|
|Натдестинатионаддресс|String|IP-адрес назначения преобразования сетевых адресов.|
|Натдестинатионпорт|String|Порт назначения преобразования сетевых адресов.|
|Натсаурцеаддресс|String|IP-адрес источника преобразования сетевых адресов.|
|Натсаурцепорт|String|Порт источника преобразования сетевых адресов.|
|Protocol|[securityNetworkProtocol](securitynetworkprotocolenumtype.md)|Сетевой протокол. Возможные значения: `unknown`, `ip`, `icmp`, `igmp` `ggp` `ipv4` `tcp` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `ipv6RoutingHeader` `ipv6FragmentHeader`,,,,,,,,,,,,,,,,,,,,, `pup` `udp` `idp` `ipv6` , `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|String|Созданный поставщиком/вычисляемый показатель риска для сетевого подключения. Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.|
|Саурцеаддресс|String|Источник (то есть источник) IP-адрес сетевого подключения.|
|Саурцепорт|String|Исходный (то есть источник) IP-порт (сетевого подключения).|
|status|connectionStatus|Состояние сетевого подключения. Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|Урлпараметерс|String|Параметры (суффикс) конечного URL-адреса.|

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
