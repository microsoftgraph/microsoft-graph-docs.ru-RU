---
title: Тип ресурса Рекуестсчедуле
description: Расписание запроса можно включить в запрос на назначение пакета Access и оно присутствует в назначении пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d5a80db31b0499648c5f297b613a198ddec6d25d
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413397"
---
# <a name="requestschedule-resource-type"></a><span data-ttu-id="26a15-103">Тип ресурса Рекуестсчедуле</span><span class="sxs-lookup"><span data-stu-id="26a15-103">requestSchedule resource type</span></span>

<span data-ttu-id="26a15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26a15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26a15-105">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="26a15-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="26a15-106">Этот запрос может включать расписание, когда пользователь хочет назначить назначение.</span><span class="sxs-lookup"><span data-stu-id="26a15-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="26a15-107">Назначение пакета Access, полученное в результате такого запроса, также имеет расписание.</span><span class="sxs-lookup"><span data-stu-id="26a15-107">An access package assignment that results from such a request also has a schedule.</span></span>

## <a name="properties"></a><span data-ttu-id="26a15-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="26a15-108">Properties</span></span>

| <span data-ttu-id="26a15-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="26a15-109">Property</span></span>     | <span data-ttu-id="26a15-110">Тип</span><span class="sxs-lookup"><span data-stu-id="26a15-110">Type</span></span>        | <span data-ttu-id="26a15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="26a15-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26a15-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="26a15-112">startDateTime</span></span>|<span data-ttu-id="26a15-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26a15-113">DateTimeOffset</span></span>|<span data-ttu-id="26a15-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="26a15-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="26a15-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="26a15-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="26a15-116">срока действия</span><span class="sxs-lookup"><span data-stu-id="26a15-116">expiration</span></span>|[<span data-ttu-id="26a15-117">експиратионпаттерн</span><span class="sxs-lookup"><span data-stu-id="26a15-117">expirationPattern</span></span>](expirationpattern.md)|<span data-ttu-id="26a15-118">По истечении срока действия доступа.</span><span class="sxs-lookup"><span data-stu-id="26a15-118">When the access should expire.</span></span>|
|<span data-ttu-id="26a15-119">recurrence</span><span class="sxs-lookup"><span data-stu-id="26a15-119">recurrence</span></span>|[<span data-ttu-id="26a15-120">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="26a15-120">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="26a15-121">Для повторяющегося доступа.</span><span class="sxs-lookup"><span data-stu-id="26a15-121">For recurring access.</span></span> <span data-ttu-id="26a15-122">Не используется в данный момент.</span><span class="sxs-lookup"><span data-stu-id="26a15-122">Not used at present.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26a15-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26a15-123">JSON representation</span></span>

<span data-ttu-id="26a15-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26a15-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestSchedule",
  "baseType": ""
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
