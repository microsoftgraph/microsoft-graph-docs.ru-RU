---
title: Тип ресурса educationOrganization
description: 'Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.  '
author: mmast-msft
ms.openlocfilehash: 54f281de29033418b6acb2f9821c5ebd1eaf4db0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349891"
---
# <a name="educationorganization-resource-type"></a>Тип ресурса educationOrganization

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.  

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|описание|Строка| Описание организации.|
|displayName|Строка| Отображаемое имя организации.|
|externalSource|string| Источник, где был создан данной организации. Возможные значения: `sis`, `manual`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->