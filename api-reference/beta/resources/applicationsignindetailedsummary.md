---
title: Тип ресурса Аппликатионсигниндетаиледсуммари — API Microsoft Graph
description: Представляет подробные сведения о входе в приложение.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 754a7f69b4f38fa101fe2fe5c349e089ae25c457
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455285"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="f7479-103">Тип ресурса Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="f7479-103">applicationSignInDetailedSummary resource type</span></span>

<span data-ttu-id="f7479-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7479-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7479-105">Представляет подробные сведения о входе в приложение.</span><span class="sxs-lookup"><span data-stu-id="f7479-105">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="f7479-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f7479-106">Methods</span></span>

| <span data-ttu-id="f7479-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f7479-107">Method</span></span>       | <span data-ttu-id="f7479-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f7479-108">Return Type</span></span> | <span data-ttu-id="f7479-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f7479-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f7479-110">Получение Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="f7479-110">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="f7479-111">аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="f7479-111">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="f7479-112">Чтение свойств и связей объекта **аппликатионсигниндетаиледсуммари** .</span><span class="sxs-lookup"><span data-stu-id="f7479-112">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f7479-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7479-113">Properties</span></span>
| <span data-ttu-id="f7479-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7479-114">Property</span></span>     | <span data-ttu-id="f7479-115">Тип</span><span class="sxs-lookup"><span data-stu-id="f7479-115">Type</span></span>        | <span data-ttu-id="f7479-116">Описание</span><span class="sxs-lookup"><span data-stu-id="f7479-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7479-117">аггрегатедевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="f7479-117">aggregatedEventDateTime</span></span>|<span data-ttu-id="f7479-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7479-118">DateTimeOffset</span></span>|<span data-ttu-id="f7479-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f7479-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f7479-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f7479-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f7479-121">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="f7479-121">appDisplayName</span></span>|<span data-ttu-id="f7479-122">String</span><span class="sxs-lookup"><span data-stu-id="f7479-122">String</span></span>|<span data-ttu-id="f7479-123">Имя приложения, в которое пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="f7479-123">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="f7479-124">appId</span><span class="sxs-lookup"><span data-stu-id="f7479-124">appId</span></span>|<span data-ttu-id="f7479-125">String</span><span class="sxs-lookup"><span data-stu-id="f7479-125">String</span></span>|<span data-ttu-id="f7479-126">Идентификатор приложения, в который пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="f7479-126">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="f7479-127">id</span><span class="sxs-lookup"><span data-stu-id="f7479-127">id</span></span>|<span data-ttu-id="f7479-128">Строка</span><span class="sxs-lookup"><span data-stu-id="f7479-128">String</span></span>| <span data-ttu-id="f7479-129">Уникальный идентификатор, представляющий действия при входе.</span><span class="sxs-lookup"><span data-stu-id="f7479-129">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="f7479-130">сигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="f7479-130">signInCount</span></span>|<span data-ttu-id="f7479-131">Int64</span><span class="sxs-lookup"><span data-stu-id="f7479-131">Int64</span></span>|<span data-ttu-id="f7479-132">Количество входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="f7479-132">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="f7479-133">status</span><span class="sxs-lookup"><span data-stu-id="f7479-133">status</span></span>|[<span data-ttu-id="f7479-134">signInStatus</span><span class="sxs-lookup"><span data-stu-id="f7479-134">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="f7479-135">Сведения о состоянии входа.</span><span class="sxs-lookup"><span data-stu-id="f7479-135">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7479-136">Связи</span><span class="sxs-lookup"><span data-stu-id="f7479-136">Relationships</span></span>
<span data-ttu-id="f7479-137">Нет</span><span class="sxs-lookup"><span data-stu-id="f7479-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f7479-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7479-138">JSON representation</span></span>

<span data-ttu-id="f7479-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7479-139">The following is a JSON representation of the resource.</span></span>

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
