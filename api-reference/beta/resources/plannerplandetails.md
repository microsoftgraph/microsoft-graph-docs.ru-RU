---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом plan связан объект details.
localization_priority: Normal
ms.openlocfilehash: 117a2f69324180a7ef45dcf96c773f510bdbcb9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860160"
---
# <a name="plannerplandetails-resource-type"></a>Тип ресурса plannerPlanDetails

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом [plan](plannerplan.md) связан объект details.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |Чтение свойства и связи объекта **plannerPlanDetails** .|
|[Обновление](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |Обновление объекта **plannerPlanDetails** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.|
|id|Строка| Только для чтения. Идентификатор сведений о плане. Это 28 знаков без учета регистра. [Формат](tasks-identifiers-disclaimer.md) проверяются на службу.|
|sharedWith|[plannerUserIds](planneruserids.md)|Набор, этот план используется совместно с идентификаторами пользователей. Если вы используете Office 365 групп, используйте группы API для управления членством в группе для совместного использования плана [группы](group.md) . Можно также добавить существующих членов группы этой коллекции, несмотря на то, что в порядке их для доступа к плана, принадлежащих группе не требуется. |
|contextDetails|[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md);|Только для чтения. Коллекция Дополнительные сведения, связанные с записями [plannerPlanContext](plannerplancontext.md) , определенных для контейнера [plannerPlan](plannerplan.md) . |

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "contextDetails": {"@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
