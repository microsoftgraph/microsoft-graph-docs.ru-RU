---
title: Тип ресурса privilegedRoleSummary
description: Сводка статистики для определенной роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 368ed2ba6b206ba102f821ceac38de70494f8718
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133976"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="9e38f-103">Тип ресурса privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="9e38f-103">privilegedRoleSummary resource type</span></span>

<span data-ttu-id="9e38f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e38f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e38f-105">Сводка статистики для определенной роли.</span><span class="sxs-lookup"><span data-stu-id="9e38f-105">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="9e38f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9e38f-106">Methods</span></span>

| <span data-ttu-id="9e38f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9e38f-107">Method</span></span>           | <span data-ttu-id="9e38f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9e38f-108">Return Type</span></span>    |<span data-ttu-id="9e38f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9e38f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e38f-110">Получение privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="9e38f-110">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="9e38f-111">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="9e38f-111">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="9e38f-112">Чтение свойств и связей объекта privilegedRoleSummary.</span><span class="sxs-lookup"><span data-stu-id="9e38f-112">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e38f-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e38f-113">Properties</span></span>
| <span data-ttu-id="9e38f-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e38f-114">Property</span></span>     | <span data-ttu-id="9e38f-115">Тип</span><span class="sxs-lookup"><span data-stu-id="9e38f-115">Type</span></span>   |<span data-ttu-id="9e38f-116">Описание</span><span class="sxs-lookup"><span data-stu-id="9e38f-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e38f-117">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="9e38f-117">elevatedCount</span></span>|<span data-ttu-id="9e38f-118">int32</span><span class="sxs-lookup"><span data-stu-id="9e38f-118">int32</span></span>|<span data-ttu-id="9e38f-119">Количество пользователей, для пользователей с назначенной ролью и ролью активируется.</span><span class="sxs-lookup"><span data-stu-id="9e38f-119">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="9e38f-120">id</span><span class="sxs-lookup"><span data-stu-id="9e38f-120">id</span></span>|<span data-ttu-id="9e38f-121">string</span><span class="sxs-lookup"><span data-stu-id="9e38f-121">string</span></span>| <span data-ttu-id="9e38f-122">Уникальный идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="9e38f-122">The unique identifier for the role.</span></span> <span data-ttu-id="9e38f-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e38f-123">Read-only.</span></span>|
|<span data-ttu-id="9e38f-124">managedCount</span><span class="sxs-lookup"><span data-stu-id="9e38f-124">managedCount</span></span>|<span data-ttu-id="9e38f-125">int32</span><span class="sxs-lookup"><span data-stu-id="9e38f-125">int32</span></span>|<span data-ttu-id="9e38f-126">Количество пользователей с назначенной ролью, но отключаемой ролью.</span><span class="sxs-lookup"><span data-stu-id="9e38f-126">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="9e38f-127">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="9e38f-127">mfaEnabled</span></span>|<span data-ttu-id="9e38f-128">boolean</span><span class="sxs-lookup"><span data-stu-id="9e38f-128">boolean</span></span>|<span data-ttu-id="9e38f-129">**true,** если для активации роли требуется многофаксная активация.</span><span class="sxs-lookup"><span data-stu-id="9e38f-129">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="9e38f-130">**false,** если активация роли не требует многофаксической активации.</span><span class="sxs-lookup"><span data-stu-id="9e38f-130">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="9e38f-131">status</span><span class="sxs-lookup"><span data-stu-id="9e38f-131">status</span></span>|<span data-ttu-id="9e38f-132">string</span><span class="sxs-lookup"><span data-stu-id="9e38f-132">string</span></span>| <span data-ttu-id="9e38f-133">Возможные значения: `ok`, `bad`.</span><span class="sxs-lookup"><span data-stu-id="9e38f-133">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="9e38f-134">Значение зависит от соотношения (managedCount / usersCount).</span><span class="sxs-lookup"><span data-stu-id="9e38f-134">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="9e38f-135">Если коэффициент меньше предварительно заранее установленного порогового значения, `ok` возвращается.</span><span class="sxs-lookup"><span data-stu-id="9e38f-135">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="9e38f-136">В `bad` противном случае возвращается.</span><span class="sxs-lookup"><span data-stu-id="9e38f-136">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="9e38f-137">usersCount</span><span class="sxs-lookup"><span data-stu-id="9e38f-137">usersCount</span></span>|<span data-ttu-id="9e38f-138">int32</span><span class="sxs-lookup"><span data-stu-id="9e38f-138">int32</span></span>|<span data-ttu-id="9e38f-139">Количество пользователей, которые назначены этой роли.</span><span class="sxs-lookup"><span data-stu-id="9e38f-139">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e38f-140">Связи</span><span class="sxs-lookup"><span data-stu-id="9e38f-140">Relationships</span></span>
<span data-ttu-id="9e38f-141">Нет</span><span class="sxs-lookup"><span data-stu-id="9e38f-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9e38f-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e38f-142">JSON representation</span></span>

<span data-ttu-id="9e38f-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e38f-143">Here is a JSON representation of the resource.</span></span>

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


