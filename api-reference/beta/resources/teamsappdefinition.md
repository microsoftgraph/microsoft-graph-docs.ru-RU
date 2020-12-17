---
title: Тип ресурса teamsAppDefinition
description: Сведения об одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6b5fd771d1fb38de5354c74778f5eae798ccc91e
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706117"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="9cdf2-103">Тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="9cdf2-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="9cdf2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cdf2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cdf2-105">Сведения о версии [teamsApp.](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="9cdf2-105">The details of a version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9cdf2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9cdf2-106">Properties</span></span>

| <span data-ttu-id="9cdf2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cdf2-107">Property</span></span>            | <span data-ttu-id="9cdf2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9cdf2-108">Type</span></span>     | <span data-ttu-id="9cdf2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9cdf2-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="9cdf2-110">id</span><span class="sxs-lookup"><span data-stu-id="9cdf2-110">id</span></span>                  | <span data-ttu-id="9cdf2-111">string</span><span class="sxs-lookup"><span data-stu-id="9cdf2-111">string</span></span>   | <span data-ttu-id="9cdf2-112">Уникальный ид (не appid teams).</span><span class="sxs-lookup"><span data-stu-id="9cdf2-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="9cdf2-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="9cdf2-113">teamsAppId</span></span>          | <span data-ttu-id="9cdf2-114">string</span><span class="sxs-lookup"><span data-stu-id="9cdf2-114">string</span></span>   | <span data-ttu-id="9cdf2-115">ИД из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="9cdf2-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="9cdf2-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="9cdf2-116">publishingState</span></span>| <span data-ttu-id="9cdf2-117">string</span><span class="sxs-lookup"><span data-stu-id="9cdf2-117">string</span></span>|<span data-ttu-id="9cdf2-118">Состояние публикации определенной версии приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="9cdf2-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="9cdf2-119">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="9cdf2-119">Possible values are:</span></span></br><span data-ttu-id="9cdf2-120">`submitted` — конкретная версия приложения Teams была отправлена и находится на рассмотрении.</span><span class="sxs-lookup"><span data-stu-id="9cdf2-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="9cdf2-121">`published`  — запрос на публикацию определенной версии приложения Teams утвержден администратором, и приложение опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9cdf2-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="9cdf2-122">`rejected` — запрос на публикацию определенной версии приложения Teams был отклонен администратором.</span><span class="sxs-lookup"><span data-stu-id="9cdf2-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="9cdf2-123">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="9cdf2-123">azureADAppId</span></span>        | <span data-ttu-id="9cdf2-124">string</span><span class="sxs-lookup"><span data-stu-id="9cdf2-124">string</span></span>   | <span data-ttu-id="9cdf2-125">WebApplicationInfo.id из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="9cdf2-125">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="9cdf2-126">displayName</span><span class="sxs-lookup"><span data-stu-id="9cdf2-126">displayName</span></span>         | <span data-ttu-id="9cdf2-127">string</span><span class="sxs-lookup"><span data-stu-id="9cdf2-127">string</span></span>   | <span data-ttu-id="9cdf2-128">Имя приложения, предоставленное разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="9cdf2-128">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="9cdf2-129">version</span><span class="sxs-lookup"><span data-stu-id="9cdf2-129">version</span></span>             | <span data-ttu-id="9cdf2-130">string</span><span class="sxs-lookup"><span data-stu-id="9cdf2-130">string</span></span>   | <span data-ttu-id="9cdf2-131">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="9cdf2-131">The version number of the application.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9cdf2-132">Связи</span><span class="sxs-lookup"><span data-stu-id="9cdf2-132">Relationships</span></span>

| <span data-ttu-id="9cdf2-133">Связь</span><span class="sxs-lookup"><span data-stu-id="9cdf2-133">Relationship</span></span> | <span data-ttu-id="9cdf2-134">Тип</span><span class="sxs-lookup"><span data-stu-id="9cdf2-134">Type</span></span>   | <span data-ttu-id="9cdf2-135">Описание</span><span class="sxs-lookup"><span data-stu-id="9cdf2-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9cdf2-136">bot</span><span class="sxs-lookup"><span data-stu-id="9cdf2-136">bot</span></span>|[<span data-ttu-id="9cdf2-137">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="9cdf2-137">teamworkBot</span></span>](teamworkbot.md) | <span data-ttu-id="9cdf2-138">Сведения о боте, указанном в манифесте приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="9cdf2-138">The details of the bot specified in the Teams App manifest.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9cdf2-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9cdf2-139">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0"
}
```

## <a name="see-also"></a><span data-ttu-id="9cdf2-140">См. также</span><span class="sxs-lookup"><span data-stu-id="9cdf2-140">See also</span></span>

- [<span data-ttu-id="9cdf2-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9cdf2-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="9cdf2-142">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="9cdf2-142">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="9cdf2-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9cdf2-143">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


