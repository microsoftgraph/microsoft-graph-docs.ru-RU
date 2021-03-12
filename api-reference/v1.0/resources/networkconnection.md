---
title: тип ресурса networkConnection
description: Содержит сведения о сетевом подключении, связанном с оповещением.
localization_priority: Normal
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5671726ead3da811c109a9a2afe01c49b665e513
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719012"
---
# <a name="networkconnection-resource-type"></a>тип ресурса networkConnection

Пространство имен: microsoft.graph

Содержит сведения о сетевом подключении, связанном с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управляющего сетевым подключением (например, Facebook или SMTP).|
|destinationAddress|String|IP-адрес назначения (сетевого подключения).|
|destinationLocation|String|Расположение (сопоставление IP-адресов), связанное с назначением сетевого подключения.|
|destinationDomain|String|Часть домена назначения URL-адреса. (например, "www.contoso.com").|
|destinationPort|String|Порт назначения (сетевого подключения).|
|destinationUrl|String|Строка URL-адрес/строка URI сетевого подключения без учета параметров. (например, www.contoso.com/products/default.html')|
|direction|connectionDirection|Направление сетевого подключения. Возможные значения: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Дата регистрации домена назначения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|localDnsName|String|Локальное разрешение имен DNS, как оно отображается в локальном DNS-кэше хоста (например, в случае, если файл "хост" был подделан).|
|natDestinationAddress|String|IP-адрес назначения перевода сетевого адреса.|
|natDestinationPort|String|Порт назначения перевода сетевых адресов.|
|natSourceAddress|String|IP-адрес источника перевода сетевого адреса.|
|natSourcePort|String|Порт источника перевода сетевых адресов.|
|протокол|[securityNetworkProtocol](securitynetworkprotocol.md)|Сетевой протокол. Возможные значения: `unknown` `ip` , , `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` , `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` .|
|riskScore|String|Оценка риска сетевого подключения поставщика сгенерирована и рассчитана. Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.|
|sourceAddress|String|IP-адрес источника (то есть происхождения) (сетевого подключения).|
|sourceLocation|String|Расположение (по сопоставлению IP-адресов), связанное с источником сетевого подключения.|
|sourcePort|String|Ip-порт source (то есть происхождение) (сетевого подключения).|
|status|connectionStatus|Состояние сетевого подключения. Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|String|Параметры (суффикс) URL-адреса назначения.|

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

