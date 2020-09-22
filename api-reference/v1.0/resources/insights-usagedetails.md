---
title: Тип ресурса Усажедетаилс
description: Сложный тип, содержащий свойства используемых элементов. Сведения о том, когда ресурс был последний раз обращался (просматривался) или изменился (редактируется) пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 79007d71ef44971bfab250c22abc6795a6b38dd4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054765"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="e70e7-104">Тип ресурса Усажедетаилс</span><span class="sxs-lookup"><span data-stu-id="e70e7-104">usageDetails resource type</span></span>

<span data-ttu-id="e70e7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e70e7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e70e7-106">Сложный тип, содержащий свойства [используемых](insights-used.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="e70e7-106">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="e70e7-107">Сведения о том, когда ресурс был последний раз обращался (просматривался) или изменился (редактируется) пользователем.</span><span class="sxs-lookup"><span data-stu-id="e70e7-107">Information on when the resource was last accessed (viewed) or modified (edited) by the user.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e70e7-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e70e7-108">JSON representation</span></span>

<span data-ttu-id="e70e7-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e70e7-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e70e7-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="e70e7-110">Properties</span></span>

| <span data-ttu-id="e70e7-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="e70e7-111">Property</span></span>              | <span data-ttu-id="e70e7-112">Тип</span><span class="sxs-lookup"><span data-stu-id="e70e7-112">Type</span></span>          | <span data-ttu-id="e70e7-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e70e7-113">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="e70e7-114">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="e70e7-114">lastAccessedDateTime</span></span>                  | <span data-ttu-id="e70e7-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e70e7-115">DateTimeOffset</span></span>        | <span data-ttu-id="e70e7-116">Дата и время последнего обращения пользователя к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="e70e7-116">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="e70e7-117">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e70e7-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e70e7-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e70e7-118">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="e70e7-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e70e7-119">Read-only.</span></span>                      |
| <span data-ttu-id="e70e7-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e70e7-120">lastModifiedDateTime</span></span>              | <span data-ttu-id="e70e7-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e70e7-121">DateTimeOffset</span></span>        | <span data-ttu-id="e70e7-122">Дата и время последнего изменения ресурса пользователем.</span><span class="sxs-lookup"><span data-stu-id="e70e7-122">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="e70e7-123">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e70e7-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e70e7-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e70e7-124">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="e70e7-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e70e7-125">Read-only.</span></span>       |

