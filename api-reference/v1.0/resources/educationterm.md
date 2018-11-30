---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
ms.openlocfilehash: a74ea283f153a535008003e6875018eb12a35d15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024360"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="6907e-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="6907e-105">educationTerm resource type</span></span>

<span data-ttu-id="6907e-106">Срок.</span><span class="sxs-lookup"><span data-stu-id="6907e-106">A term.</span></span> <span data-ttu-id="6907e-107">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="6907e-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="6907e-108">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="6907e-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6907e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6907e-109">Properties</span></span>
| <span data-ttu-id="6907e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6907e-110">Property</span></span>     | <span data-ttu-id="6907e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6907e-111">Type</span></span>   |<span data-ttu-id="6907e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6907e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6907e-113">displayName</span><span class="sxs-lookup"><span data-stu-id="6907e-113">displayName</span></span>| <span data-ttu-id="6907e-114">String</span><span class="sxs-lookup"><span data-stu-id="6907e-114">String</span></span>| <span data-ttu-id="6907e-115">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="6907e-115">Display name of the term.</span></span>| 
|<span data-ttu-id="6907e-116">externalId</span><span class="sxs-lookup"><span data-stu-id="6907e-116">externalId</span></span>|<span data-ttu-id="6907e-117">String</span><span class="sxs-lookup"><span data-stu-id="6907e-117">String</span></span>| <span data-ttu-id="6907e-118">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="6907e-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="6907e-119">startDate</span><span class="sxs-lookup"><span data-stu-id="6907e-119">startDate</span></span>|<span data-ttu-id="6907e-120">Date</span><span class="sxs-lookup"><span data-stu-id="6907e-120">Date</span></span>|<span data-ttu-id="6907e-121">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="6907e-121">Start of the term.</span></span>|
|<span data-ttu-id="6907e-122">endDate</span><span class="sxs-lookup"><span data-stu-id="6907e-122">endDate</span></span>|<span data-ttu-id="6907e-123">Date</span><span class="sxs-lookup"><span data-stu-id="6907e-123">Date</span></span>|<span data-ttu-id="6907e-124">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="6907e-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6907e-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6907e-125">JSON representation</span></span>

<span data-ttu-id="6907e-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6907e-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->