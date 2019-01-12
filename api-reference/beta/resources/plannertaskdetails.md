---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом task связан объект details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84b7191822be56e881b31d99503fdcdc4097890c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941144"
---
# <a name="plannertaskdetails-resource-type"></a>Тип ресурса plannerTaskDetails

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом [task](plannertask.md) связан объект details.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerTaskDetails](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md) |Чтение свойств и отношений объекта **plannerTaskDetails**.|
|[Обновление](../api/plannertaskdetails-update.md) | [plannerTaskDetails](plannertaskdetails.md)    |Обновление объекта **plannerTaskDetails**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|Коллекция элементов контрольного списка задачи.|
|описание|Строка|Описание задачи.|
|id|String| Только для чтения. Идентификатор сведения о задаче. Это 28 знаков без учета регистра. [Формат](tasks-identifiers-disclaimer.md) проверяются на службу.|
|previewType|строка|Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.|
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
