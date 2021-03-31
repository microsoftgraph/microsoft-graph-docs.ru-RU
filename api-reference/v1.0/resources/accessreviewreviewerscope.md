---
title: тип ресурса accessReviewReviewerScope
description: Представляет, кто будет рассматривать обзор доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 55f881ff1bcb1b08cc66938fd8a7b4d28f540687
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469675"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="fa38f-103">тип ресурса accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="fa38f-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="fa38f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa38f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa38f-105">AccessReviewReviewerScope определяет, кто указан в [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) для просмотра [appConsentRequests](../resources/appconsentrequest.md) и [userConsentRequests](../resources/appconsentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="fa38f-105">The accessReviewReviewerScope defines who is specified in the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) to review [appConsentRequests](../resources/appconsentrequest.md) and [userConsentRequests](../resources/appconsentrequest.md).</span></span> <span data-ttu-id="fa38f-106">Это выражается как запрос OData, который позволяет рецензентам быть указанными как статический список пользователей (например, конкретных пользователей, владельцев групп, членов группы) или динамически (т.е. в случае, когда каждый пользователь просматривается их менеджером).</span><span class="sxs-lookup"><span data-stu-id="fa38f-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span>

## <a name="properties"></a><span data-ttu-id="fa38f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa38f-107">Properties</span></span>

|<span data-ttu-id="fa38f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa38f-108">Property</span></span>|<span data-ttu-id="fa38f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fa38f-109">Type</span></span>|<span data-ttu-id="fa38f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fa38f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa38f-111">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa38f-111">query</span></span>|<span data-ttu-id="fa38f-112">String</span><span class="sxs-lookup"><span data-stu-id="fa38f-112">String</span></span>|<span data-ttu-id="fa38f-113">Запрос, определяющий, кто будет рецензентом.</span><span class="sxs-lookup"><span data-stu-id="fa38f-113">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="fa38f-114">Примеры см. в таблице.</span><span class="sxs-lookup"><span data-stu-id="fa38f-114">See table for examples.</span></span> |
|<span data-ttu-id="fa38f-115">queryRoot</span><span class="sxs-lookup"><span data-stu-id="fa38f-115">queryRoot</span></span>|<span data-ttu-id="fa38f-116">String</span><span class="sxs-lookup"><span data-stu-id="fa38f-116">String</span></span>|<span data-ttu-id="fa38f-117">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="fa38f-117">The type of query.</span></span> <span data-ttu-id="fa38f-118">Примеры включают `MicrosoftGraph` и `ARM` .</span><span class="sxs-lookup"><span data-stu-id="fa38f-118">Examples include `MicrosoftGraph` and `ARM`.</span></span>|
|<span data-ttu-id="fa38f-119">queryType</span><span class="sxs-lookup"><span data-stu-id="fa38f-119">queryType</span></span>|<span data-ttu-id="fa38f-120">String</span><span class="sxs-lookup"><span data-stu-id="fa38f-120">String</span></span>|<span data-ttu-id="fa38f-121">В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса.</span><span class="sxs-lookup"><span data-stu-id="fa38f-121">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="fa38f-122">Это свойство требуется только в том случае, если указан относительный запрос (например, `./manager` ).</span><span class="sxs-lookup"><span data-stu-id="fa38f-122">This property is only required if a relative query (i.e., `./manager`) is specified.</span></span>|

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="fa38f-123">Поддерживаемые запросы для accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="fa38f-123">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="fa38f-124">Сценарий</span><span class="sxs-lookup"><span data-stu-id="fa38f-124">Scenario</span></span>| <span data-ttu-id="fa38f-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa38f-125">query</span></span> | <span data-ttu-id="fa38f-126">queryType</span><span class="sxs-lookup"><span data-stu-id="fa38f-126">queryType</span></span> | <span data-ttu-id="fa38f-127">queryRoot</span><span class="sxs-lookup"><span data-stu-id="fa38f-127">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="fa38f-128">Владелец группы в качестве рецензента</span><span class="sxs-lookup"><span data-stu-id="fa38f-128">Group owner as reviewer</span></span> | <span data-ttu-id="fa38f-129">/groups/{group id}/owners</span><span class="sxs-lookup"><span data-stu-id="fa38f-129">/groups/{group id}/owners</span></span> |<span data-ttu-id="fa38f-130">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="fa38f-130">MicrosoftGraph</span></span>||
| <span data-ttu-id="fa38f-131">Конкретный пользователь в качестве рецензента</span><span class="sxs-lookup"><span data-stu-id="fa38f-131">Specific user as reviewer</span></span> | <span data-ttu-id="fa38f-132">/users/{user id}</span><span class="sxs-lookup"><span data-stu-id="fa38f-132">/users/{user id}</span></span> |<span data-ttu-id="fa38f-133">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="fa38f-133">MicrosoftGraph</span></span>||
| <span data-ttu-id="fa38f-134">Менеджер пользователя, проверяемого в качестве рецензента</span><span class="sxs-lookup"><span data-stu-id="fa38f-134">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="fa38f-135">./manager</span><span class="sxs-lookup"><span data-stu-id="fa38f-135">./manager</span></span> | <span data-ttu-id="fa38f-136">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="fa38f-136">MicrosoftGraph</span></span> |<span data-ttu-id="fa38f-137">решения</span><span class="sxs-lookup"><span data-stu-id="fa38f-137">decisions</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa38f-138">Связи</span><span class="sxs-lookup"><span data-stu-id="fa38f-138">Relationships</span></span>

<span data-ttu-id="fa38f-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fa38f-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa38f-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fa38f-140">JSON representation</span></span>

<span data-ttu-id="fa38f-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa38f-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewerScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewerScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
