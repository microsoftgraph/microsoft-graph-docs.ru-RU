---
title: Тип ресурса plannerChecklistItems
description: Ресурс **plannerChecklistItemCollection** представляет коллекцию элементов контрольного списка для задачи. Это открытый тип. Он является частью объекта сведений о задаче. Значение в паре "свойство-значение" представляет собой объект checklistItem.
ms.openlocfilehash: 44e64872c34a70062e847889576bd226d4fe51fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078966"
---
# <a name="plannerchecklistitems-resource-type"></a><span data-ttu-id="b96b6-106">Тип ресурса plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="b96b6-106">plannerChecklistItems resource type</span></span>

> <span data-ttu-id="b96b6-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b96b6-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b96b6-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b96b6-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b96b6-p103">Ресурс **plannerChecklistItemCollection** представляет коллекцию элементов контрольного списка для задачи. Это открытый тип. Он является частью объекта [сведений о задаче](plannertaskdetails.md). Значение в паре "свойство-значение" представляет собой объект [checklistItem](plannerchecklistitem.md).</span><span class="sxs-lookup"><span data-stu-id="b96b6-p103">The **plannerChecklistItemCollection** resource represents the collection of checklist items on a task. It is an Open Type. It is part of the [task details](plannertaskdetails.md) object. The value in the property-value pair is the [checklistItem](plannerchecklistitem.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="b96b6-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="b96b6-113">Properties</span></span>
<span data-ttu-id="b96b6-p104">Клиент может определять свойства открытого типа. В этом случае клиент должен указать идентификаторы **GUID** в качестве свойств, а их значения должны представлять собой объекты [checklistItem](plannerchecklistitem.md). Ниже показан пример. Чтобы удалить элемент в контрольном списке, задайте для свойства значение `null`.</span><span class="sxs-lookup"><span data-stu-id="b96b6-p104">Properties of an Open Type can be defined by the client. In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects. Example is shown below. To remove an item in the checklist, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b96b6-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b96b6-118">JSON representation</span></span>

<span data-ttu-id="b96b6-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b96b6-119">Here is a JSON representation of the resource</span></span>

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
<span data-ttu-id="b96b6-120">Пример:</span><span class="sxs-lookup"><span data-stu-id="b96b6-120">// Example</span></span>

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