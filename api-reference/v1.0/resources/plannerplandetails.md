---
title: тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый объект плана имеет объект подробностей.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8631aa508c73a4921cc1e3d6a1805acbbc7defbf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129812"
---
# <a name="plannerplandetails-resource-type"></a>тип ресурса plannerPlanDetails

Пространство имен: microsoft.graph


Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый [объект](plannerplan.md) плана имеет объект подробностей.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md); |Чтение свойств и связей **объекта plannerPlanDetails.**|
|[Обновление](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md);    |Объект **Update plannerPlanDetails.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.|
|id|String| Только для чтения. ID сведений плана. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|sharedWith|[plannerUserIds](planneruserids.md)|Набор пользовательских ids, с помощью которые мы делим этот план. Если вы используете Microsoft 365 группы, используйте API групп для управления членством в группе, чтобы поделиться [планом](group.md) группы. Вы также можете добавить в эту коллекцию существующих членов группы, хотя для них не требуется доступ к плану, который принадлежит группе. |

## <a name="relationships"></a>Отношения
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

