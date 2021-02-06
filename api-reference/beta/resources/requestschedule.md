---
title: Тип ресурса requestSchedule
description: Расписание запроса может быть включено в запрос на назначение пакета доступа и присутствует в назначении пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 74fa9589552ba860962c73814e66332eda1c8e8f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132540"
---
# <a name="requestschedule-resource-type"></a><span data-ttu-id="9f249-103">Тип ресурса requestSchedule</span><span class="sxs-lookup"><span data-stu-id="9f249-103">requestSchedule resource type</span></span>

<span data-ttu-id="9f249-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f249-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f249-105">В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="9f249-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="9f249-106">Этот запрос может включать расписание для того, когда пользователь хочет получить назначение.</span><span class="sxs-lookup"><span data-stu-id="9f249-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="9f249-107">Назначение пакета доступа, которое является результатом такого запроса, также имеет расписание.</span><span class="sxs-lookup"><span data-stu-id="9f249-107">An access package assignment that results from such a request also has a schedule.</span></span>

## <a name="properties"></a><span data-ttu-id="9f249-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f249-108">Properties</span></span>

| <span data-ttu-id="9f249-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f249-109">Property</span></span>     | <span data-ttu-id="9f249-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9f249-110">Type</span></span>        | <span data-ttu-id="9f249-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9f249-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9f249-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9f249-112">startDateTime</span></span>|<span data-ttu-id="9f249-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f249-113">DateTimeOffset</span></span>|<span data-ttu-id="9f249-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9f249-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9f249-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9f249-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9f249-116">expiration</span><span class="sxs-lookup"><span data-stu-id="9f249-116">expiration</span></span>|[<span data-ttu-id="9f249-117">expirationPattern</span><span class="sxs-lookup"><span data-stu-id="9f249-117">expirationPattern</span></span>](expirationpattern.md)|<span data-ttu-id="9f249-118">По истечении срока действия доступа.</span><span class="sxs-lookup"><span data-stu-id="9f249-118">When the access should expire.</span></span>|
|<span data-ttu-id="9f249-119">recurrence</span><span class="sxs-lookup"><span data-stu-id="9f249-119">recurrence</span></span>|[<span data-ttu-id="9f249-120">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="9f249-120">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="9f249-121">Для повторяющегося доступа.</span><span class="sxs-lookup"><span data-stu-id="9f249-121">For recurring access.</span></span> <span data-ttu-id="9f249-122">В настоящее время не используется.</span><span class="sxs-lookup"><span data-stu-id="9f249-122">Not used at present.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f249-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9f249-123">JSON representation</span></span>

<span data-ttu-id="9f249-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f249-124">The following is a JSON representation of the resource.</span></span>

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


