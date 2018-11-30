---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
ms.openlocfilehash: c45c63a2517848cf89d6780ee578b252508d72f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079823"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="0c25f-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="0c25f-105">educationTerm resource type</span></span>

> <span data-ttu-id="0c25f-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c25f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c25f-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c25f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c25f-108">Срок.</span><span class="sxs-lookup"><span data-stu-id="0c25f-108">A term.</span></span> <span data-ttu-id="0c25f-109">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="0c25f-109">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="0c25f-110">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="0c25f-110">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0c25f-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c25f-111">Properties</span></span>
| <span data-ttu-id="0c25f-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c25f-112">Property</span></span>     | <span data-ttu-id="0c25f-113">Тип</span><span class="sxs-lookup"><span data-stu-id="0c25f-113">Type</span></span>   |<span data-ttu-id="0c25f-114">Описание</span><span class="sxs-lookup"><span data-stu-id="0c25f-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c25f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="0c25f-115">displayName</span></span>| <span data-ttu-id="0c25f-116">String</span><span class="sxs-lookup"><span data-stu-id="0c25f-116">String</span></span>| <span data-ttu-id="0c25f-117">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="0c25f-117">Display name of the term.</span></span>| 
|<span data-ttu-id="0c25f-118">externalId</span><span class="sxs-lookup"><span data-stu-id="0c25f-118">externalId</span></span>|<span data-ttu-id="0c25f-119">String</span><span class="sxs-lookup"><span data-stu-id="0c25f-119">String</span></span>| <span data-ttu-id="0c25f-120">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="0c25f-120">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="0c25f-121">startDate</span><span class="sxs-lookup"><span data-stu-id="0c25f-121">startDate</span></span>|<span data-ttu-id="0c25f-122">Date</span><span class="sxs-lookup"><span data-stu-id="0c25f-122">Date</span></span>|<span data-ttu-id="0c25f-123">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="0c25f-123">Start of the term.</span></span>|
|<span data-ttu-id="0c25f-124">endDate</span><span class="sxs-lookup"><span data-stu-id="0c25f-124">endDate</span></span>|<span data-ttu-id="0c25f-125">Date</span><span class="sxs-lookup"><span data-stu-id="0c25f-125">Date</span></span>|<span data-ttu-id="0c25f-126">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="0c25f-126">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c25f-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0c25f-127">JSON representation</span></span>

<span data-ttu-id="0c25f-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c25f-128">The following is a JSON representation of the resource.</span></span>

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