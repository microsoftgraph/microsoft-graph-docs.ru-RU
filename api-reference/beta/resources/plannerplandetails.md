---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый объект Plan содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 51bc28e93f7978fb080969de413db4e804918f6d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344405"
---
# <a name="plannerplandetails-resource-type"></a>Тип ресурса plannerPlanDetails

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый объект [Plan](plannerplan.md) содержит объект Details.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |Чтение свойств и связей объекта **plannerPlanDetails** .|
|[Обновление](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |Обновление объекта **plannerPlanDetails** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.|
|id|String| Только для чтения. Идентификатор сведений о плане. Содержит 28 знаков, учитывается регистр. [Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.|
|sharedWith|[plannerUserIds](planneruserids.md)|Набор идентификаторов пользователей, к которым предоставлен общий доступ к этому плану. Если вы используете группы Office 365, используйте API групп для управления членством в группах, чтобы поделиться планом [группы](group.md) . Вы также можете добавить существующих членов группы в эту коллекцию, хотя это не требуется для доступа к плану, принадлежащему группе. |
|Контекстдетаилс|[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md);|Только для чтения. Коллекция дополнительных сведений, связанных с записями [планнерпланконтекст](plannerplancontext.md) , которые определены для контейнера [plannerPlan](plannerplan.md) . |

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
