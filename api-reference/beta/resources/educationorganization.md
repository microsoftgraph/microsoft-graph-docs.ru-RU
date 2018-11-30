---
title: Тип ресурса educationOrganization
description: 'Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.  '
ms.openlocfilehash: 86da4e19f9cc36de7a61ca2c76565a17ec3acac0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077673"
---
# <a name="educationorganization-resource-type"></a>Тип ресурса educationOrganization

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.  

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|описание|String| Описание организации.|
|displayName|String| Отображаемое имя организации.|
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