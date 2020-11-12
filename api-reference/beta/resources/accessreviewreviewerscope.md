---
title: Тип ресурса Акцессревиевревиеверскопе
description: Указывает, кто будет просматривать проверку доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: edc25e19a51f787dd0799fbd9e6e6c2a1b45787e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001059"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="fe749-103">Тип ресурса Акцессревиевревиеверскопе</span><span class="sxs-lookup"><span data-stu-id="fe749-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="fe749-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe749-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe749-105">Акцессревиевревиеверскопе определяет, кто будет проверять экземпляры объекта [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fe749-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="fe749-106">Он выражается в виде запроса OData, который позволяет предоставлять проверяющих как статический список пользователей (например, определенных пользователей, владельцев группы, членов группы) или динамически (например, в случае, если каждый пользователь просматривается руководителем).</span><span class="sxs-lookup"><span data-stu-id="fe749-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span> <span data-ttu-id="fe749-107">Чтобы создать самостоятельный обзор (где пользователи просматривают собственный доступ), не предоставляйте проверяющих при создании [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="fe749-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>


## <a name="properties"></a><span data-ttu-id="fe749-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe749-108">Properties</span></span>
| <span data-ttu-id="fe749-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe749-109">Property</span></span> | <span data-ttu-id="fe749-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fe749-110">Type</span></span> | <span data-ttu-id="fe749-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fe749-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="fe749-112">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe749-112">query</span></span> | <span data-ttu-id="fe749-113">Строка</span><span class="sxs-lookup"><span data-stu-id="fe749-113">String</span></span> | <span data-ttu-id="fe749-114">Запрос, указывающий, кто будет рецензентом.</span><span class="sxs-lookup"><span data-stu-id="fe749-114">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="fe749-115">Примеры приведены в таблице.</span><span class="sxs-lookup"><span data-stu-id="fe749-115">See table for examples.</span></span> |
| <span data-ttu-id="fe749-116">куеритипе</span><span class="sxs-lookup"><span data-stu-id="fe749-116">queryType</span></span> | <span data-ttu-id="fe749-117">Строка</span><span class="sxs-lookup"><span data-stu-id="fe749-117">String</span></span> | <span data-ttu-id="fe749-118">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="fe749-118">The type of query.</span></span> <span data-ttu-id="fe749-119">Примеры включают `MicrosoftGraph` и `ARM` .</span><span class="sxs-lookup"><span data-stu-id="fe749-119">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="fe749-120">куерирут</span><span class="sxs-lookup"><span data-stu-id="fe749-120">queryRoot</span></span> | <span data-ttu-id="fe749-121">Строка</span><span class="sxs-lookup"><span data-stu-id="fe749-121">String</span></span> | <span data-ttu-id="fe749-122">В сценарии, где Рецензенты должны быть указаны динамически, это свойство используется для указания относительного источника запроса.</span><span class="sxs-lookup"><span data-stu-id="fe749-122">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="fe749-123">Это свойство необходимо только в том случае, если указан относительный запрос (например,./Манажер).</span><span class="sxs-lookup"><span data-stu-id="fe749-123">This property is only required if a relative query (i.e., ./manager) is specified.</span></span> |

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="fe749-124">Поддерживаемые запросы для Акцессревиевревиеверскопе</span><span class="sxs-lookup"><span data-stu-id="fe749-124">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="fe749-125">Сценарий</span><span class="sxs-lookup"><span data-stu-id="fe749-125">Scenario</span></span>| <span data-ttu-id="fe749-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe749-126">query</span></span> | <span data-ttu-id="fe749-127">куеритипе</span><span class="sxs-lookup"><span data-stu-id="fe749-127">queryType</span></span> | <span data-ttu-id="fe749-128">куерирут</span><span class="sxs-lookup"><span data-stu-id="fe749-128">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="fe749-129">Владелец группы как проверяющий</span><span class="sxs-lookup"><span data-stu-id="fe749-129">Group owner as reviewer</span></span> | <span data-ttu-id="fe749-130">Идентификатор/граупс/{грауп}/овнерс</span><span class="sxs-lookup"><span data-stu-id="fe749-130">/groups/{group id}/owners</span></span> |<span data-ttu-id="fe749-131">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="fe749-131">MicrosoftGraph</span></span>||
| <span data-ttu-id="fe749-132">Определенный пользователь как проверяющий</span><span class="sxs-lookup"><span data-stu-id="fe749-132">Specific user as reviewer</span></span> | <span data-ttu-id="fe749-133">/усерс/{Усер ID}</span><span class="sxs-lookup"><span data-stu-id="fe749-133">/users/{user id}</span></span> |<span data-ttu-id="fe749-134">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="fe749-134">MicrosoftGraph</span></span>||
| <span data-ttu-id="fe749-135">Руководитель пользователя, который просматривается как проверяющий</span><span class="sxs-lookup"><span data-stu-id="fe749-135">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="fe749-136">./Манажер</span><span class="sxs-lookup"><span data-stu-id="fe749-136">./manager</span></span> | <span data-ttu-id="fe749-137">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="fe749-137">MicrosoftGraph</span></span> |<span data-ttu-id="fe749-138">решения</span><span class="sxs-lookup"><span data-stu-id="fe749-138">decisions</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe749-139">Связи</span><span class="sxs-lookup"><span data-stu-id="fe749-139">Relationships</span></span>
<span data-ttu-id="fe749-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fe749-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe749-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fe749-141">JSON representation</span></span>
<span data-ttu-id="fe749-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe749-142">The following is a JSON representation of the resource.</span></span>
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
