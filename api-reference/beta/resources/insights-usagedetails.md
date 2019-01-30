---
title: Тип ресурса usageDetails
description: Сложный тип, содержащий свойства использовавшихся элементов. Сведения о время последнего обращения к ресурса (Просмотр) и изменить (изменить) для пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4df15bf635785aba054d52beb89b5ac04d48d3d3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641528"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="71c6c-104">Тип ресурса usageDetails</span><span class="sxs-lookup"><span data-stu-id="71c6c-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71c6c-105">Сложный тип, содержащий свойства [используется](insights-used.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="71c6c-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="71c6c-106">Сведения о время последнего обращения к ресурса (Просмотр) и изменить (изменить) для пользователя.</span><span class="sxs-lookup"><span data-stu-id="71c6c-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="71c6c-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71c6c-107">JSON representation</span></span>

<span data-ttu-id="71c6c-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="71c6c-108">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="71c6c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="71c6c-109">Properties</span></span>

| <span data-ttu-id="71c6c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="71c6c-110">Property</span></span>              | <span data-ttu-id="71c6c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="71c6c-111">Type</span></span>          | <span data-ttu-id="71c6c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="71c6c-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="71c6c-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="71c6c-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="71c6c-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c6c-114">DateTimeOffset</span></span>        | <span data-ttu-id="71c6c-115">Дата и время последнего обращения к пользователю ресурса.</span><span class="sxs-lookup"><span data-stu-id="71c6c-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="71c6c-116">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="71c6c-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="71c6c-117">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="71c6c-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="71c6c-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71c6c-118">Read-only.</span></span>                      |
| <span data-ttu-id="71c6c-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71c6c-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="71c6c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c6c-120">DateTimeOffset</span></span>        | <span data-ttu-id="71c6c-121">Дата и время последнего изменения ресурса пользователем.</span><span class="sxs-lookup"><span data-stu-id="71c6c-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="71c6c-122">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="71c6c-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="71c6c-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="71c6c-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="71c6c-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71c6c-124">Read-only.</span></span>       |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-usagedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
