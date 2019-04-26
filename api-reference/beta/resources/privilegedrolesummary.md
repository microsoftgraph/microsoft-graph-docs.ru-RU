---
title: Тип ресурса Привилежедролесуммари
description: Сводка статистики для определенной роли.
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563436"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="2f177-103">Тип ресурса Привилежедролесуммари</span><span class="sxs-lookup"><span data-stu-id="2f177-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f177-104">Сводка статистики для определенной роли.</span><span class="sxs-lookup"><span data-stu-id="2f177-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="2f177-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2f177-105">Methods</span></span>

| <span data-ttu-id="2f177-106">Метод</span><span class="sxs-lookup"><span data-stu-id="2f177-106">Method</span></span>           | <span data-ttu-id="2f177-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2f177-107">Return Type</span></span>    |<span data-ttu-id="2f177-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2f177-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f177-109">Получение privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="2f177-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="2f177-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="2f177-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="2f177-111">Чтение свойств и связей объекта Привилежедролесуммари.</span><span class="sxs-lookup"><span data-stu-id="2f177-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f177-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f177-112">Properties</span></span>
| <span data-ttu-id="2f177-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f177-113">Property</span></span>     | <span data-ttu-id="2f177-114">Тип</span><span class="sxs-lookup"><span data-stu-id="2f177-114">Type</span></span>   |<span data-ttu-id="2f177-115">Описание</span><span class="sxs-lookup"><span data-stu-id="2f177-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f177-116">Елеватедкаунт</span><span class="sxs-lookup"><span data-stu-id="2f177-116">elevatedCount</span></span>|<span data-ttu-id="2f177-117">Int32</span><span class="sxs-lookup"><span data-stu-id="2f177-117">int32</span></span>|<span data-ttu-id="2f177-118">Число пользователей с назначенной ролью и активацией роли.</span><span class="sxs-lookup"><span data-stu-id="2f177-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="2f177-119">id</span><span class="sxs-lookup"><span data-stu-id="2f177-119">id</span></span>|<span data-ttu-id="2f177-120">string</span><span class="sxs-lookup"><span data-stu-id="2f177-120">string</span></span>| <span data-ttu-id="2f177-121">Уникальный идентификатор для роли.</span><span class="sxs-lookup"><span data-stu-id="2f177-121">The unique identifier for the role.</span></span> <span data-ttu-id="2f177-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f177-122">Read-only.</span></span>|
|<span data-ttu-id="2f177-123">Манажедкаунт</span><span class="sxs-lookup"><span data-stu-id="2f177-123">managedCount</span></span>|<span data-ttu-id="2f177-124">Int32</span><span class="sxs-lookup"><span data-stu-id="2f177-124">int32</span></span>|<span data-ttu-id="2f177-125">Количество пользователей, которым назначена роль, но отключена роль.</span><span class="sxs-lookup"><span data-stu-id="2f177-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="2f177-126">Мфаенаблед</span><span class="sxs-lookup"><span data-stu-id="2f177-126">mfaEnabled</span></span>|<span data-ttu-id="2f177-127">boolean</span><span class="sxs-lookup"><span data-stu-id="2f177-127">boolean</span></span>|<span data-ttu-id="2f177-128">**значение true** , если для активации роли требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="2f177-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="2f177-129">**false** , если для активации роли не требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="2f177-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="2f177-130">status</span><span class="sxs-lookup"><span data-stu-id="2f177-130">status</span></span>|<span data-ttu-id="2f177-131">string</span><span class="sxs-lookup"><span data-stu-id="2f177-131">string</span></span>| <span data-ttu-id="2f177-132">Возможные значения: `ok`, `bad`.</span><span class="sxs-lookup"><span data-stu-id="2f177-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="2f177-133">Значение зависит от коэффициента (Манажедкаунт/Усерскаунт).</span><span class="sxs-lookup"><span data-stu-id="2f177-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="2f177-134">Если отношение меньше заданного порогового значения, `ok` возвращается.</span><span class="sxs-lookup"><span data-stu-id="2f177-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="2f177-135">`bad` В противном случае возвращается.</span><span class="sxs-lookup"><span data-stu-id="2f177-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="2f177-136">Усерскаунт</span><span class="sxs-lookup"><span data-stu-id="2f177-136">usersCount</span></span>|<span data-ttu-id="2f177-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2f177-137">int32</span></span>|<span data-ttu-id="2f177-138">Число пользователей, которым назначена роль.</span><span class="sxs-lookup"><span data-stu-id="2f177-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f177-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="2f177-139">Relationships</span></span>
<span data-ttu-id="2f177-140">Нет</span><span class="sxs-lookup"><span data-stu-id="2f177-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2f177-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f177-141">JSON representation</span></span>

<span data-ttu-id="2f177-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f177-142">Here is a JSON representation of the resource.</span></span>

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
