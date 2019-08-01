---
title: Тип ресурса networkConnection
description: Содержит сведения о состоянии сетевого подключения, связанного с оповещением.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 25750b5484558c53ab03d3001bc2b8bafa307524
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035996"
---
# <a name="networkconnection-resource-type"></a>Тип ресурса networkConnection

Содержит сведения о состоянии сетевого подключения, связанного с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т. д.).|
|Дестинатионаддресс|String|Конечный IP-адрес (сетевого подключения).|
|Дестинатиондомаин|String|Часть конечного домена, в которой находится конечный URL-адрес. (например, "www.contoso.com").|
|Дестинатионпорт|String|Порт назначения (для сетевого подключения).|
|Дестинатионурл|String|URL-адрес сетевого подключения/URI-строка — без параметров. (например, "www.contoso.com/products/default.html")|
|direction|connectionDirection|Направление сетевого подключения. Возможные значения: `unknown`, `inbound`, `outbound`.|
|Домаинрегистереддатетиме|DateTimeOffset|Дата регистрации конечного домена. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Локалднснаме|String|Локальное разрешение DNS-имен, отображаемое в локальном кэше DNS узла (например, на случай, если файл hosts был подделан).|
|Натдестинатионаддресс|String|IP-адрес назначения преобразования сетевых адресов.|
|Натдестинатионпорт|String|Порт назначения преобразования сетевых адресов.|
|Натсаурцеаддресс|String|IP-адрес источника преобразования сетевых адресов.|
|Натсаурцепорт|String|Порт источника преобразования сетевых адресов.|
|Protocol|[securityNetworkProtocol](securitynetworkprotocol.md)|Сетевой протокол. Возможные значения: `unknown`, `ip`, `icmp`, `igmp` `ggp` `ipv4` `tcp` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `ipv6RoutingHeader` `ipv6FragmentHeader`,,,,,,,,,,,,,,,,,,,,, `pup` `udp` `idp` `ipv6` , `raw`, `ipx`, `spx`, `spxII`.|
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
<!-- {
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
