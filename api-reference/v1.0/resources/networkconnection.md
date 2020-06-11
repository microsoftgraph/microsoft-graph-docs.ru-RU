---
title: Тип ресурса networkConnection
description: Содержит сведения о состоянии сетевого подключения, связанного с оповещением.
localization_priority: Normal
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 72fcfcd3c6849e9c8e9f05b50671e1aa611dc129
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682056"
---
# <a name="networkconnection-resource-type"></a>Тип ресурса networkConnection

Пространство имен: microsoft.graph

Содержит сведения о состоянии сетевого подключения, связанного с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управляющего сетевым подключением (например, Facebook или SMTP).|
|дестинатионаддресс|String|Конечный IP-адрес (сетевого подключения).|
|дестинатионлокатион|String|Расположение (по сопоставлению IP-адресов), связанное с назначением сетевого подключения.|
|дестинатиондомаин|String|Часть конечного домена, в которой находится конечный URL-адрес. (например, "www.contoso.com").|
|дестинатионпорт|String|Порт назначения (для сетевого подключения).|
|дестинатионурл|String|URL-адрес сетевого подключения/URI-строка — без параметров. (например, "www.contoso.com/products/default.html")|
|direction|connectionDirection|Направление сетевого подключения. Возможные значения: `unknown`, `inbound`, `outbound`.|
|домаинрегистереддатетиме|DateTimeOffset|Дата регистрации конечного домена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|локалднснаме|String|Локальное разрешение DNS-имен, отображаемое в локальном кэше DNS узла (например, на случай, если файл hosts был подделан).|
|натдестинатионаддресс|String|IP-адрес назначения преобразования сетевых адресов.|
|натдестинатионпорт|String|Порт назначения преобразования сетевых адресов.|
|натсаурцеаддресс|String|IP-адрес источника преобразования сетевых адресов.|
|натсаурцепорт|String|Порт источника преобразования сетевых адресов.|
|Protocol|[securityNetworkProtocol](securitynetworkprotocol.md)|Сетевой протокол. Возможные значения:,,,,,,,,,,, `unknown` `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` , `ipSecEncapsulatingSecurityPayload` , `ipSecAuthenticationHeader` , `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` ,,,,,,,,,,,,,,.|
|riskScore|String|Созданный поставщиком/вычисляемый показатель риска для сетевого подключения. Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.|
|саурцеаддресс|String|Источник (то есть источник) IP-адрес сетевого подключения.|
|sourceLocation|String|Расположение (по сопоставлению IP-адресов), связанное с источником сетевого подключения.|
|саурцепорт|String|Исходный (то есть источник) IP-порт (сетевого подключения).|
|status|connectionStatus|Состояние сетевого подключения. Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|урлпараметерс|String|Параметры (суффикс) конечного URL-адреса.|

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
  "destinationLocation": "String",
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
  "sourceLocation": "String",
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
