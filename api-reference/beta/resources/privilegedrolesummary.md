---
title: Тип ресурса Привилежедролесуммари
description: Сводка статистики для определенной роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 2ce475e224e1de714ee033c5b50e831ff54e8e4c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807474"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="1ec73-103">Тип ресурса Привилежедролесуммари</span><span class="sxs-lookup"><span data-stu-id="1ec73-103">privilegedRoleSummary resource type</span></span>

<span data-ttu-id="1ec73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ec73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ec73-105">Сводка статистики для определенной роли.</span><span class="sxs-lookup"><span data-stu-id="1ec73-105">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="1ec73-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1ec73-106">Methods</span></span>

| <span data-ttu-id="1ec73-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1ec73-107">Method</span></span>           | <span data-ttu-id="1ec73-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1ec73-108">Return Type</span></span>    |<span data-ttu-id="1ec73-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1ec73-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ec73-110">Получение privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="1ec73-110">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="1ec73-111">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="1ec73-111">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="1ec73-112">Чтение свойств и связей объекта Привилежедролесуммари.</span><span class="sxs-lookup"><span data-stu-id="1ec73-112">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1ec73-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ec73-113">Properties</span></span>
| <span data-ttu-id="1ec73-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ec73-114">Property</span></span>     | <span data-ttu-id="1ec73-115">Тип</span><span class="sxs-lookup"><span data-stu-id="1ec73-115">Type</span></span>   |<span data-ttu-id="1ec73-116">Описание</span><span class="sxs-lookup"><span data-stu-id="1ec73-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ec73-117">елеватедкаунт</span><span class="sxs-lookup"><span data-stu-id="1ec73-117">elevatedCount</span></span>|<span data-ttu-id="1ec73-118">int32</span><span class="sxs-lookup"><span data-stu-id="1ec73-118">int32</span></span>|<span data-ttu-id="1ec73-119">Число пользователей с назначенной ролью и активацией роли.</span><span class="sxs-lookup"><span data-stu-id="1ec73-119">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="1ec73-120">id</span><span class="sxs-lookup"><span data-stu-id="1ec73-120">id</span></span>|<span data-ttu-id="1ec73-121">string</span><span class="sxs-lookup"><span data-stu-id="1ec73-121">string</span></span>| <span data-ttu-id="1ec73-122">Уникальный идентификатор для роли.</span><span class="sxs-lookup"><span data-stu-id="1ec73-122">The unique identifier for the role.</span></span> <span data-ttu-id="1ec73-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ec73-123">Read-only.</span></span>|
|<span data-ttu-id="1ec73-124">манажедкаунт</span><span class="sxs-lookup"><span data-stu-id="1ec73-124">managedCount</span></span>|<span data-ttu-id="1ec73-125">int32</span><span class="sxs-lookup"><span data-stu-id="1ec73-125">int32</span></span>|<span data-ttu-id="1ec73-126">Количество пользователей, которым назначена роль, но отключена роль.</span><span class="sxs-lookup"><span data-stu-id="1ec73-126">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="1ec73-127">мфаенаблед</span><span class="sxs-lookup"><span data-stu-id="1ec73-127">mfaEnabled</span></span>|<span data-ttu-id="1ec73-128">boolean</span><span class="sxs-lookup"><span data-stu-id="1ec73-128">boolean</span></span>|<span data-ttu-id="1ec73-129">**значение true** , если для активации роли требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="1ec73-129">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="1ec73-130">**false** , если для активации роли не требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="1ec73-130">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="1ec73-131">status</span><span class="sxs-lookup"><span data-stu-id="1ec73-131">status</span></span>|<span data-ttu-id="1ec73-132">string</span><span class="sxs-lookup"><span data-stu-id="1ec73-132">string</span></span>| <span data-ttu-id="1ec73-133">Возможные значения: `ok`, `bad`.</span><span class="sxs-lookup"><span data-stu-id="1ec73-133">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="1ec73-134">Значение зависит от коэффициента (Манажедкаунт/Усерскаунт).</span><span class="sxs-lookup"><span data-stu-id="1ec73-134">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="1ec73-135">Если отношение меньше заданного порогового значения, `ok` возвращается.</span><span class="sxs-lookup"><span data-stu-id="1ec73-135">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="1ec73-136">В противном случае `bad` возвращается.</span><span class="sxs-lookup"><span data-stu-id="1ec73-136">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="1ec73-137">усерскаунт</span><span class="sxs-lookup"><span data-stu-id="1ec73-137">usersCount</span></span>|<span data-ttu-id="1ec73-138">int32</span><span class="sxs-lookup"><span data-stu-id="1ec73-138">int32</span></span>|<span data-ttu-id="1ec73-139">Число пользователей, которым назначена роль.</span><span class="sxs-lookup"><span data-stu-id="1ec73-139">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ec73-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="1ec73-140">Relationships</span></span>
<span data-ttu-id="1ec73-141">Нет</span><span class="sxs-lookup"><span data-stu-id="1ec73-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1ec73-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ec73-142">JSON representation</span></span>

<span data-ttu-id="1ec73-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ec73-143">Here is a JSON representation of the resource.</span></span>

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
