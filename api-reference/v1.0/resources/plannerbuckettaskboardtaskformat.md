---
title: тип ресурса plannerBucketTaskBoardTaskFormat
description: Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для правильного отрисовки задачи в представлении "Ведерки" доски задач (представление, организованное задачами в ведрах, на которые они назначены). Каждая задача будет иметь один **объект plannerBucketTaskBoardTaskFormat,** связанный с ним.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 809622d656a56b4f21c0660515602ab468c1f5e7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044323"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a>тип ресурса plannerBucketTaskBoardTaskFormat

Пространство имен: microsoft.graph

Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для правильного отрисовки задачи в представлении "Ведерки" доски задач (представление, организованное задачами в ведрах, на которые они назначены). Каждая [задача](plannertask.md) будет иметь один **объект plannerBucketTaskBoardTaskFormat,** связанный с ним.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-get.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md); |Чтение свойств и связей **объекта plannerBucketTaskBoardTaskFormat.**|
|[Обновление](../api/plannerbuckettaskboardtaskformat-update.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);  |Update **plannerBucketTaskBoardTaskFormat** object. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. ID ресурса. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|orderHint|String|Указание, используемое для расположения задач в окне "Сегмент" доски задачи. Формат определяется, как описано [здесь](planner-order-hint-format.md).|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

