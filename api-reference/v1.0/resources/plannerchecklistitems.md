---
title: Тип ресурса Планнерчекклиститемс
description: Ресурс **планнерчекклиститемколлектион** представляет коллекцию элементов контрольного списка в задаче. Это открытый тип. Он является частью объекта сведений о задаче. Значение в параметре "свойство-значение" является объектом Чекклиститем.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6904d473ace51363f8cd292524456b378e6f4e86
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037530"
---
# <a name="plannerchecklistitems-resource-type"></a><span data-ttu-id="d741e-106">Тип ресурса Планнерчекклиститемс</span><span class="sxs-lookup"><span data-stu-id="d741e-106">plannerChecklistItems resource type</span></span>

<span data-ttu-id="d741e-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d741e-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d741e-108">Ресурс **планнерчекклиститемколлектион** представляет коллекцию элементов контрольного списка в задаче.</span><span class="sxs-lookup"><span data-stu-id="d741e-108">The **plannerChecklistItemCollection** resource represents the collection of checklist items on a task.</span></span> <span data-ttu-id="d741e-109">Это открытый тип.</span><span class="sxs-lookup"><span data-stu-id="d741e-109">It is an Open Type.</span></span> <span data-ttu-id="d741e-110">Он является частью объекта [сведений о задаче](plannertaskdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="d741e-110">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="d741e-111">Значение в параметре "свойство-значение" является объектом [чекклиститем](plannerchecklistitem.md) .</span><span class="sxs-lookup"><span data-stu-id="d741e-111">The value in the property-value pair is the [checklistItem](plannerchecklistitem.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="d741e-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="d741e-112">Properties</span></span>
<span data-ttu-id="d741e-113">Клиентская возможность может определять свойства открытого типа.</span><span class="sxs-lookup"><span data-stu-id="d741e-113">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="d741e-114">В этом случае клиент должен предоставлять **GUID** в качестве свойств, а их значения должны быть объектами [чекклиститем](plannerchecklistitem.md) .</span><span class="sxs-lookup"><span data-stu-id="d741e-114">In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects.</span></span> <span data-ttu-id="d741e-115">Пример показан ниже.</span><span class="sxs-lookup"><span data-stu-id="d741e-115">Example is shown below.</span></span> <span data-ttu-id="d741e-116">Чтобы удалить элемент в контрольном списке, присвойте свойству значение `null` .</span><span class="sxs-lookup"><span data-stu-id="d741e-116">To remove an item in the checklist, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d741e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d741e-117">JSON representation</span></span>

<span data-ttu-id="d741e-118">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d741e-118">Here is a JSON representation of the resource</span></span>

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
<span data-ttu-id="d741e-119">Примеры</span><span class="sxs-lookup"><span data-stu-id="d741e-119">// Example</span></span>

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

