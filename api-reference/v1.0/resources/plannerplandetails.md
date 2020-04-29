---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый объект Plan содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e06afabfa01e7c63f103208bb0f290bcb58e4c56
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447110"
---
# <a name="plannerplandetails-resource-type"></a>Тип ресурса plannerPlanDetails

Пространство имен: microsoft.graph


Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый объект [Plan](plannerplan.md) содержит объект Details.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md); |Чтение свойств и связей объекта **plannerPlanDetails** .|
|[обновление](../api/plannerplandetails-update.md). | [plannerPlanDetails](plannerplandetails.md);    |Обновление объекта **plannerPlanDetails** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.|
|id|String| Только для чтения. Идентификатор сведений о плане. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|sharedWith|[plannerUserIds](planneruserids.md)|Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, используйте API Групп для предоставления доступа к плану [группы](group.md). Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого. |

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
