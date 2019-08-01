---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 36426a7e3f1fb79264a788d8af7e7768f5bae26a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032622"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="41485-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="41485-105">educationTerm resource type</span></span>

<span data-ttu-id="41485-106">Срок.</span><span class="sxs-lookup"><span data-stu-id="41485-106">A term.</span></span> <span data-ttu-id="41485-107">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="41485-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="41485-108">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="41485-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="41485-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="41485-109">Properties</span></span>
| <span data-ttu-id="41485-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="41485-110">Property</span></span>     | <span data-ttu-id="41485-111">Тип</span><span class="sxs-lookup"><span data-stu-id="41485-111">Type</span></span>   |<span data-ttu-id="41485-112">Описание</span><span class="sxs-lookup"><span data-stu-id="41485-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41485-113">displayName</span><span class="sxs-lookup"><span data-stu-id="41485-113">displayName</span></span>| <span data-ttu-id="41485-114">String</span><span class="sxs-lookup"><span data-stu-id="41485-114">String</span></span>| <span data-ttu-id="41485-115">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="41485-115">Display name of the term.</span></span>| 
|<span data-ttu-id="41485-116">externalId</span><span class="sxs-lookup"><span data-stu-id="41485-116">externalId</span></span>|<span data-ttu-id="41485-117">String</span><span class="sxs-lookup"><span data-stu-id="41485-117">String</span></span>| <span data-ttu-id="41485-118">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="41485-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="41485-119">startDate</span><span class="sxs-lookup"><span data-stu-id="41485-119">startDate</span></span>|<span data-ttu-id="41485-120">Дата</span><span class="sxs-lookup"><span data-stu-id="41485-120">Date</span></span>|<span data-ttu-id="41485-121">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="41485-121">Start of the term.</span></span>|
|<span data-ttu-id="41485-122">endDate</span><span class="sxs-lookup"><span data-stu-id="41485-122">endDate</span></span>|<span data-ttu-id="41485-123">Date</span><span class="sxs-lookup"><span data-stu-id="41485-123">Date</span></span>|<span data-ttu-id="41485-124">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="41485-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41485-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41485-125">JSON representation</span></span>

<span data-ttu-id="41485-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41485-126">The following is a JSON representation of the resource.</span></span>

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
