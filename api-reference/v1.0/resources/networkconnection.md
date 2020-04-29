---
title: Тип ресурса networkConnection
description: Содержит сведения о состоянии сетевого подключения, связанного с оповещением.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 86986178bc7104118dfb4db83ae43f7780307fe6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447369"
---
# <a name="networkconnection-resource-type"></a>Тип ресурса networkConnection

Пространство имен: microsoft.graph

Содержит сведения о состоянии сетевого подключения, связанного с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т. д.).|
|дестинатионаддресс|String|Конечный IP-адрес (сетевого подключения).|
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
|Protocol|[securityNetworkProtocol](securitynetworkprotocol.md)|Сетевой протокол. Возможные `unknown`значения:, `ip`, `icmp`, `igmp` `ggp` `ipv4` `tcp` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII`,,,,,,, `ipv6FragmentHeader`,,,,,,,,,,,,,,,,,,. `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader`|
|riskScore|String|Созданный поставщиком/вычисляемый показатель риска для сетевого подключения. Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.|
|саурцеаддресс|String|Источник (то есть источник) IP-адрес сетевого подключения.|
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
