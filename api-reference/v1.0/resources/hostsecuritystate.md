---
title: Тип ресурса hostSecurityState
description: Содержит с сохранением состояния сведения об узле (включая устройства, компьютеры и т. п.).
ms.openlocfilehash: 3649553ae0f96222a09825e8819dfd0d199f8454
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027197"
---
# <a name="hostsecuritystate-resource-type"></a>Тип ресурса hostSecurityState

Содержит с сохранением состояния сведения об узле (включая устройства, компьютеры и т. п.).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|полное доменное имя|String|Полное доменное имя (полное доменное имя) размещения (например, `machine.company.com`).|
|isAzureAadJoined|Логический|Значение true, если узел является домен, в состав доменных служб Active Directory Azure.|
|isAzureAadRegistered|Логический|Значение true, если узел зарегистрирован устройства регистрации Azure Active Directory (BYOD устройства - то есть, не полностью управляются предприятия).|
|isHybridAzureDomainJoined|Логический|Значение true, если узел присоединен к домену на локальный домен Active Directory.|
|netBiosName|String|Имя локального узла без DNS-имени домена.|
|операционная система|String|Операционной системы. (Например, Windows10, MacOS, RHEL, и т.д.).|
|privateIpAddress|String|Частный (не маршрутизируемые) адрес IPv4 или IPv6 [(см)](https://tools.ietf.org/html/rfc1918)во время оповещения.|
|publicIpAddress|String|Открыто маршрутизируемыми IPv4 или IPv6-адрес [(см)](https://tools.ietf.org/html/rfc1918)во время оповещения.|
|riskScore|String|Оценка риска поставщика создается/вычисляемые узла.  Рекомендуемое значение диапазона 0-1, который соответствует в процентах.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
