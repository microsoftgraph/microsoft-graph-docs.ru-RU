---
title: тип ресурса plannerChecklistItems
description: Ресурс **plannerChecklistItemCollection** представляет коллекцию элементов контрольного списка для задачи. Это открытый тип. Это часть объекта сведений о задачах. Значение в паре свойство-значение — это объект checklistItem.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 2badca7f220c3686e0064bf3624934d2d1d1a08c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129853"
---
# <a name="plannerchecklistitems-resource-type"></a>тип ресурса plannerChecklistItems

Пространство имен: microsoft.graph

Ресурс **plannerChecklistItemCollection** представляет коллекцию элементов контрольного списка для задачи. Это открытый тип. Это часть объекта [сведений о задачах.](plannertaskdetails.md) Значение в паре свойство-значение — это [объект checklistItem.](plannerchecklistitem.md)


## <a name="properties"></a>Свойства
Свойства открытого типа могут быть определены клиентом. В этом случае клиент должен предоставить **GUID-объекты** в качестве свойств, а их значения должны быть [объектами checklistItem.](plannerchecklistitem.md) Пример показан ниже. Чтобы удалить элемент в списке, установите значение свойства `null` .

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
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
Пример

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

