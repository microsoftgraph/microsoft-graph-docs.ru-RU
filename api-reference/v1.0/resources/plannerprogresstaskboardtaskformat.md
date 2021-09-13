---
title: тип ресурса plannerProgressTaskBoardTaskFormat
description: Ресурс **plannerProgressTaskBoardTaskFormat** представляет сведения, используемые для правильного отрисовки задачи в представлении Progress of the Task Board (представление, организованное состоянием поля PercentComplete на объекте задачи, с столбцами для not Started, In Progress и Complete). Каждая задача будет иметь один **объект plannerProgressTaskBoardTaskFormat,** связанный с ним.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 0288b8c5ef99f4e72f019c6ffaee15bfe1022348
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59052939"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>тип ресурса plannerProgressTaskBoardTaskFormat

Пространство имен: microsoft.graph

Ресурс **plannerProgressTaskBoardTaskFormat** представляет сведения, используемые для правильного отрисовки задачи в представлении Progress of the Task Board (представление, организованное состоянием поля PercentComplete на объекте задачи, с столбцами для not Started, In Progress и Complete). Каждая [задача](plannertask.md) будет иметь один **объект plannerProgressTaskBoardTaskFormat,** связанный с ним.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md). |Чтение свойств и связей **объекта plannerProgressTaskBoardTaskFormat.**|
|[Обновление](../api/plannerprogresstaskboardtaskformat-update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md).    |Обновление **объекта plannerProgressTaskBoardTaskFormat.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. ID ресурса. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|orderHint|String|Указание, используемое для расположения задачи в окне "Ход выполнения" доски задач. Формат определяется, как описано [здесь](planner-order-hint-format.md).|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

