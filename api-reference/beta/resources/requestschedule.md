---
title: тип ресурса requestSchedule
description: Расписание запросов может быть включено в запрос назначения пакета доступа и присутствует в назначении пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 33abd221d22d37cc58bcf3770b4e28fa78b77064
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718471"
---
# <a name="requestschedule-resource-type"></a><span data-ttu-id="6eab1-103">тип ресурса requestSchedule</span><span class="sxs-lookup"><span data-stu-id="6eab1-103">requestSchedule resource type</span></span>

<span data-ttu-id="6eab1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eab1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eab1-105">В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="6eab1-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="6eab1-106">Этот запрос может включать расписание, когда пользователь хотел бы получить назначение.</span><span class="sxs-lookup"><span data-stu-id="6eab1-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="6eab1-107">Назначение пакета доступа, которое является результатом такого запроса, также имеет расписание.</span><span class="sxs-lookup"><span data-stu-id="6eab1-107">An access package assignment that results from such a request also has a schedule.</span></span>

## <a name="properties"></a><span data-ttu-id="6eab1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6eab1-108">Properties</span></span>

| <span data-ttu-id="6eab1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6eab1-109">Property</span></span>     | <span data-ttu-id="6eab1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6eab1-110">Type</span></span>        | <span data-ttu-id="6eab1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6eab1-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6eab1-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6eab1-112">startDateTime</span></span>|<span data-ttu-id="6eab1-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eab1-113">DateTimeOffset</span></span>|<span data-ttu-id="6eab1-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6eab1-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6eab1-115">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6eab1-115">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="6eab1-116">истечение срока действия</span><span class="sxs-lookup"><span data-stu-id="6eab1-116">expiration</span></span>|[<span data-ttu-id="6eab1-117">expirationPattern</span><span class="sxs-lookup"><span data-stu-id="6eab1-117">expirationPattern</span></span>](expirationpattern.md)|<span data-ttu-id="6eab1-118">По истечении срока действия доступа.</span><span class="sxs-lookup"><span data-stu-id="6eab1-118">When the access should expire.</span></span>|
|<span data-ttu-id="6eab1-119">recurrence</span><span class="sxs-lookup"><span data-stu-id="6eab1-119">recurrence</span></span>|[<span data-ttu-id="6eab1-120">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="6eab1-120">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="6eab1-121">Для повторного доступа.</span><span class="sxs-lookup"><span data-stu-id="6eab1-121">For recurring access.</span></span> <span data-ttu-id="6eab1-122">Не используется в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="6eab1-122">Not used at present.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6eab1-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6eab1-123">JSON representation</span></span>

<span data-ttu-id="6eab1-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6eab1-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestSchedule"
}-->

```json
{
    "startDateTime": "2020-08-11T23:06:53.307Z",
    "expiration": {
        "endDateTime": "2020-09-10T23:06:53.307Z",
        "type": "afterDateTime"
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


