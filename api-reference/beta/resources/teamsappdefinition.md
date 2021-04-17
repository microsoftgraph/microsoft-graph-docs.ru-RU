---
title: тип ресурса teamsAppDefinition
description: Сведения об одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4e8bfd4b7248d37ce8ec4d85e01a498a88fed1c3
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882322"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="d1f45-103">тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d1f45-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="d1f45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1f45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1f45-105">Сведения о версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="d1f45-105">The details of a version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d1f45-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1f45-106">Properties</span></span>

| <span data-ttu-id="d1f45-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1f45-107">Property</span></span>            | <span data-ttu-id="d1f45-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d1f45-108">Type</span></span>     | <span data-ttu-id="d1f45-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f45-109">Description</span></span>                                            |
|:------------------- |:-------- |:------------------------------------------------------ |
| <span data-ttu-id="d1f45-110">id</span><span class="sxs-lookup"><span data-stu-id="d1f45-110">id</span></span>                  | <span data-ttu-id="d1f45-111">string</span><span class="sxs-lookup"><span data-stu-id="d1f45-111">string</span></span>   | <span data-ttu-id="d1f45-112">Уникальный ID (а не ID приложения Teams).</span><span class="sxs-lookup"><span data-stu-id="d1f45-112">A unique ID (not the Teams app ID).</span></span>                     |
| <span data-ttu-id="d1f45-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="d1f45-113">teamsAppId</span></span>          | <span data-ttu-id="d1f45-114">Строка</span><span class="sxs-lookup"><span data-stu-id="d1f45-114">string</span></span>   | <span data-ttu-id="d1f45-115">ID из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="d1f45-115">The ID from the Teams app manifest.</span></span>                    |
| <span data-ttu-id="d1f45-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="d1f45-116">publishingState</span></span>     | <span data-ttu-id="d1f45-117">Строка</span><span class="sxs-lookup"><span data-stu-id="d1f45-117">string</span></span>   | <span data-ttu-id="d1f45-118">Опубликованный статус определенной версии приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="d1f45-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="d1f45-119">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="d1f45-119">Possible values are:</span></span></br><span data-ttu-id="d1f45-120">`submitted` — конкретная версия приложения Teams была представлена и находится на рассмотрении.</span><span class="sxs-lookup"><span data-stu-id="d1f45-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="d1f45-121">`published`  — Запрос на публикацию конкретной версии приложения Teams был утвержден администратором и приложение опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d1f45-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="d1f45-122">`rejected` — Запрос на публикацию конкретной версии приложения Teams был отклонен администратором.</span><span class="sxs-lookup"><span data-stu-id="d1f45-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="d1f45-123">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="d1f45-123">azureADAppId</span></span>        | <span data-ttu-id="d1f45-124">Строка</span><span class="sxs-lookup"><span data-stu-id="d1f45-124">string</span></span>   | <span data-ttu-id="d1f45-125">В WebApplicationInfo.Id из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="d1f45-125">The WebApplicationInfo.Id from the Teams app manifest.</span></span> |
| <span data-ttu-id="d1f45-126">displayName</span><span class="sxs-lookup"><span data-stu-id="d1f45-126">displayName</span></span>         | <span data-ttu-id="d1f45-127">string</span><span class="sxs-lookup"><span data-stu-id="d1f45-127">string</span></span>   | <span data-ttu-id="d1f45-128">Имя приложения, предоставленного разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="d1f45-128">The name of the app provided by the app developer.</span></span>     |
| <span data-ttu-id="d1f45-129">version</span><span class="sxs-lookup"><span data-stu-id="d1f45-129">version</span></span>             | <span data-ttu-id="d1f45-130">Строка</span><span class="sxs-lookup"><span data-stu-id="d1f45-130">string</span></span>   | <span data-ttu-id="d1f45-131">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="d1f45-131">The version number of the application.</span></span>                 |
| <span data-ttu-id="d1f45-132">allowedInstallationScopes</span><span class="sxs-lookup"><span data-stu-id="d1f45-132">allowedInstallationScopes</span></span> | <span data-ttu-id="d1f45-133">teamsAppInstallationScope collection</span><span class="sxs-lookup"><span data-stu-id="d1f45-133">teamsAppInstallationScope collection</span></span> | <span data-ttu-id="d1f45-134">Коллекция областей, в которых можно установить приложение Teams.</span><span class="sxs-lookup"><span data-stu-id="d1f45-134">A collection of scopes where the Teams app can be installed.</span></span> <span data-ttu-id="d1f45-135">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="d1f45-135">Possible values are:</span></span></br><span data-ttu-id="d1f45-136">`team` — указывает, что приложение Teams может быть установлено в команде и уполномочено получать доступ к данным этой группы.</span><span class="sxs-lookup"><span data-stu-id="d1f45-136">`team` — Indicates that the Teams app can be installed within a team and is authorized to access that team's data.</span></span> </br><span data-ttu-id="d1f45-137">`groupChat`  — указывает, что приложение Teams может быть установлено в групповом чате и уполномочено получать доступ к данным группового чата.</span><span class="sxs-lookup"><span data-stu-id="d1f45-137">`groupChat`  — Indicates that the Teams app can be installed within a group chat and is authorized to access that group chat's data.</span></span> </br> <span data-ttu-id="d1f45-138">`personal` — указывает, что приложение Teams может быть установлено в личном поле пользователя и уполномочено получать доступ к данным этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="d1f45-138">`personal` — Indicates that the Teams app can be installed in the personal scope of a user and is authorized to access that user's data.</span></span> | 

## <a name="relationships"></a><span data-ttu-id="d1f45-139">Связи</span><span class="sxs-lookup"><span data-stu-id="d1f45-139">Relationships</span></span>

| <span data-ttu-id="d1f45-140">Связь</span><span class="sxs-lookup"><span data-stu-id="d1f45-140">Relationship</span></span>   | <span data-ttu-id="d1f45-141">Тип</span><span class="sxs-lookup"><span data-stu-id="d1f45-141">Type</span></span>                           | <span data-ttu-id="d1f45-142">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f45-142">Description</span></span>                                                 |
|:-------------- |:------------------------------ |:----------------------------------------------------------- |
| <span data-ttu-id="d1f45-143">бот</span><span class="sxs-lookup"><span data-stu-id="d1f45-143">bot</span></span>            |[<span data-ttu-id="d1f45-144">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="d1f45-144">teamworkBot</span></span>](teamworkbot.md)   | <span data-ttu-id="d1f45-145">Сведения о боте, указанном в манифесте приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="d1f45-145">The details of the bot specified in the Teams app manifest.</span></span> |
| <span data-ttu-id="d1f45-146">colorIcon</span><span class="sxs-lookup"><span data-stu-id="d1f45-146">colorIcon</span></span>      |[<span data-ttu-id="d1f45-147">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="d1f45-147">teamsAppIcon</span></span>](teamsappicon.md) | <span data-ttu-id="d1f45-148">Цветная версия значка приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="d1f45-148">The color version of the Teams app's icon.</span></span>                   |
| <span data-ttu-id="d1f45-149">outlineIcon</span><span class="sxs-lookup"><span data-stu-id="d1f45-149">outlineIcon</span></span>    |[<span data-ttu-id="d1f45-150">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="d1f45-150">teamsAppIcon</span></span>](teamsappicon.md) | <span data-ttu-id="d1f45-151">Очертания версии значка приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="d1f45-151">The outline version of the Teams app's icon.</span></span>                 |

## <a name="json-representation"></a><span data-ttu-id="d1f45-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d1f45-152">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "publishingState": "#microsoft.graph.teamsAppPublishingState",
  "azureADAppId": "string",
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="d1f45-153">См. также</span><span class="sxs-lookup"><span data-stu-id="d1f45-153">See also</span></span>

- [<span data-ttu-id="d1f45-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d1f45-154">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="d1f45-155">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="d1f45-155">teamsAppIcon</span></span>](teamsappicon.md)
- [<span data-ttu-id="d1f45-156">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d1f45-156">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="d1f45-157">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d1f45-157">teamsTab</span></span>](../resources/teamstab.md)

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


