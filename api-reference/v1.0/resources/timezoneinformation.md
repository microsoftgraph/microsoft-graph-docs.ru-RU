---
title: Тип ресурса timeZoneInformation
description: Представляет часовой пояс. Поддерживаемые формата является Windows и Internet Assigned Numbers Authority (IANA) часовой пояс (также известной как Олсон часовой пояс)
ms.openlocfilehash: de80ed293af834d299be5f9543c5c3bedde7a540
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024496"
---
# <a name="timezoneinformation-resource-type"></a>Тип ресурса timeZoneInformation


Представляет часовой пояс. Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|alias|string|Идентификатор часового пояса.|
|displayName|строка|Отображаемое имя часового пояса.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->