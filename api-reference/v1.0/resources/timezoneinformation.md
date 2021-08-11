---
title: Тип ресурса timeZoneInformation
description: Представляет часовой пояс. Поддерживаемый формат Windows и часовой пояс Internet Assigned Numbers Authority (IANA) (также известный как часовой пояс Olson)
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: caf7869afa20c8f2b9c0bd85e10e00f3773cf8567b54e209f4d0de34f9fda109
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54159843"
---
# <a name="timezoneinformation-resource-type"></a>Тип ресурса timeZoneInformation

Пространство имен: microsoft.graph


Представляет часовой пояс. Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|alias|string|Идентификатор часового пояса.|
|displayName|string|Отображаемое имя часового пояса.|

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

