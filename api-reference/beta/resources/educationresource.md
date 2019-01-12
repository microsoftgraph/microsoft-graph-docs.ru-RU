---
title: Тип ресурса educationResource
description: Суперкласса для всех объектов ресурсов в системе. Ресурс связан с **назначения** и/или **отправки**, который представляет объект обучения, который
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9ac84fd9d661f31186ea65e95c680456cdabe221
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982122"
---
# <a name="educationresource-resource-type"></a>Тип ресурса educationResource

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Суперкласса для всех объектов ресурсов в системе. Ресурс связан с **назначения** и/или **отправки**, который представляет объект обучения, который раздать или передачи. Ресурс не могут создаваться напрямую; необходимо включить для подкласса, представляющий тип использования ресурсов.

Этот ресурс сохраняет общие свойства для всех типов ресурсов.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Создатель ресурса.|
|createdDateTime|Момент времени, когда был создан ресурса.  DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|displayName|Строка|Отображаемое имя ресурса.|
|lastModifiedBy|[identitySet](identityset.md)|Кто был последний пользователям изменять ресурса.|
|lastModifiedDateTime|DateTimeOffset|Момент времени, время последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
