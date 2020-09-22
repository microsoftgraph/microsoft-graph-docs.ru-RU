---
title: Тип ресурса networkConnection
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: c111082fe0b9a2f2090de3fe3abb71a96fd4a80d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026588"
---
# <a name="networkconnection-resource-type"></a>Тип ресурса networkConnection

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о состоянии сетевого подключения, связанного с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т. д.).|
|дестинатионаддресс|String|Конечный IP-адрес (сетевого подключения).|
|дестинатиондомаин|String|Часть конечного домена, в которой находится конечный URL-адрес. (например, "www.contoso.com").|
|дестинатионлокатион|String|Расположение (по сопоставлению IP-адресов), связанное с назначением сетевого подключения.|
|дестинатионпорт|String|Порт назначения (для сетевого подключения).|
|дестинатионурл|String|URL-адрес сетевого подключения/URI-строка — без параметров. (например, "www.contoso.com/products/default.html")|
|direction|connectionDirection|Направление сетевого подключения. Возможные значения: `unknown`, `inbound`, `outbound`.|
|домаинрегистереддатетиме|DateTimeOffset|Дата регистрации конечного домена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|локалднснаме|String|Локальное разрешение DNS-имен, отображаемое в локальном кэше DNS узла (например, на случай, если файл hosts был подделан).|
|натдестинатионаддресс|String|IP-адрес назначения преобразования сетевых адресов.|
|натдестинатионпорт|String|Порт назначения преобразования сетевых адресов.|
|натсаурцеаддресс|String|IP-адрес источника преобразования сетевых адресов.|
|натсаурцепорт|String|Порт источника преобразования сетевых адресов.|
|Protocol|securityNetworkProtocol|Сетевой протокол. Возможные значения:,,,,,,,,,,, `unknown` `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` , `ipSecEncapsulatingSecurityPayload` , `ipSecAuthenticationHeader` , `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` ,,,,,,,,,,,,,,.|
|riskScore|String|Созданный поставщиком/вычисляемый показатель риска для сетевого подключения. Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.|
|саурцеаддресс|String|Источник (то есть источник) IP-адрес сетевого подключения.|
|sourceLocation|String|Расположение (по сопоставлению IP-адресов), связанное с источником сетевого подключения.|
|саурцепорт|String|Исходный (то есть источник) IP-порт (сетевого подключения).|
|status|connectionStatus|Состояние сетевого подключения. Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|урлпараметерс|String|Параметры (суффикс) конечного URL-адреса.|

### <a name="securitynetworkprotocol-values"></a>значения Секуритинетворкпротокол

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|–1|Неизвестный протокол.|
|см|нуль|Протокол IP.|
|полученных|1 | Протокол управления сообщениями в Интернете.|
|режимы|2 | Протокол управления группами Интернет.|
|ггп|4| Протокол шлюза для шлюза.|
|IPv4|4 | Протокол Интернета версии 4.|
|tcp|6 | Протокол управления передачей.|
|пуп|12 | Протокол универсальных пакетов парк.|
|протокола|17 | Протокол датаграммы пользователя.|
|IDP|22| Протокол датаграмм через Интернет.|
|поддерживающ|41| Протокол IP версии 6 (IPv6).|
|ipv6RoutingHeader|43| заголовок маршрутизации IPv6.|
|ipv6FragmentHeader|44| заголовок фрагмента IPv6.|
|ипсеценкапсулатингсекуритипайлоад|50| заголовок полезных данных безопасности, включающий IPv6.|
|ипсекаусентикатионхеадер|51| заголовок проверки подлинности IPv6.|
|icmpV6|58| Протокол управления сообщениями в Интернете для IPv6.|
|ipv6NoNextHeader|59| IPv6: следующий заголовок отсутствует.|
|ipv6DestinationOptions|60| заголовок параметров назначения IPv6.|
|этаже|77| Протокол сетевого диска (неофициальный).|
|RAW|255| Протокол IP-пакетов RAW.|
|x|1000| Протокол обмена пакетами в Интернете.|
|возмож|1256| Последовательный протокол обмена пакетами.|
|спксии|1257| Последовательный протокол обмена пакетами версии 2.|

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
  "destinationLocation": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "String",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "string",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourceLocation": "String",
  "sourcePort": "String",
  "status": "String",
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
  "suppressions": []
}
-->


