---
title: тип ресурса accessReviewReviewerScope
description: Представляет, кто будет рассматривать обзор доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 68f353b81b6a14292828d82929a0eeac81d67bc5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469159"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="b5987-103">тип ресурса accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="b5987-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="b5987-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5987-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="b5987-105">AccessReviewReviewerScope определяет, кто будет рассматривать экземпляры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5987-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="b5987-106">Это выражается как запрос OData, который позволяет рецензентам быть указанными как статический список пользователей (например, конкретных пользователей, владельцев групп, членов группы) или динамически (т.е. в случае, когда каждый пользователь просматривается их менеджером).</span><span class="sxs-lookup"><span data-stu-id="b5987-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span> <span data-ttu-id="b5987-107">Чтобы создать самообзор (когда пользователи просматривают собственный доступ), не предоставлять рецензентов при создании [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5987-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>

<span data-ttu-id="b5987-108">Наследует [от accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="b5987-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b5987-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5987-109">Properties</span></span>
| <span data-ttu-id="b5987-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5987-110">Property</span></span> | <span data-ttu-id="b5987-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b5987-111">Type</span></span> | <span data-ttu-id="b5987-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b5987-112">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="b5987-113">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5987-113">query</span></span> | <span data-ttu-id="b5987-114">String</span><span class="sxs-lookup"><span data-stu-id="b5987-114">String</span></span> | <span data-ttu-id="b5987-115">Запрос, определяющий, кто будет рецензентом.</span><span class="sxs-lookup"><span data-stu-id="b5987-115">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="b5987-116">Примеры см. в таблице.</span><span class="sxs-lookup"><span data-stu-id="b5987-116">See table for examples.</span></span> |
| <span data-ttu-id="b5987-117">queryType</span><span class="sxs-lookup"><span data-stu-id="b5987-117">queryType</span></span> | <span data-ttu-id="b5987-118">String</span><span class="sxs-lookup"><span data-stu-id="b5987-118">String</span></span> | <span data-ttu-id="b5987-119">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="b5987-119">The type of query.</span></span> <span data-ttu-id="b5987-120">Примеры включают `MicrosoftGraph` и `ARM` .</span><span class="sxs-lookup"><span data-stu-id="b5987-120">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="b5987-121">queryRoot</span><span class="sxs-lookup"><span data-stu-id="b5987-121">queryRoot</span></span> | <span data-ttu-id="b5987-122">String</span><span class="sxs-lookup"><span data-stu-id="b5987-122">String</span></span> | <span data-ttu-id="b5987-123">В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса.</span><span class="sxs-lookup"><span data-stu-id="b5987-123">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="b5987-124">Это свойство требуется только в том случае, если указан относительный запрос (например, ./manager).</span><span class="sxs-lookup"><span data-stu-id="b5987-124">This property is only required if a relative query (i.e., ./manager) is specified.</span></span> |

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="b5987-125">Поддерживаемые запросы для accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="b5987-125">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="b5987-126">Сценарий</span><span class="sxs-lookup"><span data-stu-id="b5987-126">Scenario</span></span>| <span data-ttu-id="b5987-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5987-127">query</span></span> | <span data-ttu-id="b5987-128">queryType</span><span class="sxs-lookup"><span data-stu-id="b5987-128">queryType</span></span> | <span data-ttu-id="b5987-129">queryRoot</span><span class="sxs-lookup"><span data-stu-id="b5987-129">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="b5987-130">Владелец группы в качестве рецензента</span><span class="sxs-lookup"><span data-stu-id="b5987-130">Group owner as reviewer</span></span> | <span data-ttu-id="b5987-131">/groups/{group id}/owners</span><span class="sxs-lookup"><span data-stu-id="b5987-131">/groups/{group id}/owners</span></span> |<span data-ttu-id="b5987-132">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="b5987-132">MicrosoftGraph</span></span>||
| <span data-ttu-id="b5987-133">Конкретный пользователь в качестве рецензента</span><span class="sxs-lookup"><span data-stu-id="b5987-133">Specific user as reviewer</span></span> | <span data-ttu-id="b5987-134">/users/{user id}</span><span class="sxs-lookup"><span data-stu-id="b5987-134">/users/{user id}</span></span> |<span data-ttu-id="b5987-135">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="b5987-135">MicrosoftGraph</span></span>||
| <span data-ttu-id="b5987-136">Менеджер пользователя, проверяемого в качестве рецензента</span><span class="sxs-lookup"><span data-stu-id="b5987-136">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="b5987-137">./manager</span><span class="sxs-lookup"><span data-stu-id="b5987-137">./manager</span></span> | <span data-ttu-id="b5987-138">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="b5987-138">MicrosoftGraph</span></span> |<span data-ttu-id="b5987-139">решения</span><span class="sxs-lookup"><span data-stu-id="b5987-139">decisions</span></span>|
| <span data-ttu-id="b5987-140">Самообсвятие</span><span class="sxs-lookup"><span data-stu-id="b5987-140">Self Review</span></span> | <span data-ttu-id="b5987-141">Пустой список (без рецензентов)</span><span class="sxs-lookup"><span data-stu-id="b5987-141">Empty list(No reviewers)</span></span> | <span data-ttu-id="b5987-142">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="b5987-142">MicrosoftGraph</span></span>  |


## <a name="relationships"></a><span data-ttu-id="b5987-143">Связи</span><span class="sxs-lookup"><span data-stu-id="b5987-143">Relationships</span></span>
<span data-ttu-id="b5987-144">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b5987-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5987-145">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b5987-145">JSON representation</span></span>
<span data-ttu-id="b5987-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5987-146">The following is a JSON representation of the resource.</span></span>
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

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewerScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
