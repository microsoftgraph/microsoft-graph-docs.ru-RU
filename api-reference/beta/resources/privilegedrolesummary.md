---
title: Тип ресурса Привилежедролесуммари
description: Сводка статистики для определенной роли.
localization_priority: Normal
ms.openlocfilehash: 3e7b447f63c5f8545021508ae2dc137bef845210
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344290"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="ef63b-103">Тип ресурса Привилежедролесуммари</span><span class="sxs-lookup"><span data-stu-id="ef63b-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef63b-104">Сводка статистики для определенной роли.</span><span class="sxs-lookup"><span data-stu-id="ef63b-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="ef63b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ef63b-105">Methods</span></span>

| <span data-ttu-id="ef63b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ef63b-106">Method</span></span>           | <span data-ttu-id="ef63b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ef63b-107">Return Type</span></span>    |<span data-ttu-id="ef63b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ef63b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef63b-109">Получение privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="ef63b-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="ef63b-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="ef63b-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="ef63b-111">Чтение свойств и связей объекта Привилежедролесуммари.</span><span class="sxs-lookup"><span data-stu-id="ef63b-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ef63b-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef63b-112">Properties</span></span>
| <span data-ttu-id="ef63b-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef63b-113">Property</span></span>     | <span data-ttu-id="ef63b-114">Тип</span><span class="sxs-lookup"><span data-stu-id="ef63b-114">Type</span></span>   |<span data-ttu-id="ef63b-115">Описание</span><span class="sxs-lookup"><span data-stu-id="ef63b-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef63b-116">Елеватедкаунт</span><span class="sxs-lookup"><span data-stu-id="ef63b-116">elevatedCount</span></span>|<span data-ttu-id="ef63b-117">int32</span><span class="sxs-lookup"><span data-stu-id="ef63b-117">int32</span></span>|<span data-ttu-id="ef63b-118">Число пользователей с назначенной ролью и активацией роли.</span><span class="sxs-lookup"><span data-stu-id="ef63b-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="ef63b-119">id</span><span class="sxs-lookup"><span data-stu-id="ef63b-119">id</span></span>|<span data-ttu-id="ef63b-120">строка</span><span class="sxs-lookup"><span data-stu-id="ef63b-120">string</span></span>| <span data-ttu-id="ef63b-121">Уникальный идентификатор для роли.</span><span class="sxs-lookup"><span data-stu-id="ef63b-121">The unique identifier for the role.</span></span> <span data-ttu-id="ef63b-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef63b-122">Read-only.</span></span>|
|<span data-ttu-id="ef63b-123">Манажедкаунт</span><span class="sxs-lookup"><span data-stu-id="ef63b-123">managedCount</span></span>|<span data-ttu-id="ef63b-124">int32</span><span class="sxs-lookup"><span data-stu-id="ef63b-124">int32</span></span>|<span data-ttu-id="ef63b-125">Количество пользователей, которым назначена роль, но отключена роль.</span><span class="sxs-lookup"><span data-stu-id="ef63b-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="ef63b-126">Мфаенаблед</span><span class="sxs-lookup"><span data-stu-id="ef63b-126">mfaEnabled</span></span>|<span data-ttu-id="ef63b-127">boolean</span><span class="sxs-lookup"><span data-stu-id="ef63b-127">boolean</span></span>|<span data-ttu-id="ef63b-128">**значение true** , если для активации роли требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="ef63b-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="ef63b-129">**false** , если для активации роли не требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="ef63b-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="ef63b-130">status</span><span class="sxs-lookup"><span data-stu-id="ef63b-130">status</span></span>|<span data-ttu-id="ef63b-131">string</span><span class="sxs-lookup"><span data-stu-id="ef63b-131">string</span></span>| <span data-ttu-id="ef63b-132">Возможные значения: `ok`, `bad`.</span><span class="sxs-lookup"><span data-stu-id="ef63b-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="ef63b-133">Значение зависит от коэффициента (Манажедкаунт/Усерскаунт).</span><span class="sxs-lookup"><span data-stu-id="ef63b-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="ef63b-134">Если отношение меньше заданного порогового значения, `ok` возвращается.</span><span class="sxs-lookup"><span data-stu-id="ef63b-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="ef63b-135">`bad` В противном случае возвращается.</span><span class="sxs-lookup"><span data-stu-id="ef63b-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="ef63b-136">Усерскаунт</span><span class="sxs-lookup"><span data-stu-id="ef63b-136">usersCount</span></span>|<span data-ttu-id="ef63b-137">int32</span><span class="sxs-lookup"><span data-stu-id="ef63b-137">int32</span></span>|<span data-ttu-id="ef63b-138">Число пользователей, которым назначена роль.</span><span class="sxs-lookup"><span data-stu-id="ef63b-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef63b-139">Связи</span><span class="sxs-lookup"><span data-stu-id="ef63b-139">Relationships</span></span>
<span data-ttu-id="ef63b-140">Нет</span><span class="sxs-lookup"><span data-stu-id="ef63b-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ef63b-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef63b-141">JSON representation</span></span>

<span data-ttu-id="ef63b-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef63b-142">Here is a JSON representation of the resource.</span></span>

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
