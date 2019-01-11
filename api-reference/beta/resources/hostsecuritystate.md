---
title: Тип ресурса hostSecurityState
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 1ae1436dd9771d34c37542eb756f81a4f8f0306a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853377"
---
# <a name="hostsecuritystate-resource-type"></a>Тип ресурса hostSecurityState

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит с сохранением состояния сведения об узле (включая устройства, компьютеры и т. п.).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|полное доменное имя|Строка|Полное доменное имя (полное доменное имя) (например, machine.company.com) узла.|
|isAzureAadJoined|Логический|Значение true, если узел является домен, в состав доменных служб Active Directory Azure.|
|isAzureAadRegistered|Логический|Значение true, если узел зарегистрирован устройства регистрации Azure Active Directory (BYOD устройства - то есть, не полностью управляются предприятия).|
|isHybridAzureDomainJoined|Логический|Значение true, если узел присоединен к домену на локальный домен Active Directory.|
|netBiosName|Строка|Имя локального узла без DNS-имени домена.|
|операционная система|Строка|Операционной системы. (Например, Windows10, MacOS, RHEL, и т.д.).|
|privateIpAddress|Строка|Частный (не маршрутизируемые) адрес IPv4 или IPv6 [(см)](https://tools.ietf.org/html/rfc1918)во время оповещения.|
|publicIpAddress|Строка|Открыто маршрутизируемыми IPv4 или IPv6-адрес [(см)](https://tools.ietf.org/html/rfc1918)во время оповещения.|
|riskScore|Строка|Оценка риска поставщика создается/вычисляемые узла.  Рекомендуемое значение диапазона 0-1, который соответствует в процентах.|

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
