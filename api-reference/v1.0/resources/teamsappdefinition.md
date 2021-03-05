---
title: тип ресурса teamsAppDefinition
description: Представляет сведения об одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b247432171f5de9d2624d7793f25ab6bfdce91fe
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470671"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="7f9a0-103">тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="7f9a0-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="7f9a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f9a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7f9a0-105">Представляет сведения об одной версии [teamsApp.](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f9a0-105">Represents the details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7f9a0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f9a0-106">Properties</span></span>

| <span data-ttu-id="7f9a0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f9a0-107">Property</span></span>            | <span data-ttu-id="7f9a0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7f9a0-108">Type</span></span>     | <span data-ttu-id="7f9a0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7f9a0-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="7f9a0-110">id</span><span class="sxs-lookup"><span data-stu-id="7f9a0-110">id</span></span>                  | <span data-ttu-id="7f9a0-111">string</span><span class="sxs-lookup"><span data-stu-id="7f9a0-111">string</span></span>   | <span data-ttu-id="7f9a0-112">Уникальный ID (а не ID приложения Teams).</span><span class="sxs-lookup"><span data-stu-id="7f9a0-112">A unique ID (not the Teams app ID).</span></span> |
| <span data-ttu-id="7f9a0-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="7f9a0-113">teamsAppId</span></span>          | <span data-ttu-id="7f9a0-114">string</span><span class="sxs-lookup"><span data-stu-id="7f9a0-114">string</span></span>   | <span data-ttu-id="7f9a0-115">ID из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="7f9a0-115">The ID from the Teams app manifest.</span></span> |
| <span data-ttu-id="7f9a0-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="7f9a0-116">publishingState</span></span>| <span data-ttu-id="7f9a0-117">string</span><span class="sxs-lookup"><span data-stu-id="7f9a0-117">string</span></span>|<span data-ttu-id="7f9a0-118">Опубликованный статус определенной версии приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="7f9a0-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="7f9a0-119">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="7f9a0-119">Possible values are:</span></span></br><span data-ttu-id="7f9a0-120">`submitted` — конкретная версия приложения Teams была представлена и находится на рассмотрении.</span><span class="sxs-lookup"><span data-stu-id="7f9a0-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="7f9a0-121">`published`  — Запрос на публикацию конкретной версии приложения Teams был утвержден администратором и приложение опубликовано.</span><span class="sxs-lookup"><span data-stu-id="7f9a0-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="7f9a0-122">`rejected` — Запрос на публикацию конкретной версии приложения Teams был отклонен администратором.</span><span class="sxs-lookup"><span data-stu-id="7f9a0-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="7f9a0-123">displayName</span><span class="sxs-lookup"><span data-stu-id="7f9a0-123">displayName</span></span>         | <span data-ttu-id="7f9a0-124">string</span><span class="sxs-lookup"><span data-stu-id="7f9a0-124">string</span></span>   | <span data-ttu-id="7f9a0-125">Имя приложения, предоставленного разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="7f9a0-125">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="7f9a0-126">version</span><span class="sxs-lookup"><span data-stu-id="7f9a0-126">version</span></span>             | <span data-ttu-id="7f9a0-127">string</span><span class="sxs-lookup"><span data-stu-id="7f9a0-127">string</span></span>   | <span data-ttu-id="7f9a0-128">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="7f9a0-128">The version number of the application.</span></span> |
| <span data-ttu-id="7f9a0-129">shortDescription</span><span class="sxs-lookup"><span data-stu-id="7f9a0-129">shortDescription</span></span>    | <span data-ttu-id="7f9a0-130">string</span><span class="sxs-lookup"><span data-stu-id="7f9a0-130">string</span></span>   | <span data-ttu-id="7f9a0-131">Краткое описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7f9a0-131">Short description of the application.</span></span> |
| <span data-ttu-id="7f9a0-132">description</span><span class="sxs-lookup"><span data-stu-id="7f9a0-132">description</span></span>         | <span data-ttu-id="7f9a0-133">string</span><span class="sxs-lookup"><span data-stu-id="7f9a0-133">string</span></span>   | <span data-ttu-id="7f9a0-134">Подробное описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7f9a0-134">Verbose description of the application.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7f9a0-135">Связи</span><span class="sxs-lookup"><span data-stu-id="7f9a0-135">Relationships</span></span>

| <span data-ttu-id="7f9a0-136">Связь</span><span class="sxs-lookup"><span data-stu-id="7f9a0-136">Relationship</span></span> | <span data-ttu-id="7f9a0-137">Тип</span><span class="sxs-lookup"><span data-stu-id="7f9a0-137">Type</span></span>   | <span data-ttu-id="7f9a0-138">Описание</span><span class="sxs-lookup"><span data-stu-id="7f9a0-138">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7f9a0-139">бот</span><span class="sxs-lookup"><span data-stu-id="7f9a0-139">bot</span></span>|[<span data-ttu-id="7f9a0-140">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="7f9a0-140">teamworkBot</span></span>](teamworkbot.md) | <span data-ttu-id="7f9a0-141">Сведения о боте, указанном в манифесте приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="7f9a0-141">The details of the bot specified in the Teams app manifest.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7f9a0-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7f9a0-142">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7f9a0-143">См. также</span><span class="sxs-lookup"><span data-stu-id="7f9a0-143">See also</span></span>

- [<span data-ttu-id="7f9a0-144">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7f9a0-144">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="7f9a0-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7f9a0-145">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="7f9a0-146">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7f9a0-146">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

