---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 55fd373fd59f79abdfca8b3e066ca496daf8770b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706005"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="35cf8-103">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="35cf8-103">teamsApp resource type</span></span>

<span data-ttu-id="35cf8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35cf8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35cf8-105">Представляет приложение в каталоге приложений [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="35cf8-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="35cf8-106">Пользователи могут видеть эти приложения в магазине Microsoft Teams, а эти приложения можно устанавливать в [командах](team.md), используя метод [добавления приложения в команду](../api/team-post-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="35cf8-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/team-post-installedapps.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="35cf8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="35cf8-107">Methods</span></span>

| <span data-ttu-id="35cf8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="35cf8-108">Method</span></span>       | <span data-ttu-id="35cf8-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="35cf8-109">Return Type</span></span>  |<span data-ttu-id="35cf8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="35cf8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35cf8-111">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="35cf8-111">List apps in catalog</span></span>](../api/appcatalogs-list-teamsapps.md) | <span data-ttu-id="35cf8-112">Коллекция [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="35cf8-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="35cf8-113">Перечисление всех приложений в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="35cf8-113">List all the apps in the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="35cf8-114">Отправка приложения в каталог</span><span class="sxs-lookup"><span data-stu-id="35cf8-114">Upload app to catalog</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="35cf8-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="35cf8-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="35cf8-116">Отправка приложения в каталог приложений организации.</span><span class="sxs-lookup"><span data-stu-id="35cf8-116">Upload an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="35cf8-117">Обновление приложения в каталоге</span><span class="sxs-lookup"><span data-stu-id="35cf8-117">Update app in catalog</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="35cf8-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="35cf8-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="35cf8-119">Обновление приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="35cf8-119">Update an app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="35cf8-120">Удаление приложения из каталога</span><span class="sxs-lookup"><span data-stu-id="35cf8-120">Delete app from catalog</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="35cf8-121">Нет</span><span class="sxs-lookup"><span data-stu-id="35cf8-121">None</span></span> | <span data-ttu-id="35cf8-122">Удаление приложения из каталога приложений организации.</span><span class="sxs-lookup"><span data-stu-id="35cf8-122">Remove an app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="35cf8-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="35cf8-123">Properties</span></span>

| <span data-ttu-id="35cf8-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="35cf8-124">Property</span></span>            | <span data-ttu-id="35cf8-125">Тип</span><span class="sxs-lookup"><span data-stu-id="35cf8-125">Type</span></span>     | <span data-ttu-id="35cf8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="35cf8-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="35cf8-127">id</span><span class="sxs-lookup"><span data-stu-id="35cf8-127">id</span></span>                  | <span data-ttu-id="35cf8-128">string</span><span class="sxs-lookup"><span data-stu-id="35cf8-128">string</span></span>   | <span data-ttu-id="35cf8-129">Сгенерированный идентификатор приложения из каталога приложений (отличающийся от предоставленного разработчиком идентификатора в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="35cf8-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="35cf8-130">externalId</span><span class="sxs-lookup"><span data-stu-id="35cf8-130">externalId</span></span>          | <span data-ttu-id="35cf8-131">строка</span><span class="sxs-lookup"><span data-stu-id="35cf8-131">string</span></span>   | <span data-ttu-id="35cf8-132">Идентификатор каталога, предоставленный разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="35cf8-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="35cf8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="35cf8-133">displayName</span></span>                | <span data-ttu-id="35cf8-134">string</span><span class="sxs-lookup"><span data-stu-id="35cf8-134">string</span></span>   | <span data-ttu-id="35cf8-135">Название приложения каталога, предоставленное разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="35cf8-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="35cf8-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="35cf8-136">distributionMethod</span></span>  | <span data-ttu-id="35cf8-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="35cf8-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="35cf8-138">Метод распространения приложения.</span><span class="sxs-lookup"><span data-stu-id="35cf8-138">The method of distribution for the app.</span></span> <span data-ttu-id="35cf8-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35cf8-139">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="35cf8-140">Значения teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="35cf8-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="35cf8-141">Элемент</span><span class="sxs-lookup"><span data-stu-id="35cf8-141">Member</span></span>|<span data-ttu-id="35cf8-142">Значение</span><span class="sxs-lookup"><span data-stu-id="35cf8-142">Value</span></span>|<span data-ttu-id="35cf8-143">Описание</span><span class="sxs-lookup"><span data-stu-id="35cf8-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35cf8-144">store</span><span class="sxs-lookup"><span data-stu-id="35cf8-144">store</span></span>|<span data-ttu-id="35cf8-145">0</span><span class="sxs-lookup"><span data-stu-id="35cf8-145">0</span></span>| <span data-ttu-id="35cf8-146">Приложение доступно всем клиентам через магазин приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="35cf8-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="35cf8-147">organization</span><span class="sxs-lookup"><span data-stu-id="35cf8-147">organization</span></span>|<span data-ttu-id="35cf8-148">1</span><span class="sxs-lookup"><span data-stu-id="35cf8-148">1</span></span>|<span data-ttu-id="35cf8-149">Приложение доступно только в этом клиенте</span><span class="sxs-lookup"><span data-stu-id="35cf8-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="35cf8-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="35cf8-150">sideloaded</span></span>|<span data-ttu-id="35cf8-151">2</span><span class="sxs-lookup"><span data-stu-id="35cf8-151">2</span></span>|<span data-ttu-id="35cf8-152">Приложение доступно только тому пользователю или той команде, где оно установлено.</span><span class="sxs-lookup"><span data-stu-id="35cf8-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35cf8-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="35cf8-153">Relationships</span></span>

| <span data-ttu-id="35cf8-154">Связь</span><span class="sxs-lookup"><span data-stu-id="35cf8-154">Relationship</span></span> | <span data-ttu-id="35cf8-155">Тип</span><span class="sxs-lookup"><span data-stu-id="35cf8-155">Type</span></span>   | <span data-ttu-id="35cf8-156">Описание</span><span class="sxs-lookup"><span data-stu-id="35cf8-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="35cf8-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="35cf8-157">appDefinitions</span></span>|<span data-ttu-id="35cf8-158">Коллекция [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="35cf8-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="35cf8-159">Сведения о каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="35cf8-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35cf8-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="35cf8-160">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="35cf8-161">См. также</span><span class="sxs-lookup"><span data-stu-id="35cf8-161">See also</span></span>

- [<span data-ttu-id="35cf8-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="35cf8-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="35cf8-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="35cf8-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="35cf8-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="35cf8-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


