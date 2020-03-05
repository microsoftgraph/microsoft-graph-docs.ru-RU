---
title: Тип ресурса Аппликатионсигниндетаиледсуммари — API Microsoft Graph
description: Представляет подробные сведения о входе в приложение.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 118d26e6d46e5b64861a041eec12d03bea533552
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508277"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="cea2f-103">Тип ресурса Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="cea2f-103">applicationSignInDetailedSummary resource type</span></span>

<span data-ttu-id="cea2f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cea2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cea2f-105">Представляет подробные сведения о входе в приложение.</span><span class="sxs-lookup"><span data-stu-id="cea2f-105">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="cea2f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cea2f-106">Methods</span></span>

| <span data-ttu-id="cea2f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cea2f-107">Method</span></span>       | <span data-ttu-id="cea2f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cea2f-108">Return Type</span></span> | <span data-ttu-id="cea2f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cea2f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cea2f-110">Получение Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="cea2f-110">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="cea2f-111">аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="cea2f-111">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="cea2f-112">Чтение свойств и связей объекта **аппликатионсигниндетаиледсуммари** .</span><span class="sxs-lookup"><span data-stu-id="cea2f-112">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cea2f-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="cea2f-113">Properties</span></span>
| <span data-ttu-id="cea2f-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="cea2f-114">Property</span></span>     | <span data-ttu-id="cea2f-115">Тип</span><span class="sxs-lookup"><span data-stu-id="cea2f-115">Type</span></span>        | <span data-ttu-id="cea2f-116">Описание</span><span class="sxs-lookup"><span data-stu-id="cea2f-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cea2f-117">аггрегатедевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="cea2f-117">aggregatedEventDateTime</span></span>|<span data-ttu-id="cea2f-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cea2f-118">DateTimeOffset</span></span>|<span data-ttu-id="cea2f-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="cea2f-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cea2f-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cea2f-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="cea2f-121">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="cea2f-121">appDisplayName</span></span>|<span data-ttu-id="cea2f-122">String</span><span class="sxs-lookup"><span data-stu-id="cea2f-122">String</span></span>|<span data-ttu-id="cea2f-123">Имя приложения, в которое пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="cea2f-123">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="cea2f-124">appId</span><span class="sxs-lookup"><span data-stu-id="cea2f-124">appId</span></span>|<span data-ttu-id="cea2f-125">String</span><span class="sxs-lookup"><span data-stu-id="cea2f-125">String</span></span>|<span data-ttu-id="cea2f-126">Идентификатор приложения, в который пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="cea2f-126">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="cea2f-127">id</span><span class="sxs-lookup"><span data-stu-id="cea2f-127">id</span></span>|<span data-ttu-id="cea2f-128">Строка</span><span class="sxs-lookup"><span data-stu-id="cea2f-128">String</span></span>| <span data-ttu-id="cea2f-129">Уникальный идентификатор, представляющий действия при входе.</span><span class="sxs-lookup"><span data-stu-id="cea2f-129">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="cea2f-130">сигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="cea2f-130">signInCount</span></span>|<span data-ttu-id="cea2f-131">Int64</span><span class="sxs-lookup"><span data-stu-id="cea2f-131">Int64</span></span>|<span data-ttu-id="cea2f-132">Количество входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="cea2f-132">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="cea2f-133">status</span><span class="sxs-lookup"><span data-stu-id="cea2f-133">status</span></span>|[<span data-ttu-id="cea2f-134">signInStatus</span><span class="sxs-lookup"><span data-stu-id="cea2f-134">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="cea2f-135">Сведения о состоянии входа.</span><span class="sxs-lookup"><span data-stu-id="cea2f-135">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cea2f-136">Связи</span><span class="sxs-lookup"><span data-stu-id="cea2f-136">Relationships</span></span>
<span data-ttu-id="cea2f-137">Нет</span><span class="sxs-lookup"><span data-stu-id="cea2f-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cea2f-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cea2f-138">JSON representation</span></span>

<span data-ttu-id="cea2f-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cea2f-139">The following is a JSON representation of the resource.</span></span>

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
