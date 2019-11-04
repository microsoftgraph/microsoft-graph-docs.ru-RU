---
title: Тип ресурса СкиллпрофиЦиенци
description: Тип ресурса СкиллпрофиЦиенци
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 9490947aea170f2b6e94ecd8f02f59d396746e3a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938711"
---
# <a name="skillproficiency-resource-type"></a>Тип ресурса СкиллпрофиЦиенци

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о навыках, связанных с самим пользователем в различных службах.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы
 
| Метод                                                 | Возвращаемый тип                             | Описание                                                   |
|:-------------------------------------------------------|:----------------------------------------|:--------------------------------------------------------------|
| [Получение СкиллпрофиЦиенци](../api/skillproficiency-get.md) | [скиллпрофиЦиенци](skillproficiency.md) | Чтение свойств и связей объекта СкиллпрофиЦиенци. |
| [Update](../api/skillproficiency-update.md)            | [скиллпрофиЦиенци](skillproficiency.md) | Обновление объекта СкиллпрофиЦиенци.                               |
| [Delete](../api/skillproficiency-delete.md)            | Нет.                                    | Удаление объекта СкиллпрофиЦиенци.                               |

## <a name="properties"></a>Свойства

| Свойство     | Тип             | Описание                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|categories    |Коллекция String | Содержит категории, связанные с навыком (например: личное, профессиональный, для увлечений)                                       |
|displayName   |Строка            | Содержит понятное имя для навыка.                                                                                            |      
|навыки   |string            | Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.|
|webUrl        |String            | Содержит ссылку на источник информации о навыке.                                                                          |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.skillProficiency",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "displayName": "String",
  "proficiency": "string",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "skillProficiency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->