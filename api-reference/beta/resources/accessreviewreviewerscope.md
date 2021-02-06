---
title: Тип ресурса accessReviewReviewerScope
description: Представляет, кто будет рассматривать проверку доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c8a0644699daf7e204226d89bdd6cab6048888d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133492"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="21582-103">Тип ресурса accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="21582-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="21582-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21582-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21582-105">AccessReviewReviewerScope определяет, кто будет рассматривать экземпляры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="21582-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="21582-106">Это выражается в виде запроса OData, который позволяет рецензентам быть задан как статический список пользователей (т. е. определенных пользователей, владельцев групп, членов группы) или динамически (т. е. в случае, когда каждый пользователь просматривается руководителем).</span><span class="sxs-lookup"><span data-stu-id="21582-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span> <span data-ttu-id="21582-107">Чтобы создать самообзор (когда пользователи проверяют собственный доступ), не выдавайте рецензентов при создании [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="21582-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>


## <a name="properties"></a><span data-ttu-id="21582-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="21582-108">Properties</span></span>
| <span data-ttu-id="21582-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="21582-109">Property</span></span> | <span data-ttu-id="21582-110">Тип</span><span class="sxs-lookup"><span data-stu-id="21582-110">Type</span></span> | <span data-ttu-id="21582-111">Описание</span><span class="sxs-lookup"><span data-stu-id="21582-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="21582-112">Запрос</span><span class="sxs-lookup"><span data-stu-id="21582-112">query</span></span> | <span data-ttu-id="21582-113">Строка</span><span class="sxs-lookup"><span data-stu-id="21582-113">String</span></span> | <span data-ttu-id="21582-114">Запрос, определяющий, кто будет рецензентом.</span><span class="sxs-lookup"><span data-stu-id="21582-114">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="21582-115">Примеры см. в таблице.</span><span class="sxs-lookup"><span data-stu-id="21582-115">See table for examples.</span></span> |
| <span data-ttu-id="21582-116">queryType</span><span class="sxs-lookup"><span data-stu-id="21582-116">queryType</span></span> | <span data-ttu-id="21582-117">Строка</span><span class="sxs-lookup"><span data-stu-id="21582-117">String</span></span> | <span data-ttu-id="21582-118">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="21582-118">The type of query.</span></span> <span data-ttu-id="21582-119">Примеры: `MicrosoftGraph` и `ARM` .</span><span class="sxs-lookup"><span data-stu-id="21582-119">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="21582-120">queryRoot</span><span class="sxs-lookup"><span data-stu-id="21582-120">queryRoot</span></span> | <span data-ttu-id="21582-121">Строка</span><span class="sxs-lookup"><span data-stu-id="21582-121">String</span></span> | <span data-ttu-id="21582-122">В сценарии, где проверяющих необходимо указать динамически, это свойство используется для указать относительный источник запроса.</span><span class="sxs-lookup"><span data-stu-id="21582-122">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="21582-123">Это свойство необходимо, только если указан относительный запрос (например, ./manager).</span><span class="sxs-lookup"><span data-stu-id="21582-123">This property is only required if a relative query (i.e., ./manager) is specified.</span></span> |

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="21582-124">Поддерживаемые запросы для accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="21582-124">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="21582-125">Сценарий</span><span class="sxs-lookup"><span data-stu-id="21582-125">Scenario</span></span>| <span data-ttu-id="21582-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="21582-126">query</span></span> | <span data-ttu-id="21582-127">queryType</span><span class="sxs-lookup"><span data-stu-id="21582-127">queryType</span></span> | <span data-ttu-id="21582-128">queryRoot</span><span class="sxs-lookup"><span data-stu-id="21582-128">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="21582-129">Владелец группы в качестве рецензента</span><span class="sxs-lookup"><span data-stu-id="21582-129">Group owner as reviewer</span></span> | <span data-ttu-id="21582-130">/groups/{group id}/owners</span><span class="sxs-lookup"><span data-stu-id="21582-130">/groups/{group id}/owners</span></span> |<span data-ttu-id="21582-131">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="21582-131">MicrosoftGraph</span></span>||
| <span data-ttu-id="21582-132">Конкретный пользователь в качестве рецензента</span><span class="sxs-lookup"><span data-stu-id="21582-132">Specific user as reviewer</span></span> | <span data-ttu-id="21582-133">/users/{user id}</span><span class="sxs-lookup"><span data-stu-id="21582-133">/users/{user id}</span></span> |<span data-ttu-id="21582-134">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="21582-134">MicrosoftGraph</span></span>||
| <span data-ttu-id="21582-135">Руководитель пользователя, проверяемого в качестве рецензента</span><span class="sxs-lookup"><span data-stu-id="21582-135">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="21582-136">./manager</span><span class="sxs-lookup"><span data-stu-id="21582-136">./manager</span></span> | <span data-ttu-id="21582-137">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="21582-137">MicrosoftGraph</span></span> |<span data-ttu-id="21582-138">decisions</span><span class="sxs-lookup"><span data-stu-id="21582-138">decisions</span></span>|

## <a name="relationships"></a><span data-ttu-id="21582-139">Связи</span><span class="sxs-lookup"><span data-stu-id="21582-139">Relationships</span></span>
<span data-ttu-id="21582-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="21582-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="21582-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="21582-141">JSON representation</span></span>
<span data-ttu-id="21582-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21582-142">The following is a JSON representation of the resource.</span></span>
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
