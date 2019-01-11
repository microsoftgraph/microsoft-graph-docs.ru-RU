---
title: Тип ресурса plannerChecklistItems
description: Ресурс **plannerChecklistItemCollection** представляет коллекцию элементов контрольного списка для задачи. Это открытый тип. Он является частью объекта сведений о задаче. Значение в паре "свойство-значение" представляет собой объект checklistItem.
localization_priority: Normal
ms.openlocfilehash: f958289e22ccc7515fe0e79145bba5fb5188e660
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858627"
---
# <a name="plannerchecklistitems-resource-type"></a>Тип ресурса plannerChecklistItems

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **plannerChecklistItemCollection** представляет коллекцию элементов контрольного списка для задачи. Это открытый тип. Он является частью объекта [сведений о задаче](plannertaskdetails.md). Значение в паре "свойство-значение" представляет собой объект [checklistItem](plannerchecklistitem.md).


## <a name="properties"></a>Свойства
Клиент может определять свойства открытого типа. В этом случае клиент должен указать идентификаторы **GUID** в качестве свойств, а их значения должны представлять собой объекты [checklistItem](plannerchecklistitem.md). Ниже показан пример. Чтобы удалить элемент в контрольном списке, задайте для свойства значение `null`.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItems"
}-->

```json
{
  "String-value":
  {
    "isChecked": true,
    "lastModifiedBy": "String-value",
    "lastModifiedByDateTime": "String(timestamp)",
    "orderHint": "String-value",
    "title": "String-value"
  }
}
```
Пример:

```json
{
  "3a73c9dd-fb47-4230-9c0f-b80788fb0f9b": // client-generated GUID
  {
    "@odata.type": "microsoft.graph.checklistItem", // required in PATCH requests to edit the checklist on a task
    "isChecked": true,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0009005756397228702",
    "title": "Get stamps"
  },
  "5f36f5b2-1ec0-4c48-9c75-ed59429516c5":
  {
     "@odata.type": "microsoft.graph.checklistItem",
    "isChecked": false,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0004105723397228784",
    "title": "Mail card at UPS"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItems resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
