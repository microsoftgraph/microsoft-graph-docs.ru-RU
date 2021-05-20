---
title: тип ресурса accessReviewReviewerScope
description: Представляет, кто будет рассматривать обзор доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 58abda6c89e484336b34d546edc68ebbfe432162
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579263"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="831d5-103">тип ресурса accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="831d5-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="831d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="831d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="831d5-105">AccessReviewReviewerScope определяет, кто будет рассматривать экземпляры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="831d5-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="831d5-106">Это запрос OData, который позволяет рецензентам быть указанными как статический список пользователей (то есть конкретных пользователей, владельцев групп и членов группы) или динамически, в которых каждый пользователь просматривается их менеджером или владельцами групп.</span><span class="sxs-lookup"><span data-stu-id="831d5-106">It is an OData query that allows reviewers to be specified both as a static list of users (that is, specific users, group owners, and group members) or dynamically in which every user is reviewed by their manager or by group owners.</span></span> <span data-ttu-id="831d5-107">Чтобы создать самообзор (когда пользователи просматривают собственный доступ), не предоставлять рецензентов при создании [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="831d5-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>

<span data-ttu-id="831d5-108">Наследует [от accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="831d5-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="831d5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="831d5-109">Properties</span></span>
| <span data-ttu-id="831d5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="831d5-110">Property</span></span> | <span data-ttu-id="831d5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="831d5-111">Type</span></span> | <span data-ttu-id="831d5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="831d5-112">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="831d5-113">Запрос</span><span class="sxs-lookup"><span data-stu-id="831d5-113">query</span></span> | <span data-ttu-id="831d5-114">Строка</span><span class="sxs-lookup"><span data-stu-id="831d5-114">String</span></span> | <span data-ttu-id="831d5-115">Запрос, определяющий, кто будет рецензентом.</span><span class="sxs-lookup"><span data-stu-id="831d5-115">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="831d5-116">Примеры см. в таблице.</span><span class="sxs-lookup"><span data-stu-id="831d5-116">See table for examples.</span></span> |
| <span data-ttu-id="831d5-117">queryType</span><span class="sxs-lookup"><span data-stu-id="831d5-117">queryType</span></span> | <span data-ttu-id="831d5-118">Строка</span><span class="sxs-lookup"><span data-stu-id="831d5-118">String</span></span> | <span data-ttu-id="831d5-119">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="831d5-119">The type of query.</span></span> <span data-ttu-id="831d5-120">Примеры включают `MicrosoftGraph` и `ARM` .</span><span class="sxs-lookup"><span data-stu-id="831d5-120">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="831d5-121">queryRoot</span><span class="sxs-lookup"><span data-stu-id="831d5-121">queryRoot</span></span> | <span data-ttu-id="831d5-122">Строка</span><span class="sxs-lookup"><span data-stu-id="831d5-122">String</span></span> | <span data-ttu-id="831d5-123">В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса.</span><span class="sxs-lookup"><span data-stu-id="831d5-123">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="831d5-124">Это свойство требуется только в том случае, если указан относительный запрос, `./manager` например.</span><span class="sxs-lookup"><span data-stu-id="831d5-124">This property is only required if a relative query, for example, `./manager`, is specified.</span></span> <span data-ttu-id="831d5-125">Возможное значение: `decisions` .</span><span class="sxs-lookup"><span data-stu-id="831d5-125">Possible value: `decisions`.</span></span> |

<span data-ttu-id="831d5-126">Дополнительные возможности настройки для рецензентов см. в обзоре Назначение рецензентов определению обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-reviewers-concept)</span><span class="sxs-lookup"><span data-stu-id="831d5-126">For more about configuration options for **reviewers**, see [Assign reviewers to your access review definition using the Microsoft Graph API](/graph/accessreviews-reviewers-concept).</span></span>


## <a name="relationships"></a><span data-ttu-id="831d5-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="831d5-127">Relationships</span></span>
<span data-ttu-id="831d5-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="831d5-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="831d5-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="831d5-129">JSON representation</span></span>
<span data-ttu-id="831d5-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="831d5-130">The following is a JSON representation of the resource.</span></span>
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
