---
title: Тип ресурса usageDetails
description: Сложный тип, содержащий свойства использовавшихся элементов. Сведения о время последнего обращения к ресурса (Просмотр) и изменить (изменить) для пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 04e064d5ebf8599466218722d89f46ececc5e58c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577489"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="8622d-104">Тип ресурса usageDetails</span><span class="sxs-lookup"><span data-stu-id="8622d-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8622d-105">Сложный тип, содержащий свойства [используется](insights-used.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="8622d-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="8622d-106">Сведения о время последнего обращения к ресурса (Просмотр) и изменить (изменить) для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8622d-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8622d-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8622d-107">JSON representation</span></span>

<span data-ttu-id="8622d-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="8622d-108">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="8622d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8622d-109">Properties</span></span>

| <span data-ttu-id="8622d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8622d-110">Property</span></span>              | <span data-ttu-id="8622d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8622d-111">Type</span></span>          | <span data-ttu-id="8622d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8622d-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="8622d-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="8622d-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="8622d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8622d-114">DateTimeOffset</span></span>        | <span data-ttu-id="8622d-115">Дата и время последнего обращения к пользователю ресурса.</span><span class="sxs-lookup"><span data-stu-id="8622d-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="8622d-116">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8622d-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8622d-117">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8622d-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8622d-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8622d-118">Read-only.</span></span>                      |
| <span data-ttu-id="8622d-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8622d-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="8622d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8622d-120">DateTimeOffset</span></span>        | <span data-ttu-id="8622d-121">Дата и время последнего изменения ресурса пользователем.</span><span class="sxs-lookup"><span data-stu-id="8622d-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="8622d-122">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8622d-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8622d-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8622d-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8622d-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8622d-124">Read-only.</span></span>       |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-usagedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
