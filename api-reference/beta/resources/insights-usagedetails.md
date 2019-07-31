---
title: Тип ресурса Усажедетаилс
description: Сложный тип, содержащий свойства используемых элементов. Сведения о том, когда ресурс был последний раз обращался (просматривался) и изменен (изменен) пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2b91275840546f0ff7486d8ecd5bdde2c1ff31e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005697"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="97a0a-104">Тип ресурса Усажедетаилс</span><span class="sxs-lookup"><span data-stu-id="97a0a-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97a0a-105">Сложный тип, содержащий свойства [используемых](insights-used.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="97a0a-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="97a0a-106">Сведения о том, когда ресурс был последний раз обращался (просматривался) и изменен (изменен) пользователем.</span><span class="sxs-lookup"><span data-stu-id="97a0a-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97a0a-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97a0a-107">JSON representation</span></span>

<span data-ttu-id="97a0a-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="97a0a-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usageDetails"
}-->

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="97a0a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="97a0a-109">Properties</span></span>

| <span data-ttu-id="97a0a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="97a0a-110">Property</span></span>              | <span data-ttu-id="97a0a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="97a0a-111">Type</span></span>          | <span data-ttu-id="97a0a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="97a0a-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="97a0a-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="97a0a-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="97a0a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97a0a-114">DateTimeOffset</span></span>        | <span data-ttu-id="97a0a-115">Дата и время последнего обращения пользователя к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="97a0a-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="97a0a-116">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="97a0a-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97a0a-117">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="97a0a-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="97a0a-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97a0a-118">Read-only.</span></span>                      |
| <span data-ttu-id="97a0a-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97a0a-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="97a0a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97a0a-120">DateTimeOffset</span></span>        | <span data-ttu-id="97a0a-121">Дата и время последнего изменения ресурса пользователем.</span><span class="sxs-lookup"><span data-stu-id="97a0a-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="97a0a-122">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="97a0a-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97a0a-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="97a0a-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="97a0a-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97a0a-124">Read-only.</span></span>       |
