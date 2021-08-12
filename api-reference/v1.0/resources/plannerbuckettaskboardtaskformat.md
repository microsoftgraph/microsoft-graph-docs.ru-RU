---
title: тип ресурса plannerBucketTaskBoardTaskFormat
description: Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для правильного отрисовки задачи в представлении "Ведерки" доски задач (представление, организованное задачами в ведрах, на которые они назначены). Каждая задача будет иметь один **объект plannerBucketTaskBoardTaskFormat,** связанный с ним.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 38e159858591f7e1725c455e07162f9e0f10bbd1f8fc8d8bcfe974e952c95ae6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178118"
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
|id|String| Только для чтения. ID ресурса. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|orderHint|String|Указание, используемое для расположения задач в окне "Сегмент" доски задачи. Формат определяется, как описано [здесь](planner-order-hint-format.md).|

## <a name="relationships"></a>Связи
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

