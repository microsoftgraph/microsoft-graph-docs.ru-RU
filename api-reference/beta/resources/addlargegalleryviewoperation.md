---
title: Тип ресурса addLargeGalleryViewOperation
description: Описывает формат ответа для операции, которая добавляет представление большой коллекции.
author: navali-msft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 312f3ea1d9c924e142e6b192a7f6542cc6e0cd19
ms.sourcegitcommit: 4ff6e89e89178cbd5aef8aa019e714d95817fae4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2022
ms.locfileid: "65017064"
---
# <a name="addlargegalleryviewoperation-resource-type"></a>Тип ресурса addLargeGalleryViewOperation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает формат ответа для операции, которая добавляет представление большой коллекции.

Наследуется от [commsOperation](commsoperation.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-|:-|:-|
| [Получение addLargeGalleryViewOperation](../api/addlargegalleryviewoperation-get.md) | [addLargeGalleryViewOperation](addlargegalleryviewoperation.md) | Получение состояния операции, которая добавляет представление большой коллекции к вызову. |

## <a name="properties"></a>Свойства

| Свойство                       | Тип                        | Описание                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | Контекст клиента.                                                                                                                               |
| id                             | String                      | Идентификатор операции сервера. Только для чтения.                                                                                             |
| resultInfo                     | [resultInfo](resultinfo.md) | Сведения о результате.  Только для чтения.                                                                                             |
| status                         | operationStatus             | Состояние операции. Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения.                                                 |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addLargeGalleryViewOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addLargeGalleryViewOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


