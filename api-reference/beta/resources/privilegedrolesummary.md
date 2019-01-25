---
title: Тип ресурса privilegedRoleSummary
description: Статистика для определенной роли.
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513741"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="05de8-103">Тип ресурса privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="05de8-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05de8-104">Статистика для определенной роли.</span><span class="sxs-lookup"><span data-stu-id="05de8-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="05de8-105">Методы</span><span class="sxs-lookup"><span data-stu-id="05de8-105">Methods</span></span>

| <span data-ttu-id="05de8-106">Метод</span><span class="sxs-lookup"><span data-stu-id="05de8-106">Method</span></span>           | <span data-ttu-id="05de8-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05de8-107">Return Type</span></span>    |<span data-ttu-id="05de8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="05de8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="05de8-109">Получение privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="05de8-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="05de8-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="05de8-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="05de8-111">Чтение свойства и связи объекта privilegedRoleSummary.</span><span class="sxs-lookup"><span data-stu-id="05de8-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="05de8-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="05de8-112">Properties</span></span>
| <span data-ttu-id="05de8-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="05de8-113">Property</span></span>     | <span data-ttu-id="05de8-114">Тип</span><span class="sxs-lookup"><span data-stu-id="05de8-114">Type</span></span>   |<span data-ttu-id="05de8-115">Описание</span><span class="sxs-lookup"><span data-stu-id="05de8-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05de8-116">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="05de8-116">elevatedCount</span></span>|<span data-ttu-id="05de8-117">int32</span><span class="sxs-lookup"><span data-stu-id="05de8-117">int32</span></span>|<span data-ttu-id="05de8-118">Число пользователей, имеющих роли, назначенной и роль активирован.</span><span class="sxs-lookup"><span data-stu-id="05de8-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="05de8-119">id</span><span class="sxs-lookup"><span data-stu-id="05de8-119">id</span></span>|<span data-ttu-id="05de8-120">string</span><span class="sxs-lookup"><span data-stu-id="05de8-120">string</span></span>| <span data-ttu-id="05de8-121">Уникальный идентификатор для роли.</span><span class="sxs-lookup"><span data-stu-id="05de8-121">The unique identifier for the role.</span></span> <span data-ttu-id="05de8-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="05de8-122">Read-only.</span></span>|
|<span data-ttu-id="05de8-123">managedCount</span><span class="sxs-lookup"><span data-stu-id="05de8-123">managedCount</span></span>|<span data-ttu-id="05de8-124">int32</span><span class="sxs-lookup"><span data-stu-id="05de8-124">int32</span></span>|<span data-ttu-id="05de8-125">Число пользователей, имеющих роли, назначенной, но роль отключена.</span><span class="sxs-lookup"><span data-stu-id="05de8-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="05de8-126">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="05de8-126">mfaEnabled</span></span>|<span data-ttu-id="05de8-127">boolean</span><span class="sxs-lookup"><span data-stu-id="05de8-127">boolean</span></span>|<span data-ttu-id="05de8-128">**значение true,** Если требуется для активации роли многофакторной проверкой Подлинности.</span><span class="sxs-lookup"><span data-stu-id="05de8-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="05de8-129">**значение false,** Если роль активации не требует многофакторной проверкой Подлинности.</span><span class="sxs-lookup"><span data-stu-id="05de8-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="05de8-130">status</span><span class="sxs-lookup"><span data-stu-id="05de8-130">status</span></span>|<span data-ttu-id="05de8-131">string</span><span class="sxs-lookup"><span data-stu-id="05de8-131">string</span></span>| <span data-ttu-id="05de8-132">Возможные значения: `ok`, `bad`.</span><span class="sxs-lookup"><span data-stu-id="05de8-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="05de8-133">Значение зависит от отношение числа (managedCount / usersCount).</span><span class="sxs-lookup"><span data-stu-id="05de8-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="05de8-134">Если отношение меньше, чем пороговых, `ok` возвращается.</span><span class="sxs-lookup"><span data-stu-id="05de8-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="05de8-135">В противном случае `bad` возвращается.</span><span class="sxs-lookup"><span data-stu-id="05de8-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="05de8-136">usersCount</span><span class="sxs-lookup"><span data-stu-id="05de8-136">usersCount</span></span>|<span data-ttu-id="05de8-137">int32</span><span class="sxs-lookup"><span data-stu-id="05de8-137">int32</span></span>|<span data-ttu-id="05de8-138">Число пользователей, которым назначен роли.</span><span class="sxs-lookup"><span data-stu-id="05de8-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05de8-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="05de8-139">Relationships</span></span>
<span data-ttu-id="05de8-140">Нет</span><span class="sxs-lookup"><span data-stu-id="05de8-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="05de8-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05de8-141">JSON representation</span></span>

<span data-ttu-id="05de8-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05de8-142">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesummary.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
