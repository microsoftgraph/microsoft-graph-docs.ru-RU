---
title: тип ресурса teamsAppDefinition
description: Представляет сведения об одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8a43083e1f7fb717e2d54caef4017aeae97d9392
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625935"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="ceac4-103">тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ceac4-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="ceac4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceac4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ceac4-105">Представляет сведения о версии [teamsApp.](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="ceac4-105">Represents the details of a version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ceac4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ceac4-106">Properties</span></span>

| <span data-ttu-id="ceac4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ceac4-107">Property</span></span>            | <span data-ttu-id="ceac4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ceac4-108">Type</span></span>     | <span data-ttu-id="ceac4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ceac4-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ceac4-110">id</span><span class="sxs-lookup"><span data-stu-id="ceac4-110">id</span></span>                  | <span data-ttu-id="ceac4-111">string</span><span class="sxs-lookup"><span data-stu-id="ceac4-111">string</span></span>   | <span data-ttu-id="ceac4-112">Уникальный ID (а не ID приложения Teams).</span><span class="sxs-lookup"><span data-stu-id="ceac4-112">A unique ID (not the Teams app ID).</span></span> |
| <span data-ttu-id="ceac4-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="ceac4-113">teamsAppId</span></span>          | <span data-ttu-id="ceac4-114">Строка</span><span class="sxs-lookup"><span data-stu-id="ceac4-114">string</span></span>   | <span data-ttu-id="ceac4-115">ID из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="ceac4-115">The ID from the Teams app manifest.</span></span> |
| <span data-ttu-id="ceac4-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="ceac4-116">publishingState</span></span>| <span data-ttu-id="ceac4-117">Строка</span><span class="sxs-lookup"><span data-stu-id="ceac4-117">string</span></span>|<span data-ttu-id="ceac4-118">Опубликованный статус определенной версии приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="ceac4-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="ceac4-119">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="ceac4-119">Possible values are:</span></span></br><span data-ttu-id="ceac4-120">`submitted` — конкретная версия приложения Teams была представлена и находится на рассмотрении.</span><span class="sxs-lookup"><span data-stu-id="ceac4-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="ceac4-121">`published`  — Запрос на публикацию конкретной версии приложения Teams был утвержден администратором и приложение опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ceac4-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="ceac4-122">`rejected` — Запрос на публикацию конкретной версии приложения Teams был отклонен администратором.</span><span class="sxs-lookup"><span data-stu-id="ceac4-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="ceac4-123">displayName</span><span class="sxs-lookup"><span data-stu-id="ceac4-123">displayName</span></span>         | <span data-ttu-id="ceac4-124">string</span><span class="sxs-lookup"><span data-stu-id="ceac4-124">string</span></span>   | <span data-ttu-id="ceac4-125">Имя приложения, предоставленного разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="ceac4-125">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="ceac4-126">version</span><span class="sxs-lookup"><span data-stu-id="ceac4-126">version</span></span>             | <span data-ttu-id="ceac4-127">Строка</span><span class="sxs-lookup"><span data-stu-id="ceac4-127">string</span></span>   | <span data-ttu-id="ceac4-128">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="ceac4-128">The version number of the application.</span></span> |
| <span data-ttu-id="ceac4-129">shortDescription</span><span class="sxs-lookup"><span data-stu-id="ceac4-129">shortDescription</span></span>    | <span data-ttu-id="ceac4-130">Строка</span><span class="sxs-lookup"><span data-stu-id="ceac4-130">string</span></span>   | <span data-ttu-id="ceac4-131">Краткое описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ceac4-131">Short description of the application.</span></span> |
| <span data-ttu-id="ceac4-132">description</span><span class="sxs-lookup"><span data-stu-id="ceac4-132">description</span></span>         | <span data-ttu-id="ceac4-133">string</span><span class="sxs-lookup"><span data-stu-id="ceac4-133">string</span></span>   | <span data-ttu-id="ceac4-134">Подробное описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ceac4-134">Verbose description of the application.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ceac4-135">Связи</span><span class="sxs-lookup"><span data-stu-id="ceac4-135">Relationships</span></span>

| <span data-ttu-id="ceac4-136">Связь</span><span class="sxs-lookup"><span data-stu-id="ceac4-136">Relationship</span></span> | <span data-ttu-id="ceac4-137">Тип</span><span class="sxs-lookup"><span data-stu-id="ceac4-137">Type</span></span>   | <span data-ttu-id="ceac4-138">Описание</span><span class="sxs-lookup"><span data-stu-id="ceac4-138">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ceac4-139">бот</span><span class="sxs-lookup"><span data-stu-id="ceac4-139">bot</span></span>|[<span data-ttu-id="ceac4-140">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="ceac4-140">teamworkBot</span></span>](teamworkbot.md) | <span data-ttu-id="ceac4-141">Сведения о боте, указанном в манифесте приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="ceac4-141">The details of the bot specified in the Teams app manifest.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ceac4-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ceac4-142">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="ceac4-143">См. также</span><span class="sxs-lookup"><span data-stu-id="ceac4-143">See also</span></span>

- [<span data-ttu-id="ceac4-144">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ceac4-144">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="ceac4-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ceac4-145">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="ceac4-146">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ceac4-146">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

