---
title: Тип ресурса privilegedRoleSummary
description: Статистика для определенной роли.
localization_priority: Normal
ms.openlocfilehash: b74b562a992f7795f3ae8e317608f1e370bc2a4e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858620"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="07f3b-103">Тип ресурса privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="07f3b-103">privilegedRoleSummary resource type</span></span>

> <span data-ttu-id="07f3b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07f3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07f3b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07f3b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07f3b-106">Статистика для определенной роли.</span><span class="sxs-lookup"><span data-stu-id="07f3b-106">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="07f3b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="07f3b-107">Methods</span></span>

| <span data-ttu-id="07f3b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="07f3b-108">Method</span></span>           | <span data-ttu-id="07f3b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="07f3b-109">Return Type</span></span>    |<span data-ttu-id="07f3b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="07f3b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07f3b-111">Получение privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="07f3b-111">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="07f3b-112">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="07f3b-112">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="07f3b-113">Чтение свойства и связи объекта privilegedRoleSummary.</span><span class="sxs-lookup"><span data-stu-id="07f3b-113">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07f3b-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="07f3b-114">Properties</span></span>
| <span data-ttu-id="07f3b-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="07f3b-115">Property</span></span>     | <span data-ttu-id="07f3b-116">Тип</span><span class="sxs-lookup"><span data-stu-id="07f3b-116">Type</span></span>   |<span data-ttu-id="07f3b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="07f3b-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07f3b-118">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="07f3b-118">elevatedCount</span></span>|<span data-ttu-id="07f3b-119">int32</span><span class="sxs-lookup"><span data-stu-id="07f3b-119">int32</span></span>|<span data-ttu-id="07f3b-120">Число пользователей, имеющих роли, назначенной и роль активирован.</span><span class="sxs-lookup"><span data-stu-id="07f3b-120">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="07f3b-121">id</span><span class="sxs-lookup"><span data-stu-id="07f3b-121">id</span></span>|<span data-ttu-id="07f3b-122">строка</span><span class="sxs-lookup"><span data-stu-id="07f3b-122">string</span></span>| <span data-ttu-id="07f3b-123">Уникальный идентификатор для роли.</span><span class="sxs-lookup"><span data-stu-id="07f3b-123">The unique identifier for the role.</span></span> <span data-ttu-id="07f3b-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="07f3b-124">Read-only.</span></span>|
|<span data-ttu-id="07f3b-125">managedCount</span><span class="sxs-lookup"><span data-stu-id="07f3b-125">managedCount</span></span>|<span data-ttu-id="07f3b-126">int32</span><span class="sxs-lookup"><span data-stu-id="07f3b-126">int32</span></span>|<span data-ttu-id="07f3b-127">Число пользователей, имеющих роли, назначенной, но роль отключена.</span><span class="sxs-lookup"><span data-stu-id="07f3b-127">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="07f3b-128">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="07f3b-128">mfaEnabled</span></span>|<span data-ttu-id="07f3b-129">boolean</span><span class="sxs-lookup"><span data-stu-id="07f3b-129">boolean</span></span>|<span data-ttu-id="07f3b-130">**значение true,** Если требуется для активации роли многофакторной проверкой Подлинности.</span><span class="sxs-lookup"><span data-stu-id="07f3b-130">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="07f3b-131">**значение false,** Если роль активации не требует многофакторной проверкой Подлинности.</span><span class="sxs-lookup"><span data-stu-id="07f3b-131">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="07f3b-132">status</span><span class="sxs-lookup"><span data-stu-id="07f3b-132">status</span></span>|<span data-ttu-id="07f3b-133">string</span><span class="sxs-lookup"><span data-stu-id="07f3b-133">string</span></span>| <span data-ttu-id="07f3b-134">Возможные значения: `ok`, `bad`.</span><span class="sxs-lookup"><span data-stu-id="07f3b-134">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="07f3b-135">Значение зависит от отношение числа (managedCount / usersCount).</span><span class="sxs-lookup"><span data-stu-id="07f3b-135">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="07f3b-136">Если отношение меньше, чем пороговых, `ok` возвращается.</span><span class="sxs-lookup"><span data-stu-id="07f3b-136">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="07f3b-137">В противном случае `bad` возвращается.</span><span class="sxs-lookup"><span data-stu-id="07f3b-137">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="07f3b-138">usersCount</span><span class="sxs-lookup"><span data-stu-id="07f3b-138">usersCount</span></span>|<span data-ttu-id="07f3b-139">int32</span><span class="sxs-lookup"><span data-stu-id="07f3b-139">int32</span></span>|<span data-ttu-id="07f3b-140">Число пользователей, которым назначен роли.</span><span class="sxs-lookup"><span data-stu-id="07f3b-140">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07f3b-141">Связи</span><span class="sxs-lookup"><span data-stu-id="07f3b-141">Relationships</span></span>
<span data-ttu-id="07f3b-142">Нет</span><span class="sxs-lookup"><span data-stu-id="07f3b-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="07f3b-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07f3b-143">JSON representation</span></span>

<span data-ttu-id="07f3b-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07f3b-144">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
