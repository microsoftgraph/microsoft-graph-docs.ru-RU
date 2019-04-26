---
title: Тип ресурса Аппликатионсигниндетаиледсуммари — API Microsoft Graph
description: Представляет подробные сведения о входе в приложение.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 783201ec40ac0749d2c2999649bf1c420eaba5b6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328530"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="6851f-103">Тип ресурса Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="6851f-103">applicationSignInDetailedSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6851f-104">Представляет подробные сведения о входе в приложение.</span><span class="sxs-lookup"><span data-stu-id="6851f-104">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="6851f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6851f-105">Methods</span></span>

| <span data-ttu-id="6851f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6851f-106">Method</span></span>       | <span data-ttu-id="6851f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6851f-107">Return Type</span></span> | <span data-ttu-id="6851f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6851f-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6851f-109">Получение Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="6851f-109">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="6851f-110">Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="6851f-110">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="6851f-111">Чтение свойств и связей объекта **аппликатионсигниндетаиледсуммари** .</span><span class="sxs-lookup"><span data-stu-id="6851f-111">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6851f-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="6851f-112">Properties</span></span>
| <span data-ttu-id="6851f-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="6851f-113">Property</span></span>     | <span data-ttu-id="6851f-114">Тип</span><span class="sxs-lookup"><span data-stu-id="6851f-114">Type</span></span>        | <span data-ttu-id="6851f-115">Описание</span><span class="sxs-lookup"><span data-stu-id="6851f-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6851f-116">Аггрегатедевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="6851f-116">aggregatedEventDateTime</span></span>|<span data-ttu-id="6851f-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6851f-117">DateTimeOffset</span></span>|<span data-ttu-id="6851f-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6851f-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6851f-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6851f-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="6851f-120">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="6851f-120">appDisplayName</span></span>|<span data-ttu-id="6851f-121">String</span><span class="sxs-lookup"><span data-stu-id="6851f-121">String</span></span>|<span data-ttu-id="6851f-122">Имя приложения, в которое пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="6851f-122">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="6851f-123">appId</span><span class="sxs-lookup"><span data-stu-id="6851f-123">appId</span></span>|<span data-ttu-id="6851f-124">String</span><span class="sxs-lookup"><span data-stu-id="6851f-124">String</span></span>|<span data-ttu-id="6851f-125">Идентификатор приложения, в который пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="6851f-125">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="6851f-126">id</span><span class="sxs-lookup"><span data-stu-id="6851f-126">id</span></span>|<span data-ttu-id="6851f-127">Строка</span><span class="sxs-lookup"><span data-stu-id="6851f-127">String</span></span>| <span data-ttu-id="6851f-128">Уникальный идентификатор, представляющий действия при входе.</span><span class="sxs-lookup"><span data-stu-id="6851f-128">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="6851f-129">Сигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="6851f-129">signInCount</span></span>|<span data-ttu-id="6851f-130">Int64</span><span class="sxs-lookup"><span data-stu-id="6851f-130">Int64</span></span>|<span data-ttu-id="6851f-131">Количество входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="6851f-131">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="6851f-132">status</span><span class="sxs-lookup"><span data-stu-id="6851f-132">status</span></span>|[<span data-ttu-id="6851f-133">signInStatus</span><span class="sxs-lookup"><span data-stu-id="6851f-133">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="6851f-134">Сведения о состоянии входа.</span><span class="sxs-lookup"><span data-stu-id="6851f-134">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6851f-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="6851f-135">Relationships</span></span>
<span data-ttu-id="6851f-136">Нет</span><span class="sxs-lookup"><span data-stu-id="6851f-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6851f-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6851f-137">JSON representation</span></span>

<span data-ttu-id="6851f-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6851f-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
}-->

```json
{
  "aggregatedEventDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "appId": "String",
  "id": "String (identifier)",
  "signInCount": 1024,
  "status": {"@odata.type": "microsoft.graph.signInStatus"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
