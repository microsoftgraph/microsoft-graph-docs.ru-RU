---
title: тип ресурса privilegedRoleSummary
description: Сводка статистики для определенной роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 962cd1b830542c5b17c5f742af357d5855b81886
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962563"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="a3f8d-103">тип ресурса privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="a3f8d-103">privilegedRoleSummary resource type</span></span>

<span data-ttu-id="a3f8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3f8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3f8d-105">Сводка статистики для определенной роли.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-105">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="a3f8d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a3f8d-106">Methods</span></span>

| <span data-ttu-id="a3f8d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a3f8d-107">Method</span></span>           | <span data-ttu-id="a3f8d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3f8d-108">Return Type</span></span>    |<span data-ttu-id="a3f8d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a3f8d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3f8d-110">Получение privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="a3f8d-110">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="a3f8d-111">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="a3f8d-111">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="a3f8d-112">Чтение свойств и связей объекта privilegedRoleSummary.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-112">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3f8d-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3f8d-113">Properties</span></span>
| <span data-ttu-id="a3f8d-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3f8d-114">Property</span></span>     | <span data-ttu-id="a3f8d-115">Тип</span><span class="sxs-lookup"><span data-stu-id="a3f8d-115">Type</span></span>   |<span data-ttu-id="a3f8d-116">Описание</span><span class="sxs-lookup"><span data-stu-id="a3f8d-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3f8d-117">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="a3f8d-117">elevatedCount</span></span>|<span data-ttu-id="a3f8d-118">int32</span><span class="sxs-lookup"><span data-stu-id="a3f8d-118">int32</span></span>|<span data-ttu-id="a3f8d-119">Число пользователей, которые имеют назначенную роль и роль активируется.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-119">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="a3f8d-120">id</span><span class="sxs-lookup"><span data-stu-id="a3f8d-120">id</span></span>|<span data-ttu-id="a3f8d-121">string</span><span class="sxs-lookup"><span data-stu-id="a3f8d-121">string</span></span>| <span data-ttu-id="a3f8d-122">Уникальный идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-122">The unique identifier for the role.</span></span> <span data-ttu-id="a3f8d-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-123">Read-only.</span></span>|
|<span data-ttu-id="a3f8d-124">managedCount</span><span class="sxs-lookup"><span data-stu-id="a3f8d-124">managedCount</span></span>|<span data-ttu-id="a3f8d-125">int32</span><span class="sxs-lookup"><span data-stu-id="a3f8d-125">int32</span></span>|<span data-ttu-id="a3f8d-126">Число пользователей, которые имеют назначенную роль, но роль отключена.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-126">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="a3f8d-127">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="a3f8d-127">mfaEnabled</span></span>|<span data-ttu-id="a3f8d-128">boolean</span><span class="sxs-lookup"><span data-stu-id="a3f8d-128">boolean</span></span>|<span data-ttu-id="a3f8d-129">`true` если активация роли требует MFA.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-129">`true` if the role activation requires MFA.</span></span> <span data-ttu-id="a3f8d-130">`false` если активация роли не требует MFA.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-130">`false` if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="a3f8d-131">status</span><span class="sxs-lookup"><span data-stu-id="a3f8d-131">status</span></span>|<span data-ttu-id="a3f8d-132">roleSummaryStatus</span><span class="sxs-lookup"><span data-stu-id="a3f8d-132">roleSummaryStatus</span></span>| <span data-ttu-id="a3f8d-133">Возможные значения: `ok`, `bad`.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-133">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="a3f8d-134">Значение зависит от соотношения (managedCount /usersCount).</span><span class="sxs-lookup"><span data-stu-id="a3f8d-134">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="a3f8d-135">Если коэффициент меньше заранее установленного порогового значения, `ok` возвращается.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-135">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="a3f8d-136">В `bad` противном случае возвращается.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-136">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="a3f8d-137">usersCount</span><span class="sxs-lookup"><span data-stu-id="a3f8d-137">usersCount</span></span>|<span data-ttu-id="a3f8d-138">int32</span><span class="sxs-lookup"><span data-stu-id="a3f8d-138">int32</span></span>|<span data-ttu-id="a3f8d-139">Число пользователей, которые назначены с ролью.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-139">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3f8d-140">Связи</span><span class="sxs-lookup"><span data-stu-id="a3f8d-140">Relationships</span></span>
<span data-ttu-id="a3f8d-141">Нет</span><span class="sxs-lookup"><span data-stu-id="a3f8d-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a3f8d-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3f8d-142">JSON representation</span></span>

<span data-ttu-id="a3f8d-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3f8d-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


