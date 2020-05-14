---
title: Тип ресурса Усажедетаилс
description: Сложный тип, содержащий свойства используемых элементов. Сведения о том, когда ресурс был последний раз обращался (просматривался) или изменился (редактируется) пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: d73af15dc3578e9e6c0a568eebfd42480f7065e2
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2020
ms.locfileid: "44227026"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="529ae-104">Тип ресурса Усажедетаилс</span><span class="sxs-lookup"><span data-stu-id="529ae-104">usageDetails resource type</span></span>

<span data-ttu-id="529ae-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="529ae-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="529ae-106">Сложный тип, содержащий свойства [используемых](insights-used.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="529ae-106">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="529ae-107">Сведения о том, когда ресурс был последний раз обращался (просматривался) или изменился (редактируется) пользователем.</span><span class="sxs-lookup"><span data-stu-id="529ae-107">Information on when the resource was last accessed (viewed) or modified (edited) by the user.</span></span>


## <a name="json-representation"></a><span data-ttu-id="529ae-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="529ae-108">JSON representation</span></span>

<span data-ttu-id="529ae-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="529ae-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="529ae-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="529ae-110">Properties</span></span>

| <span data-ttu-id="529ae-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="529ae-111">Property</span></span>              | <span data-ttu-id="529ae-112">Тип</span><span class="sxs-lookup"><span data-stu-id="529ae-112">Type</span></span>          | <span data-ttu-id="529ae-113">Описание</span><span class="sxs-lookup"><span data-stu-id="529ae-113">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="529ae-114">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="529ae-114">lastAccessedDateTime</span></span>                  | <span data-ttu-id="529ae-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="529ae-115">DateTimeOffset</span></span>        | <span data-ttu-id="529ae-116">Дата и время последнего обращения пользователя к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="529ae-116">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="529ae-117">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="529ae-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="529ae-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="529ae-118">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="529ae-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="529ae-119">Read-only.</span></span>                      |
| <span data-ttu-id="529ae-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="529ae-120">lastModifiedDateTime</span></span>              | <span data-ttu-id="529ae-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="529ae-121">DateTimeOffset</span></span>        | <span data-ttu-id="529ae-122">Дата и время последнего изменения ресурса пользователем.</span><span class="sxs-lookup"><span data-stu-id="529ae-122">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="529ae-123">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="529ae-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="529ae-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="529ae-124">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="529ae-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="529ae-125">Read-only.</span></span>       |
