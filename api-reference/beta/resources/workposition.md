---
title: Тип ресурса Воркпоситион
description: Тип ресурса Воркпоситион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 086273e54d923054ce8e71ef1c67fb2bb4f7002a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519066"
---
# <a name="workposition-resource-type"></a>Тип ресурса Воркпоситион

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о должностных единицах, связанных с [профилем](profile.md)пользователя.

Этот тип ресурса наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

| Метод                                         | Возвращаемый тип                     | Описание                                               |
|:-----------------------------------------------|:--------------------------------|:----------------------------------------------------------|
| [Получение Воркпоситион](../api/workposition-get.md) | [воркпоситион](workposition.md) | Чтение свойств и связей объекта **воркпоситион** . |
| [Обновление Воркпоситион](../api/workposition-update.md)        | [воркпоситион](workposition.md) | Обновление объекта **воркпоситион** .                               |
| [Удаление Воркпоситион](../api/workposition-delete.md)        | Нет                            | Удаление объекта **воркпоситион** .                               |

## <a name="properties"></a>Свойства

| Свойство             | Тип                               | Описание                                                                                                |
|:---------------------|:-----------------------------------|:-----------------------------------------------------------------------------------------------------------|
|categories            |Коллекция String                   | Содержит категории, связанные с положением пользователя (например, цифровое преобразование, люди). |
|описаны                |[поситиондетаил](positiondetail.md) | Содержит подробные сведения о текущей и предыдущей позиции найма пользователя.                                 |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workPosition",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "detail": {"@odata.type": "microsoft.graph.positionDetail"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workPosition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
