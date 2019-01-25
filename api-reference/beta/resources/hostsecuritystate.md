---
title: Тип ресурса hostSecurityState
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: d6f566a2bd42163c570fe837d2419057c62664bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526699"
---
# <a name="hostsecuritystate-resource-type"></a>Тип ресурса hostSecurityState

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит с сохранением состояния сведения об узле (включая устройства, компьютеры и т. п.).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|полное доменное имя|String|Полное доменное имя (полное доменное имя) (например, machine.company.com) узла.|
|isAzureAadJoined|Логическое|Значение true, если узел является домен, в состав доменных служб Active Directory Azure.|
|isAzureAadRegistered|Логическое|Значение true, если узел зарегистрирован устройства регистрации Azure Active Directory (BYOD устройства - то есть, не полностью управляются предприятия).|
|isHybridAzureDomainJoined|Логическое|Значение true, если узел присоединен к домену на локальный домен Active Directory.|
|netBiosName|String|Имя локального узла без DNS-имени домена.|
|И-5.|String|Операционной системы. (Например, Windows10, MacOS, RHEL, и т.д.).|
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
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/hostsecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
