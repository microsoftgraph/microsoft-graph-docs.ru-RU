---
title: тип ресурса teamsAppDefinition
description: Сведения об одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 205c656e81ed9dfc75e97cbe0734eeb36c5c0127
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638909"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="1b5fc-103">тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1b5fc-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="1b5fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b5fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b5fc-105">Сведения о версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b5fc-105">The details of a version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1b5fc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b5fc-106">Properties</span></span>

| <span data-ttu-id="1b5fc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b5fc-107">Property</span></span>            | <span data-ttu-id="1b5fc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1b5fc-108">Type</span></span>     | <span data-ttu-id="1b5fc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1b5fc-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1b5fc-110">id</span><span class="sxs-lookup"><span data-stu-id="1b5fc-110">id</span></span>                  | <span data-ttu-id="1b5fc-111">string</span><span class="sxs-lookup"><span data-stu-id="1b5fc-111">string</span></span>   | <span data-ttu-id="1b5fc-112">Уникальный id (а не командный appid).</span><span class="sxs-lookup"><span data-stu-id="1b5fc-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="1b5fc-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="1b5fc-113">teamsAppId</span></span>          | <span data-ttu-id="1b5fc-114">Строка</span><span class="sxs-lookup"><span data-stu-id="1b5fc-114">string</span></span>   | <span data-ttu-id="1b5fc-115">Id из манифеста Teams App.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="1b5fc-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="1b5fc-116">publishingState</span></span>| <span data-ttu-id="1b5fc-117">Строка</span><span class="sxs-lookup"><span data-stu-id="1b5fc-117">string</span></span>|<span data-ttu-id="1b5fc-118">Опубликованный статус определенной версии приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="1b5fc-119">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="1b5fc-119">Possible values are:</span></span></br><span data-ttu-id="1b5fc-120">`submitted` — конкретная версия приложения Teams была представлена и находится на рассмотрении.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="1b5fc-121">`published`  — Запрос на публикацию конкретной версии приложения Teams был утвержден администратором и приложение опубликовано.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="1b5fc-122">`rejected` — Запрос на публикацию конкретной версии приложения Teams был отклонен администратором.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="1b5fc-123">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="1b5fc-123">azureADAppId</span></span>        | <span data-ttu-id="1b5fc-124">Строка</span><span class="sxs-lookup"><span data-stu-id="1b5fc-124">string</span></span>   | <span data-ttu-id="1b5fc-125">В WebApplicationInfo.id из манифеста Teams App.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-125">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="1b5fc-126">displayName</span><span class="sxs-lookup"><span data-stu-id="1b5fc-126">displayName</span></span>         | <span data-ttu-id="1b5fc-127">string</span><span class="sxs-lookup"><span data-stu-id="1b5fc-127">string</span></span>   | <span data-ttu-id="1b5fc-128">Имя приложения, предоставленного разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-128">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="1b5fc-129">version</span><span class="sxs-lookup"><span data-stu-id="1b5fc-129">version</span></span>             | <span data-ttu-id="1b5fc-130">Строка</span><span class="sxs-lookup"><span data-stu-id="1b5fc-130">string</span></span>   | <span data-ttu-id="1b5fc-131">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-131">The version number of the application.</span></span> |
| <span data-ttu-id="1b5fc-132">allowedInstallationScopes</span><span class="sxs-lookup"><span data-stu-id="1b5fc-132">allowedInstallationScopes</span></span> | <span data-ttu-id="1b5fc-133">teamsAppInstallationScope collection</span><span class="sxs-lookup"><span data-stu-id="1b5fc-133">teamsAppInstallationScope collection</span></span> | <span data-ttu-id="1b5fc-134">Коллекция областей, в которых можно установить приложение Teams.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-134">A collection of scopes where the Teams app can be installed.</span></span> <span data-ttu-id="1b5fc-135">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="1b5fc-135">Possible values are:</span></span></br><span data-ttu-id="1b5fc-136">`team` — указывает, что приложение Teams может быть установлено в команде и уполномочено получать доступ к данным этой группы.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-136">`team` — Indicates that the Teams app can be installed within a team and is authorized to access that team's data.</span></span> </br><span data-ttu-id="1b5fc-137">`groupChat`  — указывает, что приложение Teams может быть установлено в групповом чате и уполномочено получать доступ к данным группового чата.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-137">`groupChat`  — Indicates that the Teams app can be installed within a group chat and is authorized to access that group chat's data.</span></span> </br> <span data-ttu-id="1b5fc-138">`personal` — указывает, что приложение Teams может быть установлено в личном поле пользователя и уполномочено получать доступ к данным этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-138">`personal` — Indicates that the Teams app can be installed in the personal scope of a user and is authorized to access that user's data.</span></span> | 

## <a name="relationships"></a><span data-ttu-id="1b5fc-139">Связи</span><span class="sxs-lookup"><span data-stu-id="1b5fc-139">Relationships</span></span>

| <span data-ttu-id="1b5fc-140">Связь</span><span class="sxs-lookup"><span data-stu-id="1b5fc-140">Relationship</span></span> | <span data-ttu-id="1b5fc-141">Тип</span><span class="sxs-lookup"><span data-stu-id="1b5fc-141">Type</span></span>   | <span data-ttu-id="1b5fc-142">Описание</span><span class="sxs-lookup"><span data-stu-id="1b5fc-142">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1b5fc-143">бот</span><span class="sxs-lookup"><span data-stu-id="1b5fc-143">bot</span></span>|[<span data-ttu-id="1b5fc-144">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="1b5fc-144">teamworkBot</span></span>](teamworkbot.md) | <span data-ttu-id="1b5fc-145">Сведения о боте, указанном в манифесте приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="1b5fc-145">The details of the bot specified in the Teams app manifest.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1b5fc-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1b5fc-146">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="1b5fc-147">См. также</span><span class="sxs-lookup"><span data-stu-id="1b5fc-147">See also</span></span>

- [<span data-ttu-id="1b5fc-148">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1b5fc-148">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="1b5fc-149">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1b5fc-149">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="1b5fc-150">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1b5fc-150">teamsTab</span></span>](../resources/teamstab.md)

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


