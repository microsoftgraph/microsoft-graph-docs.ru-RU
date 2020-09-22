---
title: Тип ресурса Планнерекстерналреференцес
description: Ресурс **планнерекстерналреференцес** представляет коллекцию ссылок на задачу. Это открытый тип. Он является частью объекта сведений о задаче. Значение в параметре "свойство-значение" является объектом Екстерналреференце.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 0bf0945fb133e87d2dee3000c6084aa13e9638ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037488"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="ae5b5-106">Тип ресурса Планнерекстерналреференцес</span><span class="sxs-lookup"><span data-stu-id="ae5b5-106">plannerExternalReferences resource type</span></span>

<span data-ttu-id="ae5b5-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae5b5-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae5b5-108">Ресурс **планнерекстерналреференцес** представляет коллекцию ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="ae5b5-108">The **plannerExternalReferences** resource represents the collection of references on a task.</span></span> <span data-ttu-id="ae5b5-109">Это открытый тип.</span><span class="sxs-lookup"><span data-stu-id="ae5b5-109">This is an Open Type.</span></span> <span data-ttu-id="ae5b5-110">Он является частью объекта [сведений о задаче](plannertaskdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="ae5b5-110">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="ae5b5-111">Значение в параметре "свойство-значение" является объектом [екстерналреференце](plannerexternalreference.md) .</span><span class="sxs-lookup"><span data-stu-id="ae5b5-111">The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="ae5b5-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae5b5-112">Properties</span></span>
<span data-ttu-id="ae5b5-113">Клиентская возможность может определять свойства открытого типа.</span><span class="sxs-lookup"><span data-stu-id="ae5b5-113">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="ae5b5-114">В этом случае клиент должен предоставить **действительные URL-адреса** на основе протоколов **HTTP/HTTPS** , а их значения должны быть объектами [екстерналреференце](plannerexternalreference.md) .</span><span class="sxs-lookup"><span data-stu-id="ae5b5-114">In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects.</span></span> <span data-ttu-id="ae5b5-115">На основе OData имена свойств в открытых типах не могут содержать следующие символы: `.` , `:` и `%`  поэтому их необходимо закодировать.</span><span class="sxs-lookup"><span data-stu-id="ae5b5-115">Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded.</span></span> <span data-ttu-id="ae5b5-116">Пример показан ниже.</span><span class="sxs-lookup"><span data-stu-id="ae5b5-116">Example is shown below.</span></span> <span data-ttu-id="ae5b5-117">Чтобы удалить ссылку, присвойте свойству значение `null` .</span><span class="sxs-lookup"><span data-stu-id="ae5b5-117">To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae5b5-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae5b5-118">JSON representation</span></span>

<span data-ttu-id="ae5b5-119">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae5b5-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerExternalReferences"
}-->


```json
{
  "String-value":
  {
    "alias": "String-value",
    "lastModifiedBy": "String-value",
    "lastModifiedDateTime": "String(timestamp)",
    "previewPriority": "String-value",
    "type": "String-value"
  }
}
```

<span data-ttu-id="ae5b5-120">Примеры</span><span class="sxs-lookup"><span data-stu-id="ae5b5-120">// Example</span></span>

```json
{
  "https%3A//contoso%2Esharepoint%2Ecom/teams/agile/documents/AnnualReport%2Epptx":
  {
    "@odata.type": "microsoft.graph.externalReference", // required in PATCH requests to edit the references on a task
    "alias": "Agile Team Annual Report",
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedDateTime": "2015-09-21T17:45:12.039Z",
    "previewPriority": "0009005756397228702",
    "type": "PowerPoint"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

