---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2d93bba585393b11cdb0adc573a8fed5b895ed6a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500011"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="8506c-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="8506c-105">educationTerm resource type</span></span>

<span data-ttu-id="8506c-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8506c-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8506c-107">Срок.</span><span class="sxs-lookup"><span data-stu-id="8506c-107">A term.</span></span> <span data-ttu-id="8506c-108">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="8506c-108">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="8506c-109">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="8506c-109">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8506c-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8506c-110">Properties</span></span>
| <span data-ttu-id="8506c-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="8506c-111">Property</span></span>     | <span data-ttu-id="8506c-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8506c-112">Type</span></span>   |<span data-ttu-id="8506c-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8506c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8506c-114">displayName</span><span class="sxs-lookup"><span data-stu-id="8506c-114">displayName</span></span>| <span data-ttu-id="8506c-115">String</span><span class="sxs-lookup"><span data-stu-id="8506c-115">String</span></span>| <span data-ttu-id="8506c-116">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="8506c-116">Display name of the term.</span></span>| 
|<span data-ttu-id="8506c-117">externalId</span><span class="sxs-lookup"><span data-stu-id="8506c-117">externalId</span></span>|<span data-ttu-id="8506c-118">String</span><span class="sxs-lookup"><span data-stu-id="8506c-118">String</span></span>| <span data-ttu-id="8506c-119">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8506c-119">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="8506c-120">startDate</span><span class="sxs-lookup"><span data-stu-id="8506c-120">startDate</span></span>|<span data-ttu-id="8506c-121">Дата</span><span class="sxs-lookup"><span data-stu-id="8506c-121">Date</span></span>|<span data-ttu-id="8506c-122">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="8506c-122">Start of the term.</span></span>|
|<span data-ttu-id="8506c-123">endDate</span><span class="sxs-lookup"><span data-stu-id="8506c-123">endDate</span></span>|<span data-ttu-id="8506c-124">Date</span><span class="sxs-lookup"><span data-stu-id="8506c-124">Date</span></span>|<span data-ttu-id="8506c-125">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="8506c-125">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8506c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8506c-126">JSON representation</span></span>

<span data-ttu-id="8506c-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8506c-127">The following is a JSON representation of the resource.</span></span>

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
