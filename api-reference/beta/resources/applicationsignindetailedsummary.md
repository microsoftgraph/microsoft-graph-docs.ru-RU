---
title: Тип ресурса Аппликатионсигниндетаиледсуммари — API Microsoft Graph
description: Представляет подробные сведения о входе в приложение.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 527d60ff025e9a6d081226a51ec8cbefc53c20de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013336"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="713dc-103">Тип ресурса Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="713dc-103">applicationSignInDetailedSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="713dc-104">Представляет подробные сведения о входе в приложение.</span><span class="sxs-lookup"><span data-stu-id="713dc-104">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="713dc-105">Методы</span><span class="sxs-lookup"><span data-stu-id="713dc-105">Methods</span></span>

| <span data-ttu-id="713dc-106">Метод</span><span class="sxs-lookup"><span data-stu-id="713dc-106">Method</span></span>       | <span data-ttu-id="713dc-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="713dc-107">Return Type</span></span> | <span data-ttu-id="713dc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="713dc-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="713dc-109">Получение Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="713dc-109">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="713dc-110">Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="713dc-110">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="713dc-111">Чтение свойств и связей объекта **аппликатионсигниндетаиледсуммари** .</span><span class="sxs-lookup"><span data-stu-id="713dc-111">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="713dc-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="713dc-112">Properties</span></span>
| <span data-ttu-id="713dc-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="713dc-113">Property</span></span>     | <span data-ttu-id="713dc-114">Тип</span><span class="sxs-lookup"><span data-stu-id="713dc-114">Type</span></span>        | <span data-ttu-id="713dc-115">Описание</span><span class="sxs-lookup"><span data-stu-id="713dc-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="713dc-116">Аггрегатедевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="713dc-116">aggregatedEventDateTime</span></span>|<span data-ttu-id="713dc-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="713dc-117">DateTimeOffset</span></span>|<span data-ttu-id="713dc-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="713dc-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="713dc-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="713dc-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="713dc-120">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="713dc-120">appDisplayName</span></span>|<span data-ttu-id="713dc-121">String</span><span class="sxs-lookup"><span data-stu-id="713dc-121">String</span></span>|<span data-ttu-id="713dc-122">Имя приложения, в которое пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="713dc-122">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="713dc-123">appId</span><span class="sxs-lookup"><span data-stu-id="713dc-123">appId</span></span>|<span data-ttu-id="713dc-124">String</span><span class="sxs-lookup"><span data-stu-id="713dc-124">String</span></span>|<span data-ttu-id="713dc-125">Идентификатор приложения, в который пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="713dc-125">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="713dc-126">id</span><span class="sxs-lookup"><span data-stu-id="713dc-126">id</span></span>|<span data-ttu-id="713dc-127">Строка</span><span class="sxs-lookup"><span data-stu-id="713dc-127">String</span></span>| <span data-ttu-id="713dc-128">Уникальный идентификатор, представляющий действия при входе.</span><span class="sxs-lookup"><span data-stu-id="713dc-128">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="713dc-129">Сигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="713dc-129">signInCount</span></span>|<span data-ttu-id="713dc-130">Int64</span><span class="sxs-lookup"><span data-stu-id="713dc-130">Int64</span></span>|<span data-ttu-id="713dc-131">Количество входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="713dc-131">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="713dc-132">status</span><span class="sxs-lookup"><span data-stu-id="713dc-132">status</span></span>|[<span data-ttu-id="713dc-133">signInStatus</span><span class="sxs-lookup"><span data-stu-id="713dc-133">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="713dc-134">Сведения о состоянии входа.</span><span class="sxs-lookup"><span data-stu-id="713dc-134">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="713dc-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="713dc-135">Relationships</span></span>
<span data-ttu-id="713dc-136">Нет</span><span class="sxs-lookup"><span data-stu-id="713dc-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="713dc-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="713dc-137">JSON representation</span></span>

<span data-ttu-id="713dc-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="713dc-138">The following is a JSON representation of the resource.</span></span>

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
