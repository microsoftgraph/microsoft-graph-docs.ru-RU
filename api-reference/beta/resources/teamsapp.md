---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: eb7c75f144f2056e610e45f86b44a19d9211f306
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706124"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="5ef71-103">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="5ef71-103">teamsApp resource type</span></span>

<span data-ttu-id="5ef71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ef71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ef71-105">Представляет приложение в каталоге приложений [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="5ef71-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="5ef71-106">Пользователи могут видеть эти приложения в магазине Microsoft Teams, а эти приложения можно устанавливать в [командах](team.md), используя метод [добавления приложения в команду](../api/team-post-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="5ef71-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/team-post-installedapps.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="5ef71-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5ef71-107">Methods</span></span>

| <span data-ttu-id="5ef71-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5ef71-108">Method</span></span>       | <span data-ttu-id="5ef71-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5ef71-109">Return Type</span></span>  |<span data-ttu-id="5ef71-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5ef71-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5ef71-111">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="5ef71-111">List apps in catalog</span></span>](../api/appcatalogs-list-teamsapps.md) | <span data-ttu-id="5ef71-112">Коллекция [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ef71-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="5ef71-113">Список всех приложений в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5ef71-113">List all the apps in the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="5ef71-114">Отправка приложения в каталог</span><span class="sxs-lookup"><span data-stu-id="5ef71-114">Upload app to catalog</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="5ef71-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5ef71-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="5ef71-116">Отправка приложения в каталог приложений организации.</span><span class="sxs-lookup"><span data-stu-id="5ef71-116">Upload an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="5ef71-117">Обновление приложения в каталоге</span><span class="sxs-lookup"><span data-stu-id="5ef71-117">Update app in catalog</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="5ef71-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5ef71-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="5ef71-119">Обновление приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="5ef71-119">Update an app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="5ef71-120">Удаление приложения из каталога</span><span class="sxs-lookup"><span data-stu-id="5ef71-120">Delete app from catalog</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="5ef71-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5ef71-121">None</span></span> | <span data-ttu-id="5ef71-122">Удаление приложения из каталога приложений организации.</span><span class="sxs-lookup"><span data-stu-id="5ef71-122">Remove an app from your organization's app catalog.</span></span>|
|[<span data-ttu-id="5ef71-123">Получить бота, связанного с приложением в каталоге</span><span class="sxs-lookup"><span data-stu-id="5ef71-123">Get bot associated with app in catalog</span></span>](../api/teamworkbot-get.md) | [<span data-ttu-id="5ef71-124">teamworkbot</span><span class="sxs-lookup"><span data-stu-id="5ef71-124">teamworkbot</span></span>](teamworkbot.md) | <span data-ttu-id="5ef71-125">Получите бота, связанного с приложением Teams.</span><span class="sxs-lookup"><span data-stu-id="5ef71-125">Get the bot associated with the Teams app.</span></span>|

## <a name="properties"></a><span data-ttu-id="5ef71-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ef71-126">Properties</span></span>

| <span data-ttu-id="5ef71-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ef71-127">Property</span></span>            | <span data-ttu-id="5ef71-128">Тип</span><span class="sxs-lookup"><span data-stu-id="5ef71-128">Type</span></span>     | <span data-ttu-id="5ef71-129">Описание</span><span class="sxs-lookup"><span data-stu-id="5ef71-129">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="5ef71-130">id</span><span class="sxs-lookup"><span data-stu-id="5ef71-130">id</span></span>                  | <span data-ttu-id="5ef71-131">строка</span><span class="sxs-lookup"><span data-stu-id="5ef71-131">string</span></span>   | <span data-ttu-id="5ef71-132">Сгенерированный идентификатор приложения из каталога приложений (отличающийся от предоставленного разработчиком идентификатора в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="5ef71-132">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="5ef71-133">externalId</span><span class="sxs-lookup"><span data-stu-id="5ef71-133">externalId</span></span>          | <span data-ttu-id="5ef71-134">string</span><span class="sxs-lookup"><span data-stu-id="5ef71-134">string</span></span>   | <span data-ttu-id="5ef71-135">Идентификатор каталога, предоставленный разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="5ef71-135">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="5ef71-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5ef71-136">displayName</span></span>                | <span data-ttu-id="5ef71-137">string</span><span class="sxs-lookup"><span data-stu-id="5ef71-137">string</span></span>   | <span data-ttu-id="5ef71-138">Название приложения каталога, предоставленное разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="5ef71-138">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="5ef71-139">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="5ef71-139">distributionMethod</span></span>  | <span data-ttu-id="5ef71-140">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="5ef71-140">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="5ef71-141">Метод распространения приложения.</span><span class="sxs-lookup"><span data-stu-id="5ef71-141">The method of distribution for the app.</span></span> <span data-ttu-id="5ef71-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ef71-142">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="5ef71-143">Значения teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="5ef71-143">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="5ef71-144">Элемент</span><span class="sxs-lookup"><span data-stu-id="5ef71-144">Member</span></span>|<span data-ttu-id="5ef71-145">Значение</span><span class="sxs-lookup"><span data-stu-id="5ef71-145">Value</span></span>|<span data-ttu-id="5ef71-146">Описание</span><span class="sxs-lookup"><span data-stu-id="5ef71-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ef71-147">store</span><span class="sxs-lookup"><span data-stu-id="5ef71-147">store</span></span>|<span data-ttu-id="5ef71-148">0</span><span class="sxs-lookup"><span data-stu-id="5ef71-148">0</span></span>| <span data-ttu-id="5ef71-149">Приложение доступно всем клиентам через магазин приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5ef71-149">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="5ef71-150">organization</span><span class="sxs-lookup"><span data-stu-id="5ef71-150">organization</span></span>|<span data-ttu-id="5ef71-151">1</span><span class="sxs-lookup"><span data-stu-id="5ef71-151">1</span></span>|<span data-ttu-id="5ef71-152">Приложение доступно только в этом клиенте</span><span class="sxs-lookup"><span data-stu-id="5ef71-152">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="5ef71-153">sideloaded</span><span class="sxs-lookup"><span data-stu-id="5ef71-153">sideloaded</span></span>|<span data-ttu-id="5ef71-154">2</span><span class="sxs-lookup"><span data-stu-id="5ef71-154">2</span></span>|<span data-ttu-id="5ef71-155">Приложение доступно только тому пользователю или той команде, где оно установлено.</span><span class="sxs-lookup"><span data-stu-id="5ef71-155">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ef71-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="5ef71-156">Relationships</span></span>

| <span data-ttu-id="5ef71-157">Связь</span><span class="sxs-lookup"><span data-stu-id="5ef71-157">Relationship</span></span> | <span data-ttu-id="5ef71-158">Тип</span><span class="sxs-lookup"><span data-stu-id="5ef71-158">Type</span></span>   | <span data-ttu-id="5ef71-159">Описание</span><span class="sxs-lookup"><span data-stu-id="5ef71-159">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5ef71-160">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="5ef71-160">appDefinitions</span></span>|<span data-ttu-id="5ef71-161">Коллекция [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5ef71-161">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="5ef71-162">Сведения о каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="5ef71-162">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5ef71-163">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5ef71-163">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "string",
  "distributionMethod": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="5ef71-164">См. также</span><span class="sxs-lookup"><span data-stu-id="5ef71-164">See also</span></span>

- [<span data-ttu-id="5ef71-165">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="5ef71-165">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="5ef71-166">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="5ef71-166">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="5ef71-167">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5ef71-167">teamsTab</span></span>](../resources/teamstab.md)

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



