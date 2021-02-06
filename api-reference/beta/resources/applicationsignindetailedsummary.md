---
title: Тип ресурса applicationSignInDetailedSummary — API Microsoft Graph
description: Представляет подробную сводку по входу в приложение.
localization_priority: Normal
author: sureshja
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d0d1eaa15d71dfa219271cef74880a092e9522db
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137454"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="f31ab-103">Тип ресурса applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="f31ab-103">applicationSignInDetailedSummary resource type</span></span>

<span data-ttu-id="f31ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f31ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f31ab-105">Представляет подробную сводку по входу в приложение.</span><span class="sxs-lookup"><span data-stu-id="f31ab-105">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="f31ab-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f31ab-106">Methods</span></span>

| <span data-ttu-id="f31ab-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f31ab-107">Method</span></span>       | <span data-ttu-id="f31ab-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f31ab-108">Return Type</span></span> | <span data-ttu-id="f31ab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f31ab-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f31ab-110">Получение applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="f31ab-110">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="f31ab-111">applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="f31ab-111">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="f31ab-112">Чтение свойств и связей объекта **applicationSignInDetailedSummary.**</span><span class="sxs-lookup"><span data-stu-id="f31ab-112">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f31ab-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="f31ab-113">Properties</span></span>
| <span data-ttu-id="f31ab-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="f31ab-114">Property</span></span>     | <span data-ttu-id="f31ab-115">Тип</span><span class="sxs-lookup"><span data-stu-id="f31ab-115">Type</span></span>        | <span data-ttu-id="f31ab-116">Описание</span><span class="sxs-lookup"><span data-stu-id="f31ab-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f31ab-117">aggregatedEventDateTime</span><span class="sxs-lookup"><span data-stu-id="f31ab-117">aggregatedEventDateTime</span></span>|<span data-ttu-id="f31ab-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f31ab-118">DateTimeOffset</span></span>|<span data-ttu-id="f31ab-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f31ab-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f31ab-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f31ab-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f31ab-121">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="f31ab-121">appDisplayName</span></span>|<span data-ttu-id="f31ab-122">String</span><span class="sxs-lookup"><span data-stu-id="f31ab-122">String</span></span>|<span data-ttu-id="f31ab-123">Имя приложения, в которое вписались пользователи.</span><span class="sxs-lookup"><span data-stu-id="f31ab-123">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="f31ab-124">appId</span><span class="sxs-lookup"><span data-stu-id="f31ab-124">appId</span></span>|<span data-ttu-id="f31ab-125">String</span><span class="sxs-lookup"><span data-stu-id="f31ab-125">String</span></span>|<span data-ttu-id="f31ab-126">ИД приложения, в которое вписался пользователь.</span><span class="sxs-lookup"><span data-stu-id="f31ab-126">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="f31ab-127">id</span><span class="sxs-lookup"><span data-stu-id="f31ab-127">id</span></span>|<span data-ttu-id="f31ab-128">Строка</span><span class="sxs-lookup"><span data-stu-id="f31ab-128">String</span></span>| <span data-ttu-id="f31ab-129">Уникальный ИД, представляющий действие при входе.</span><span class="sxs-lookup"><span data-stu-id="f31ab-129">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="f31ab-130">signInCount</span><span class="sxs-lookup"><span data-stu-id="f31ab-130">signInCount</span></span>|<span data-ttu-id="f31ab-131">Int64</span><span class="sxs-lookup"><span data-stu-id="f31ab-131">Int64</span></span>|<span data-ttu-id="f31ab-132">Количество входов, сделанных приложением.</span><span class="sxs-lookup"><span data-stu-id="f31ab-132">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="f31ab-133">status</span><span class="sxs-lookup"><span data-stu-id="f31ab-133">status</span></span>|[<span data-ttu-id="f31ab-134">signInStatus</span><span class="sxs-lookup"><span data-stu-id="f31ab-134">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="f31ab-135">Сведения о состоянии регистрации.</span><span class="sxs-lookup"><span data-stu-id="f31ab-135">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f31ab-136">Связи</span><span class="sxs-lookup"><span data-stu-id="f31ab-136">Relationships</span></span>
<span data-ttu-id="f31ab-137">Нет</span><span class="sxs-lookup"><span data-stu-id="f31ab-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f31ab-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f31ab-138">JSON representation</span></span>

<span data-ttu-id="f31ab-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f31ab-139">The following is a JSON representation of the resource.</span></span>

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


