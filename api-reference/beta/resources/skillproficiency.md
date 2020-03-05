---
title: Тип ресурса СкиллпрофиЦиенци
description: Тип ресурса СкиллпрофиЦиенци
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6662ab205e390ae72d283d5015aa346c4b6fc2b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520508"
---
# <a name="skillproficiency-resource-type"></a>Тип ресурса СкиллпрофиЦиенци

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о навыках, связанных с пользователем в различных службах.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы
 
| Метод                                                 | Возвращаемый тип                             | Описание                                                   |
|:-------------------------------------------------------|:----------------------------------------|:--------------------------------------------------------------|
| [Получение СкиллпрофиЦиенци](../api/skillproficiency-get.md) | [скиллпрофиЦиенци](skillproficiency.md) | Чтение свойств и связей объекта **скиллпрофиЦиенци** . |
| [Обновление СкиллпрофиЦиенци](../api/skillproficiency-update.md)            | [скиллпрофиЦиенци](skillproficiency.md) | Обновление объекта **скиллпрофиЦиенци** .                               |
| [Удаление СкиллпрофиЦиенци](../api/skillproficiency-delete.md)            | Нет                                    | Удаление объекта **скиллпрофиЦиенци** .                               |

## <a name="properties"></a>Свойства

| Свойство     | Тип             | Описание                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|categories    |Коллекция String | Содержит категории, связанные с навыком пользователя (например, персональный, профессиональный, увлеченный).                                       |
|displayName   |Строка            | Содержит понятное имя для навыка.                                                                                            |      
|навыки   |строка            | Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.|
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
