---
title: accessReviewInactiveUsersQueryScope
description: Тип accessReviewQueryScope, который позволяет выбирать только неактивных пользователей в области обзора доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 51fc61ce186b0346bc065ddc5dfea40158758223
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469799"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a><span data-ttu-id="5ef81-103">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="5ef81-103">accessReviewInactiveUsersQueryScope resource type</span></span>

<span data-ttu-id="5ef81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ef81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="5ef81-105">Тип [accessReviewQueryScope,](../resources/accessreviewqueryscope.md) который позволяет выбирать только неактивных пользователей в области обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="5ef81-105">A type of [accessReviewQueryScope](../resources/accessreviewqueryscope.md) that allows only inactive users to be selected in the scope of an access review.</span></span>

<span data-ttu-id="5ef81-106">Наследует [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="5ef81-106">Inherits from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5ef81-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ef81-107">Properties</span></span>
|<span data-ttu-id="5ef81-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ef81-108">Property</span></span>|<span data-ttu-id="5ef81-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5ef81-109">Type</span></span>|<span data-ttu-id="5ef81-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5ef81-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ef81-111">inactiveDuration</span><span class="sxs-lookup"><span data-stu-id="5ef81-111">inactiveDuration</span></span>|<span data-ttu-id="5ef81-112">Duration</span><span class="sxs-lookup"><span data-stu-id="5ef81-112">Duration</span></span>|<span data-ttu-id="5ef81-113">Определяет продолжительность периода бездействия.</span><span class="sxs-lookup"><span data-stu-id="5ef81-113">Defines the length of the duration period of inactivity.</span></span> <span data-ttu-id="5ef81-114">Неактивность основана на последнем знаке даты пользователя.</span><span class="sxs-lookup"><span data-stu-id="5ef81-114">Inactivity is based on the last sign in date of the user.</span></span>|
|<span data-ttu-id="5ef81-115">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ef81-115">query</span></span>|<span data-ttu-id="5ef81-116">String</span><span class="sxs-lookup"><span data-stu-id="5ef81-116">String</span></span>|<span data-ttu-id="5ef81-117">Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="5ef81-117">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="5ef81-118">queryRoot</span><span class="sxs-lookup"><span data-stu-id="5ef81-118">queryRoot</span></span>|<span data-ttu-id="5ef81-119">String</span><span class="sxs-lookup"><span data-stu-id="5ef81-119">String</span></span>|<span data-ttu-id="5ef81-120">Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="5ef81-120">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="5ef81-121">queryType</span><span class="sxs-lookup"><span data-stu-id="5ef81-121">queryType</span></span>|<span data-ttu-id="5ef81-122">String</span><span class="sxs-lookup"><span data-stu-id="5ef81-122">String</span></span>|<span data-ttu-id="5ef81-123">Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="5ef81-123">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|

### <a name="supported-queries-for-accessreviewinactiveuserqueryscope-as-scope"></a><span data-ttu-id="5ef81-124">Поддерживаемые запросы для accessReviewInactiveUserQueryScope в качестве области</span><span class="sxs-lookup"><span data-stu-id="5ef81-124">Supported queries for accessReviewInactiveUserQueryScope as scope</span></span>
<span data-ttu-id="5ef81-125">Те же запросы, поддерживаемые [в accessReviewScope,](../resources/accessreviewscope.md) также поддерживаются в accessReviewInactiveUserQueryScope.</span><span class="sxs-lookup"><span data-stu-id="5ef81-125">The same queries supported on [accessReviewScope](../resources/accessreviewscope.md) are also supported on accessReviewInactiveUserQueryScope.</span></span> <span data-ttu-id="5ef81-126">Ниже приводится запрос.</span><span class="sxs-lookup"><span data-stu-id="5ef81-126">The following are the queries.</span></span> <span data-ttu-id="5ef81-127">Они поддерживаются как `scope` свойство [в accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5ef81-127">They are supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span>

|<span data-ttu-id="5ef81-128">Сценарий</span><span class="sxs-lookup"><span data-stu-id="5ef81-128">Scenario</span></span>| <span data-ttu-id="5ef81-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ef81-129">Query</span></span> |
|--|--|
| <span data-ttu-id="5ef81-130">Просмотр всех неактивных гостевых пользователей, назначенных группе</span><span class="sxs-lookup"><span data-stu-id="5ef81-130">Review all inactive guest users assigned to a group</span></span> | <span data-ttu-id="5ef81-131">/groups/{group ID}/transitiveMembers/microsoft.graph.user/? \$ count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="5ef81-131">/groups/{group ID}/transitiveMembers/microsoft.graph.user/?\$count=true&$filter=(userType eq 'Guest')</span></span> |
| <span data-ttu-id="5ef81-132">Просмотр всех неактивных пользователей, заметив группу</span><span class="sxs-lookup"><span data-stu-id="5ef81-132">Review all inactive users assigned to a group</span></span> | <span data-ttu-id="5ef81-133">/groups/{group ID}/transitiveMembers</span><span class="sxs-lookup"><span data-stu-id="5ef81-133">/groups/{group ID}/transitiveMembers</span></span> |
| <span data-ttu-id="5ef81-134">Просмотр всех неактивных гостевых пользователей, назначенных всем группам</span><span class="sxs-lookup"><span data-stu-id="5ef81-134">Review all inactive guest users assigned to all groups</span></span> | <span data-ttu-id="5ef81-135">./members/microsoft.graph.user/? \$ count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="5ef81-135">./members/microsoft.graph.user/?\$count=true&$filter=(userType eq 'Guest')</span></span> |


## <a name="relationships"></a><span data-ttu-id="5ef81-136">Связи</span><span class="sxs-lookup"><span data-stu-id="5ef81-136">Relationships</span></span>
<span data-ttu-id="5ef81-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5ef81-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ef81-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5ef81-138">JSON representation</span></span>
<span data-ttu-id="5ef81-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ef81-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInactiveUsersQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String",
  "inactiveDuration": "String (duration)"
}
```
