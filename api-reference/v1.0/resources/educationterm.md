---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 59558512d27bb92c48fb5c0ac2dd0fb52f7c426d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531505"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="cd5a9-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="cd5a9-105">educationTerm resource type</span></span>

<span data-ttu-id="cd5a9-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd5a9-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd5a9-107">Срок.</span><span class="sxs-lookup"><span data-stu-id="cd5a9-107">A term.</span></span> <span data-ttu-id="cd5a9-108">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="cd5a9-108">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="cd5a9-109">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="cd5a9-109">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cd5a9-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd5a9-110">Properties</span></span>
| <span data-ttu-id="cd5a9-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd5a9-111">Property</span></span>     | <span data-ttu-id="cd5a9-112">Тип</span><span class="sxs-lookup"><span data-stu-id="cd5a9-112">Type</span></span>   |<span data-ttu-id="cd5a9-113">Описание</span><span class="sxs-lookup"><span data-stu-id="cd5a9-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd5a9-114">displayName</span><span class="sxs-lookup"><span data-stu-id="cd5a9-114">displayName</span></span>| <span data-ttu-id="cd5a9-115">Строка</span><span class="sxs-lookup"><span data-stu-id="cd5a9-115">String</span></span>| <span data-ttu-id="cd5a9-116">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="cd5a9-116">Display name of the term.</span></span>| 
|<span data-ttu-id="cd5a9-117">externalId</span><span class="sxs-lookup"><span data-stu-id="cd5a9-117">externalId</span></span>|<span data-ttu-id="cd5a9-118">String</span><span class="sxs-lookup"><span data-stu-id="cd5a9-118">String</span></span>| <span data-ttu-id="cd5a9-119">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="cd5a9-119">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="cd5a9-120">startDate</span><span class="sxs-lookup"><span data-stu-id="cd5a9-120">startDate</span></span>|<span data-ttu-id="cd5a9-121">Дата</span><span class="sxs-lookup"><span data-stu-id="cd5a9-121">Date</span></span>|<span data-ttu-id="cd5a9-122">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="cd5a9-122">Start of the term.</span></span>|
|<span data-ttu-id="cd5a9-123">endDate</span><span class="sxs-lookup"><span data-stu-id="cd5a9-123">endDate</span></span>|<span data-ttu-id="cd5a9-124">Date</span><span class="sxs-lookup"><span data-stu-id="cd5a9-124">Date</span></span>|<span data-ttu-id="cd5a9-125">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="cd5a9-125">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd5a9-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd5a9-126">JSON representation</span></span>

<span data-ttu-id="cd5a9-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd5a9-127">The following is a JSON representation of the resource.</span></span>

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
