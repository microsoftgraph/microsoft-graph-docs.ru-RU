---
title: Тип ресурса plannerProgressTaskBoardTaskFormat
description: Ресурс **plannerProgressTaskBoardTaskFormat** представляет сведения, используемые для правильного отображения задачи в представлении "ход выполнения" доски задач (представление, организованное по состоянию поля PercentComplete в объекте Task со столбцами для Not started , Выполняется и завершено). Каждой задаче будет назначен один объект **plannerProgressTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6b92cbd231e0cd194b49c11c25d24b93933abbe7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035177"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>Тип ресурса plannerProgressTaskBoardTaskFormat

Ресурс **plannerProgressTaskBoardTaskFormat** представляет сведения, используемые для правильного отображения задачи в представлении "ход выполнения" доски задач (представление, организованное по состоянию поля PercentComplete в объекте Task со столбцами для Not started , Выполняется и завершено). Каждой [задаче](plannertask.md) будет назначен один объект **plannerProgressTaskBoardTaskFormat** .


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md). |Чтение свойств и связей объекта **plannerProgressTaskBoardTaskFormat** .|
|[обновление](../api/plannerprogresstaskboardtaskformat-update.md); | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md).    |Обновление объекта **plannerProgressTaskBoardTaskFormat** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор ресурса. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
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
