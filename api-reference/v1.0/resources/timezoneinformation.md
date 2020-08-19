---
title: Тип ресурса timeZoneInformation
description: Представляет часовой пояс. Поддерживаемый формат — Windows, а часовой пояс IP Numbers Authority (IANA) (также известный как часовой пояс Олсона).
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 81f1eb3f8abbdcf95b94407019807d0d002dc286
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811828"
---
# <a name="timezoneinformation-resource-type"></a>Тип ресурса timeZoneInformation

Пространство имен: microsoft.graph


Представляет часовой пояс. Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|alias|string|Идентификатор часового пояса.|
|displayName|string|Отображаемое имя часового пояса.|

## <a name="json-representation"></a>Представление в формате JSON

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
