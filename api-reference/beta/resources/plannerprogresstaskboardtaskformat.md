---
title: Тип ресурса plannerProgressTaskBoardTaskFormat
description: Ресурс **plannerProgressTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении "Ход выполнения" на доске задач (представлении с сортировкой по состоянию поля PercentComplete и столбцами "Не начато", "В процессе" и "Выполнено"). С каждым объектом task связан один объект **plannerProgressTaskBoardTaskFormat**.
ms.openlocfilehash: 8ff6f536920bafb8734f63ef9fe9b72f8c2b1acb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076994"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>Тип ресурса plannerProgressTaskBoardTaskFormat

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **plannerProgressTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении "Ход выполнения" на доске задач (представлении с сортировкой по состоянию поля PercentComplete и столбцами "Не начато", "В процессе" и "Выполнено"). С каждым объектом [task](plannertask.md) связан один объект **plannerProgressTaskBoardTaskFormat**.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |Чтение свойств и отношений объекта **plannerProgressTaskBoardTaskFormat**.|
|[Обновление](../api/plannerprogresstaskboardtaskformat-update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)    |Обновление объекта **plannerProgressTaskBoardTaskFormat**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор ресурса. Это 28 знаков без учета регистра. [Формат](tasks-identifiers-disclaimer.md) проверяются на службу.|
|orderHint|String|Указание, используемое для расположения задачи в представлении "Ход выполнения" на доске задач. Используемый формат описан [здесь](planner-order-hint-format.md).|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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