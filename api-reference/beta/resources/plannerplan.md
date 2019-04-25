---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать группе и содержать коллекцию перечисление plannertasks. Он также может иметь коллекцию Планнербуккетс. Каждый объект Plan содержит объект Details, который может содержать дополнительные сведения о плане. Более подробную информацию о связях между группами, планами и задачами можно узнать в разделе Планировщик.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578871"
---
# <a name="plannerplan-resource-type"></a>Тип ресурса plannerPlan

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать [группе](group.md) и содержать коллекцию [перечисление plannertasks](plannertask.md). Он также может иметь коллекцию [планнербуккетс](plannerbucket.md). Каждый объект Plan содержит объект [Details](plannerplandetails.md) , который может содержать дополнительные сведения о плане. Более подробную информацию о связях между группами, планами и задачами можно узнать в разделе [планировщик](planner-overview.md).



## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |Чтение свойств и связей объекта **plannerPlan** .|
|[Перечисление сегментов](../api/plannerplan-list-buckets.md) |Коллекция [plannerBucket](plannerbucket.md)| Получение коллекции объектов **plannerBucket** .|
|[Перечисление задач](../api/plannerplan-list-tasks.md) |Коллекция [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask** .|
|[Обновление](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |Обновление объекта **plannerPlan** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания плана. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения. ИДЕНТИФИКАТОР плана. Содержит 28 знаков, учитывается регистр. [Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.|
|owner|String|Идентификатор [группы](group.md) , которой принадлежит план. Для задания этого поля должна существовать допустимая группа. После задания этого свойства это свойство невозможно обновить.|
|title|String|Обязательный. Название плана.|
|createdBy|[identitySet](identityset.md)|Только для чтения. Пользователь, создавший план.|
|контекстах|[plannerPlanContextCollection](plannerplancontextcollection.md);| Только для чтения. Дополнительные пользовательские взаимодействия, в которых используется этот план, представленный в виде записей [планнерпланконтекст](plannerplancontext.md) .|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|сегментов|Коллекция [plannerBucket](plannerbucket.md)| Только для чтения. Допускается значение null. Коллекция сегментов в плане.|
|подробности|[plannerPlanDetails](plannerplandetails.md);| Только для чтения. Допускается значение null. Дополнительные сведения о плане.|
|tasks|Коллекция [plannerTask](plannertask.md)| Только для чтения. Допускается значение null. Коллекция задач в плане.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
