---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом plan связан объект details.
localization_priority: Normal
ms.openlocfilehash: 59064093b485b6c82bd5b2e0b59ca1868e8517e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867741"
---
# <a name="plannerplandetails-resource-type"></a>Тип ресурса plannerPlanDetails


Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом [plan](plannerplan.md) связан объект details.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |Чтение свойств и отношений объекта **plannerPlanDetails**.|
|[Обновление](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |Обновление объекта **plannerPlanDetails**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.|
|id|Строка| Только для чтения. Идентификатор сведений о плане. Это 28 знаков без учета регистра. [Формат](planner-identifiers-disclaimer.md) проверяются на службу.|
|sharedWith|[plannerUserIds](planneruserids.md)|Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, то для предоставления доступа к плану [группы](group.md) используйте API Групп. Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого. |

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
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
