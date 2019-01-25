---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом task связан объект details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 579ecdbf43275de90468883d158af725eb1d1734
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512313"
---
# <a name="plannertaskdetails-resource-type"></a>Тип ресурса plannerTaskDetails

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом [task](plannertask.md) связан объект details.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerTaskDetails](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md); |Чтение свойств и отношений объекта **plannerTaskDetails**.|
|[Обновление](../api/plannertaskdetails-update.md) | [plannerTaskDetails](plannertaskdetails.md)    |Обновление объекта **plannerTaskDetails**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|Коллекция элементов контрольного списка задачи.|
|description|Строка|Описание задачи.|
|id|String| Только для чтения. Идентификатор сведения о задаче. Это 28 знаков без учета регистра. [Формат](tasks-identifiers-disclaimer.md) проверяются на службу.|
|previewType|string|Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.|
|references|[plannerExternalReferences](plannerexternalreferences.md)|Коллекция ссылок на задачу.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannertaskdetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
