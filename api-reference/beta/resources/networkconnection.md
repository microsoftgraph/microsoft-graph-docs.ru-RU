---
title: тип ресурса networkConnection
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2221f38c4ba8f8e71030d540985fb93f415bfa19
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722113"
---
# <a name="networkconnection-resource-type"></a>тип ресурса networkConnection

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о сетевом подключении, связанном с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т.д.).|
|destinationAddress|String|IP-адрес назначения (сетевого подключения).|
|destinationDomain|String|Часть домена назначения URL-адреса. (например, "www.contoso.com").|
|destinationLocation|String|Расположение (сопоставление IP-адресов), связанное с назначением сетевого подключения.|
|destinationPort|String|Порт назначения (сетевого подключения).|
|destinationUrl|String|Строка URL-адрес/строка URI сетевого подключения без учета параметров. (например, www.contoso.com/products/default.html')|
|direction|connectionDirection|Направление сетевого подключения. Возможные значения: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Дата регистрации домена назначения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|localDnsName|String|Локальное разрешение имен DNS, как оно отображается в локальном DNS-кэше хоста (например, в случае, если файл "хост" был подделан).|
|natDestinationAddress|String|IP-адрес назначения перевода сетевого адреса.|
|natDestinationPort|String|Порт назначения перевода сетевых адресов.|
|natSourceAddress|String|IP-адрес источника перевода сетевого адреса.|
|natSourcePort|String|Порт источника перевода сетевых адресов.|
|протокол|securityNetworkProtocol|Сетевой протокол. Возможные значения: `unknown` `ip` , , `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` , `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` .|
|riskScore|String|Оценка риска сетевого подключения поставщика сгенерирована и рассчитана. Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.|
|sourceAddress|String|IP-адрес источника (то есть происхождения) (сетевого подключения).|
|sourceLocation|String|Расположение (по сопоставлению IP-адресов), связанное с источником сетевого подключения.|
|sourcePort|String|Ip-порт source (то есть происхождение) (сетевого подключения).|
|status|connectionStatus|Состояние сетевого подключения. Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|String|Параметры (суффикс) URL-адреса назначения.|

### <a name="securitynetworkprotocol-values"></a>значения securityNetworkProtocol

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|-1|Неизвестный протокол.|
|IP|0|Протокол Интернета.|
|icmp|1| Протокол сообщений управления Интернетом.|
|igmp|2 | Протокол управления интернет-группой.|
|ggp|3 | Протокол Gateway to Gateway.|
|ipv4|4 | Версия 4 протокола Интернета.|
|tcp|6 | Протокол управления передачей.|
|pup|12 | Универсальный протокол пакетов PARC.|
|udp|17 | Протокол пользовательской datagram.|
|idp|22| Протокол Internet Datagram.|
|ipv6|41| Версия 6 протокола Интернета (ipv6).|
|ipv6RoutingHeader|43| загодер маршрутивки ipv6.|
|ipv6FragmentHeader|44| Заглавная часть ipv6.|
|ipSecEncapsulatingSecurityPayload|50| ipv6 Encapsulating Security Payload header.|
|ipSecAuthenticationHeader|51| загона проверки подлинности ipv6.|
|icmpV6|58| Протокол сообщения управления Интернетом для ipv6.|
|ipv6NoNextHeader|59| ipv6 Нет следующего загона.|
|ipv6DestinationOptions|60| заглавная головка вариантов назначения ipv6.|
|nd|77| Протокол чистого диска (неофициальный).|
|raw|255| Необработанные протоколы пакетов IP.|
|ipx|1000| Протокол обмена пакетами в Интернете.|
|spx|1256| Секвенный протокол Exchange пакетов.|
|spxII|1257| Секвенсорный протокол Exchange пакетов версии 2.|

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


