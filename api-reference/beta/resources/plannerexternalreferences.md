---
title: тип ресурса plannerExternalReferences
description: Ресурс **plannerExternalReferences** представляет коллекцию ссылок на задачу. Это открытый тип. Это часть объекта сведений о задачах. Значение в паре свойство-значение — объект externalReference.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 00d69ce50c3bfa1d5a9adca28ffae6ed88a9dc33
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473565"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="c6e6b-106">тип ресурса plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="c6e6b-106">plannerExternalReferences resource type</span></span>

<span data-ttu-id="c6e6b-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6e6b-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6e6b-108">Ресурс **plannerExternalReferences** представляет коллекцию ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="c6e6b-108">The **plannerExternalReferences** resource represents the collection of references on a task.</span></span> <span data-ttu-id="c6e6b-109">Это открытый тип.</span><span class="sxs-lookup"><span data-stu-id="c6e6b-109">This is an Open Type.</span></span> <span data-ttu-id="c6e6b-110">Это часть объекта [сведений о задачах.](plannertaskdetails.md)</span><span class="sxs-lookup"><span data-stu-id="c6e6b-110">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="c6e6b-111">Значение в паре свойство-значение — [объект externalReference.](plannerexternalreference.md)</span><span class="sxs-lookup"><span data-stu-id="c6e6b-111">The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="c6e6b-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6e6b-112">Properties</span></span>
<span data-ttu-id="c6e6b-113">Свойства открытого типа могут быть определены клиентом.</span><span class="sxs-lookup"><span data-stu-id="c6e6b-113">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="c6e6b-114">В этом случае клиент должен предоставить допустимые **URL-адреса** на основе протоколов **HTTP/HTTPS,** так как свойствами и их значениями должны быть [объекты externalReference.](plannerexternalreference.md)</span><span class="sxs-lookup"><span data-stu-id="c6e6b-114">In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects.</span></span> <span data-ttu-id="c6e6b-115">На основе OData имена свойств в Open Types не могут содержать следующие символы: , , , поэтому они `.` `:` должны быть `%` `@` `#` закодированы.</span><span class="sxs-lookup"><span data-stu-id="c6e6b-115">Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`, `@`, `#` so they need to be encoded.</span></span> <span data-ttu-id="c6e6b-116">Пример показан ниже.</span><span class="sxs-lookup"><span data-stu-id="c6e6b-116">Example is shown below.</span></span> <span data-ttu-id="c6e6b-117">Чтобы удалить ссылку, установите значение свойства `null` .</span><span class="sxs-lookup"><span data-stu-id="c6e6b-117">To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6e6b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6e6b-118">JSON representation</span></span>

<span data-ttu-id="c6e6b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6e6b-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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

## <a name="example"></a><span data-ttu-id="c6e6b-120">Пример</span><span class="sxs-lookup"><span data-stu-id="c6e6b-120">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


