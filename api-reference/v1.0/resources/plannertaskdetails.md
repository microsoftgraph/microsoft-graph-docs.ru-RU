---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. Каждый объект Task содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d22c932989b9c0d21350842babd9b4bbf420124c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035170"
---
# <a name="plannertaskdetails-resource-type"></a>Тип ресурса plannerTaskDetails

Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. Каждый объект [Task](plannertask.md) содержит объект Details.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerTaskDetails](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md); |Чтение свойств и связей объекта **plannerTaskDetails** .|
|[обновление](../api/plannertaskdetails-update.md); | [plannerTaskDetails](plannertaskdetails.md);    |Обновление объекта **plannerTaskDetails** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|Коллекция элементов контрольного списка задачи.|
|description|Строка|Описание задачи.|
|id|Строка| Только для чтения. Идентификатор сведений о задаче. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|previewType|string|Устанавливает тип предварительного просмотра задачи. Допустимые значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. `automatic` Если выбран отображаемый предварительный просмотр, то приложение просматривает задачу.|
|references|[plannerExternalReferences](plannerexternalreferences.md)|Коллекция ссылок на задачу.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
