---
title: Тип ресурса usageDetails
description: Сложный тип, содержащий свойства использовавшихся элементов. Сведения о время последнего обращения к ресурса (Просмотр) и изменить (изменить) для пользователя.
author: simonhult
ms.openlocfilehash: ef5efcfce439e9d08784637cb02657d7cd37adf7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349352"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="4f2ee-104">Тип ресурса usageDetails</span><span class="sxs-lookup"><span data-stu-id="4f2ee-104">usageDetails resource type</span></span>

> <span data-ttu-id="4f2ee-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4f2ee-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f2ee-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f2ee-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f2ee-107">Сложный тип, содержащий свойства [используется](insights-used.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="4f2ee-107">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="4f2ee-108">Сведения о время последнего обращения к ресурса (Просмотр) и изменить (изменить) для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f2ee-108">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f2ee-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f2ee-109">JSON representation</span></span>

<span data-ttu-id="4f2ee-110">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4f2ee-110">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="4f2ee-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f2ee-111">Properties</span></span>

| <span data-ttu-id="4f2ee-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f2ee-112">Property</span></span>              | <span data-ttu-id="4f2ee-113">Тип</span><span class="sxs-lookup"><span data-stu-id="4f2ee-113">Type</span></span>          | <span data-ttu-id="4f2ee-114">Описание</span><span class="sxs-lookup"><span data-stu-id="4f2ee-114">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="4f2ee-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f2ee-115">lastAccessedDateTime</span></span>                  | <span data-ttu-id="4f2ee-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f2ee-116">DateTimeOffset</span></span>        | <span data-ttu-id="4f2ee-117">Дата и время последнего обращения к пользователю ресурса.</span><span class="sxs-lookup"><span data-stu-id="4f2ee-117">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="4f2ee-118">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4f2ee-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4f2ee-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4f2ee-119">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="4f2ee-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f2ee-120">Read-only.</span></span>                      |
| <span data-ttu-id="4f2ee-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f2ee-121">lastModifiedDateTime</span></span>              | <span data-ttu-id="4f2ee-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f2ee-122">DateTimeOffset</span></span>        | <span data-ttu-id="4f2ee-123">Дата и время последнего изменения ресурса пользователем.</span><span class="sxs-lookup"><span data-stu-id="4f2ee-123">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="4f2ee-124">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4f2ee-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4f2ee-125">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4f2ee-125">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="4f2ee-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f2ee-126">Read-only.</span></span>       |