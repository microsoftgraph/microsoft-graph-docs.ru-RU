---
title: Тип ресурса СкиллпрофиЦиенци
description: Тип ресурса СкиллпрофиЦиенци
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7c8b5a3711c7abdbbdd8ddba8f7a36c85978718b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228875"
---
# <a name="skillproficiency-resource-type"></a>Тип ресурса СкиллпрофиЦиенци

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о навыках, связанных с пользователем в различных службах.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы
 
| Метод                                                         | Возвращаемый тип                             | Описание                                                             |
|:---------------------------------------------------------------|:----------------------------------------|:------------------------------------------------------------------------|
| [Получение СкиллпрофиЦиенци](../api/skillproficiency-get.md)         | [скиллпрофиЦиенци](skillproficiency.md) | Чтение свойств и связей объекта **скиллпрофиЦиенци** . |
| [Обновление СкиллпрофиЦиенци](../api/skillproficiency-update.md)   | [скиллпрофиЦиенци](skillproficiency.md) | Обновление объекта **скиллпрофиЦиенци** .                                   |
| [Удаление СкиллпрофиЦиенци](../api/skillproficiency-delete.md)   | Нет                                    | Удаление объекта **скиллпрофиЦиенци** .                                   |

## <a name="properties"></a>Свойства

| Свойство     | Тип             | Описание                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|categories    |Коллекция String | Содержит категории, связанные с навыком пользователя (например, персональный, профессиональный, увлеченный).                             |
|displayName   |Строка            | Содержит понятное имя для навыка.                                                                                            |
|навыки   |string            | Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.|
|webUrl        |String            | Содержит ссылку на источник информации о навыке.                                                                          |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

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
