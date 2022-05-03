---
title: Тип ресурса networkConnection
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-pc
ms.technology: microsoft-graph
author: preetikr
ms.openlocfilehash: 4e87cd2019f3dd4eeda73509857d34775017dd1b
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176826"
---
# <a name="networkconnection-resource-type"></a>Тип ресурса networkConnection

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о сетевом подключении, связанном с оповещением, с отслеживанием состояния.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т. д.).|
|destinationAddress|Строка|IP-адрес назначения (сетевого подключения).|
|destinationDomain|Строка|Часть целевого домена в URL-адресе назначения. (например, "www.contoso.com").|
|destinationLocation|Строка|Расположение (по сопоставлению IP-адресов), связанное с назначением сетевого подключения.|
|destinationPort|Строка|Порт назначения (сетевого подключения).|
|destinationUrl|Строка|Строка URL-адреса или URI сетевого подключения за исключением параметров. (например, "www.contoso.com/products/default.html")|
|direction|connectionDirection|Направление сетевого подключения. Возможные значения: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Дата регистрации целевого домена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|localDnsName|Строка|Локальное разрешение DNS-имен, которое отображается в локальном кэше DNS узла (например, в случае незаконного изменения файла hosts).|
|natDestinationAddress|Строка|IP-адрес назначения преобразования сетевых адресов.|
|natDestinationPort|Строка|Порт назначения преобразования сетевых адресов.|
|natSourceAddress|Строка|IP-адрес источника преобразования сетевых адресов.|
|natSourcePort|Строка|Исходный порт преобразования сетевых адресов.|
|Протокол|securityNetworkProtocol|Сетевой протокол. Возможные значения: `unknown`, , `ip``icmp`, , `igmp`, `ggp`, `ipv4`, `tcp``pup`, `udp``idp``ipv6RoutingHeader``ipv6`, `icmpV6``ipv6FragmentHeader``ipSecEncapsulatingSecurityPayload``ipSecAuthenticationHeader``ipv6NoNextHeader`, , `ipv6DestinationOptions`, , `nd`, `raw`, `ipx`, . `spx``spxII`|
|riskScore|Строка|Созданная поставщиком или вычисляемая оценка риска сетевого подключения. Рекомендуемый диапазон значений — 0–1, что соответствует проценту.|
|sourceAddress|Строка|Исходный (например, исходный) IP-адрес (сетевого подключения).|
|sourceLocation|Строка|Расположение (по сопоставлению IP-адресов), связанное с источником сетевого подключения.|
|sourcePort|Строка|Исходный (например, исходный) IP-порт (сетевого подключения).|
|status|connectionStatus|Состояние сетевого подключения. Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|String|Параметры (суффикс) целевого URL-адреса.|

### <a name="securitynetworkprotocol-values"></a>Значения securityNetworkProtocol

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|–1|Неизвестный протокол.|
|Ip|0|Протокол Интернета.|
|Icmp|1| Протокол сообщений управления Интернетом.|
|Igmp|2| Протокол управления интернет-группой.|
|Ggp|3| Протокол шлюза к шлюзу.|
|ipv4|4| Протокол Интернета версии 4.|
|tcp|6 | Протокол управления передачей.|
|Pup|12 | Универсальный протокол пакетов PARC.|
|Udp|17 | Протокол датаграммы пользователя.|
|Idp|22| Протокол internet Datagram.|
|ipv6|41| Internet Protocol version 6 (ipv6).|
|ipv6RoutingHeader|43| Заголовок маршрутизации ipv6.|
|ipv6FragmentHeader|44| Заголовок фрагмента ipv6.|
|ipSecEncapsulatingSecurityPayload|50| Инкапсуляция заголовка полезных данных безопасности ipv6.|
|IpSecAuthenticationHeader|51| Заголовок проверки подлинности ipv6.|
|icmpV6|58| Протокол сообщений управления Интернетом для ipv6.|
|ipv6NoNextHeader|59| ipv6 Без следующего заголовка.|
|ipv6DestinationOptions|60| Заголовок параметров назначения ipv6.|
|Nd|77| Протокол net Disk (неформальная версия).|
|Сырой|255| Необработанный протокол IP-пакетов.|
|Ipx|1000| Протокол Exchange пакетов Интернета.|
|Spx|1256| Протокол виртуализации Exchange пакетов.|
|spxII|1257| Протокол sequenced Packet Exchange версии 2.|

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


