---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e98bb1dc059439dfad927db033759ea54d240716
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340606"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="76776-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="76776-105">educationTerm resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76776-106">Срок.</span><span class="sxs-lookup"><span data-stu-id="76776-106">A term.</span></span> <span data-ttu-id="76776-107">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="76776-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="76776-108">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="76776-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="76776-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="76776-109">Properties</span></span>
| <span data-ttu-id="76776-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="76776-110">Property</span></span>     | <span data-ttu-id="76776-111">Тип</span><span class="sxs-lookup"><span data-stu-id="76776-111">Type</span></span>   |<span data-ttu-id="76776-112">Описание</span><span class="sxs-lookup"><span data-stu-id="76776-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76776-113">displayName</span><span class="sxs-lookup"><span data-stu-id="76776-113">displayName</span></span>| <span data-ttu-id="76776-114">String</span><span class="sxs-lookup"><span data-stu-id="76776-114">String</span></span>| <span data-ttu-id="76776-115">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="76776-115">Display name of the term.</span></span>| 
|<span data-ttu-id="76776-116">externalId</span><span class="sxs-lookup"><span data-stu-id="76776-116">externalId</span></span>|<span data-ttu-id="76776-117">String</span><span class="sxs-lookup"><span data-stu-id="76776-117">String</span></span>| <span data-ttu-id="76776-118">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="76776-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="76776-119">startDate</span><span class="sxs-lookup"><span data-stu-id="76776-119">startDate</span></span>|<span data-ttu-id="76776-120">Дата</span><span class="sxs-lookup"><span data-stu-id="76776-120">Date</span></span>|<span data-ttu-id="76776-121">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="76776-121">Start of the term.</span></span>|
|<span data-ttu-id="76776-122">endDate</span><span class="sxs-lookup"><span data-stu-id="76776-122">endDate</span></span>|<span data-ttu-id="76776-123">Date</span><span class="sxs-lookup"><span data-stu-id="76776-123">Date</span></span>|<span data-ttu-id="76776-124">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="76776-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76776-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76776-125">JSON representation</span></span>

<span data-ttu-id="76776-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76776-126">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
