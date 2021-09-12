---
title: тип ресурса networkConnection
description: Содержит сведения о сетевом подключении, связанном с оповещением.
ms.localizationpriority: medium
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: edddb2f14458a0c4afd60465c687f618937f43e8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59006916"
---
# <a name="networkconnection-resource-type"></a>тип ресурса networkConnection

Пространство имен: microsoft.graph

Содержит сведения о сетевом подключении, связанном с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управляющего сетевым подключением (например, Facebook или SMTP).|
|destinationAddress|Строка|IP-адрес назначения (сетевого подключения).|
|destinationLocation|Строка|Расположение (сопоставление IP-адресов), связанное с назначением сетевого подключения.|
|destinationDomain|String|Часть домена назначения URL-адреса. (например, "www.contoso.com").|
|destinationPort|Строка|Порт назначения (сетевого подключения).|
|destinationUrl|Строка|Строка URL-адрес/строка URI сетевого подключения без учета параметров. (например, www.contoso.com/products/default.html')|
|direction|connectionDirection|Направление сетевого подключения. Возможные значения: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Дата регистрации домена назначения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|localDnsName|Строка|Локальное разрешение имен DNS, как оно отображается в локальном DNS-кэше хоста (например, в случае, если файл "хост" был подделан).|
|natDestinationAddress|Строка|IP-адрес назначения перевода сетевого адреса.|
|natDestinationPort|Строка|Порт назначения перевода сетевых адресов.|
|natSourceAddress|Строка|IP-адрес источника перевода сетевого адреса.|
|natSourcePort|Строка|Порт источника перевода сетевых адресов.|
|протокол|[securityNetworkProtocol](securitynetworkprotocol.md)|Сетевой протокол. Возможные значения: `unknown` `ip` , , `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` , `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` .|
|riskScore|Строка|Оценка риска сетевого подключения поставщика сгенерирована и рассчитана. Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.|
|sourceAddress|Строка|IP-адрес источника (то есть происхождения) (сетевого подключения).|
|sourceLocation|Строка|Расположение (по сопоставлению IP-адресов), связанное с источником сетевого подключения.|
|sourcePort|Строка|Ip-порт source (то есть происхождение) (сетевого подключения).|
|status|connectionStatus|Состояние сетевого подключения. Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|Строка|Параметры (суффикс) URL-адреса назначения.|

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

