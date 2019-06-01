---
title: Тип ресурса Аппликатионсигниндетаиледсуммари — API Microsoft Graph
description: Представляет подробные сведения о входе в приложение.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4d4fcd00e305c19f1d445738a22125cc8addc143
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657639"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="356f0-103">Тип ресурса Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="356f0-103">applicationSignInDetailedSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="356f0-104">Представляет подробные сведения о входе в приложение.</span><span class="sxs-lookup"><span data-stu-id="356f0-104">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="356f0-105">Методы</span><span class="sxs-lookup"><span data-stu-id="356f0-105">Methods</span></span>

| <span data-ttu-id="356f0-106">Метод</span><span class="sxs-lookup"><span data-stu-id="356f0-106">Method</span></span>       | <span data-ttu-id="356f0-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="356f0-107">Return Type</span></span> | <span data-ttu-id="356f0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="356f0-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="356f0-109">Получение Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="356f0-109">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="356f0-110">Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="356f0-110">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="356f0-111">Чтение свойств и связей объекта **аппликатионсигниндетаиледсуммари** .</span><span class="sxs-lookup"><span data-stu-id="356f0-111">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="356f0-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="356f0-112">Properties</span></span>
| <span data-ttu-id="356f0-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="356f0-113">Property</span></span>     | <span data-ttu-id="356f0-114">Тип</span><span class="sxs-lookup"><span data-stu-id="356f0-114">Type</span></span>        | <span data-ttu-id="356f0-115">Описание</span><span class="sxs-lookup"><span data-stu-id="356f0-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="356f0-116">Аггрегатедевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="356f0-116">aggregatedEventDateTime</span></span>|<span data-ttu-id="356f0-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="356f0-117">DateTimeOffset</span></span>|<span data-ttu-id="356f0-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="356f0-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="356f0-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="356f0-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="356f0-120">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="356f0-120">appDisplayName</span></span>|<span data-ttu-id="356f0-121">String</span><span class="sxs-lookup"><span data-stu-id="356f0-121">String</span></span>|<span data-ttu-id="356f0-122">Имя приложения, в которое пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="356f0-122">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="356f0-123">appId</span><span class="sxs-lookup"><span data-stu-id="356f0-123">appId</span></span>|<span data-ttu-id="356f0-124">String</span><span class="sxs-lookup"><span data-stu-id="356f0-124">String</span></span>|<span data-ttu-id="356f0-125">Идентификатор приложения, в который пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="356f0-125">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="356f0-126">id</span><span class="sxs-lookup"><span data-stu-id="356f0-126">id</span></span>|<span data-ttu-id="356f0-127">Строка</span><span class="sxs-lookup"><span data-stu-id="356f0-127">String</span></span>| <span data-ttu-id="356f0-128">Уникальный идентификатор, представляющий действия при входе.</span><span class="sxs-lookup"><span data-stu-id="356f0-128">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="356f0-129">Сигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="356f0-129">signInCount</span></span>|<span data-ttu-id="356f0-130">Int64</span><span class="sxs-lookup"><span data-stu-id="356f0-130">Int64</span></span>|<span data-ttu-id="356f0-131">Количество входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="356f0-131">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="356f0-132">status</span><span class="sxs-lookup"><span data-stu-id="356f0-132">status</span></span>|[<span data-ttu-id="356f0-133">signInStatus</span><span class="sxs-lookup"><span data-stu-id="356f0-133">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="356f0-134">Сведения о состоянии входа.</span><span class="sxs-lookup"><span data-stu-id="356f0-134">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="356f0-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="356f0-135">Relationships</span></span>
<span data-ttu-id="356f0-136">Нет</span><span class="sxs-lookup"><span data-stu-id="356f0-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="356f0-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="356f0-137">JSON representation</span></span>

<span data-ttu-id="356f0-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="356f0-138">The following is a JSON representation of the resource.</span></span>

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
