---
title: тип ресурса plannerOrderHintsByAssignee
description: '**PlannerOrderHintsByAssignee** — это ресурс, содержащий подсказки по заказу для назначенцев на ресурсе plannerTask, чтобы указать порядок задачи в назначенной для просмотра доски задач.'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: cfe6e1ac1bd0611eac9a2a39ce89814374371d19
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019239"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>тип ресурса plannerOrderHintsByAssignee

Пространство имен: microsoft.graph

**PlannerOrderHintsByAssignee** — это ресурс, содержащий подсказки по заказу для назначенцев на [ресурсе plannerTask,](plannertask.md) чтобы указать порядок задачи в назначенной для просмотра доски задач. [](planner-order-hint-format.md)
Этот тип — открытый тип. Свойства — это ids пользователей, задав задачу, а значения — подсказки порядка.

## <a name="properties"></a>Свойства
Свойства открытого типа могут быть определены клиентом. В этом случае клиент должен предоставить удостоверения пользователей, задав задачу в качестве имен свойств, и допустимый намек на заказ [в](planner-order-hint-format.md) качестве значения.
Свойства не могут быть удалены из этого типа. Служба автоматически удаляет значения по мере обновления назначений на содержащей [планировщикеTask.](plannertask.md)

Пример:

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

