---
title: Тип ресурса Планнерордерхинтсбяссигни
description: '**Планнерордерхинтсбяссигни** — это ресурс, который содержит подсказки упорядочения для уполномоченные в ресурсе plannerTask, чтобы указать порядок задачи, назначенный для представления доски задач.'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: c4c5099485c75c41e9ebb6275a7ffa5fed3be5a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035233"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>Тип ресурса Планнерордерхинтсбяссигни

**Планнерордерхинтсбяссигни** — это ресурс, который содержит [подсказки упорядочения](planner-order-hint-format.md) для уполномоченные в ресурсе [plannerTask](plannertask.md) , чтобы указать порядок задачи, назначенный для представления доски задач.
Этот тип является открытым типом. Свойства — это идентификаторы пользователей, назначенных задаче, а значения — подсказки порядка.

## <a name="properties"></a>Свойства
Клиентская возможность может определять свойства открытого типа. В этом случае клиент должен предоставить идентификаторы пользователей, назначенных задаче, в качестве имен свойств и допустимую [подсказку порядка](planner-order-hint-format.md) в качестве значения.
Невозможно удалить свойства из этого типа. Служба автоматически удалит значения, так как назначения для содержащегося [plannerTask](plannertask.md) будут обновлены.

Пример.

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
