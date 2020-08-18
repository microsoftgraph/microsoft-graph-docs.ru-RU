---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2307bd50509cc1a44ee4de0a30309a2be98dcb3e
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791675"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="8e3b0-103">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="8e3b0-103">teamsApp resource type</span></span>

<span data-ttu-id="8e3b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e3b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e3b0-105">Представляет приложение в каталоге приложений [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8e3b0-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="8e3b0-106">Пользователи могут видеть эти приложения в магазине Microsoft Teams, а эти приложения можно устанавливать в [командах](team.md), используя метод [добавления приложения в команду](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="8e3b0-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="8e3b0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8e3b0-107">Methods</span></span>

| <span data-ttu-id="8e3b0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8e3b0-108">Method</span></span>       | <span data-ttu-id="8e3b0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8e3b0-109">Return Type</span></span>  |<span data-ttu-id="8e3b0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8e3b0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8e3b0-111">Список опубликованных приложений</span><span class="sxs-lookup"><span data-stu-id="8e3b0-111">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="8e3b0-112">Коллекция [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e3b0-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="8e3b0-113">Список опубликованных приложений из каталога приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8e3b0-113">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="8e3b0-114">Публикация приложения</span><span class="sxs-lookup"><span data-stu-id="8e3b0-114">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="8e3b0-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8e3b0-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="8e3b0-116">Публикация приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="8e3b0-116">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="8e3b0-117">Обновление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="8e3b0-117">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="8e3b0-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8e3b0-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="8e3b0-119">Обновление опубликованного приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="8e3b0-119">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="8e3b0-120">Удаление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="8e3b0-120">Delete a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="8e3b0-121">Нет</span><span class="sxs-lookup"><span data-stu-id="8e3b0-121">None</span></span> | <span data-ttu-id="8e3b0-122">Удаление опубликованного приложения из каталога приложений организации.</span><span class="sxs-lookup"><span data-stu-id="8e3b0-122">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e3b0-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e3b0-123">Properties</span></span>

| <span data-ttu-id="8e3b0-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e3b0-124">Property</span></span>            | <span data-ttu-id="8e3b0-125">Тип</span><span class="sxs-lookup"><span data-stu-id="8e3b0-125">Type</span></span>     | <span data-ttu-id="8e3b0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8e3b0-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="8e3b0-127">id</span><span class="sxs-lookup"><span data-stu-id="8e3b0-127">id</span></span>                  | <span data-ttu-id="8e3b0-128">string</span><span class="sxs-lookup"><span data-stu-id="8e3b0-128">string</span></span>   | <span data-ttu-id="8e3b0-129">Сгенерированный идентификатор приложения из каталога приложений (отличающийся от предоставленного разработчиком идентификатора в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8e3b0-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="8e3b0-130">externalId</span><span class="sxs-lookup"><span data-stu-id="8e3b0-130">externalId</span></span>          | <span data-ttu-id="8e3b0-131">строка</span><span class="sxs-lookup"><span data-stu-id="8e3b0-131">string</span></span>   | <span data-ttu-id="8e3b0-132">Идентификатор каталога, предоставленный разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8e3b0-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="8e3b0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8e3b0-133">displayName</span></span>                | <span data-ttu-id="8e3b0-134">string</span><span class="sxs-lookup"><span data-stu-id="8e3b0-134">string</span></span>   | <span data-ttu-id="8e3b0-135">Название приложения каталога, предоставленное разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8e3b0-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="8e3b0-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="8e3b0-136">distributionMethod</span></span>  | <span data-ttu-id="8e3b0-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="8e3b0-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="8e3b0-138">Метод распространения приложения.</span><span class="sxs-lookup"><span data-stu-id="8e3b0-138">The method of distribution for the app.</span></span> <span data-ttu-id="8e3b0-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e3b0-139">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="8e3b0-140">Значения teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="8e3b0-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="8e3b0-141">Элемент</span><span class="sxs-lookup"><span data-stu-id="8e3b0-141">Member</span></span>|<span data-ttu-id="8e3b0-142">Значение</span><span class="sxs-lookup"><span data-stu-id="8e3b0-142">Value</span></span>|<span data-ttu-id="8e3b0-143">Описание</span><span class="sxs-lookup"><span data-stu-id="8e3b0-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e3b0-144">store</span><span class="sxs-lookup"><span data-stu-id="8e3b0-144">store</span></span>|<span data-ttu-id="8e3b0-145">0</span><span class="sxs-lookup"><span data-stu-id="8e3b0-145">0</span></span>| <span data-ttu-id="8e3b0-146">Приложение доступно всем клиентам через магазин приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8e3b0-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="8e3b0-147">organization</span><span class="sxs-lookup"><span data-stu-id="8e3b0-147">organization</span></span>|<span data-ttu-id="8e3b0-148">1</span><span class="sxs-lookup"><span data-stu-id="8e3b0-148">1</span></span>|<span data-ttu-id="8e3b0-149">Приложение доступно только в этом клиенте</span><span class="sxs-lookup"><span data-stu-id="8e3b0-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="8e3b0-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="8e3b0-150">sideloaded</span></span>|<span data-ttu-id="8e3b0-151">2</span><span class="sxs-lookup"><span data-stu-id="8e3b0-151">2</span></span>|<span data-ttu-id="8e3b0-152">Приложение доступно только тому пользователю или той команде, где оно установлено.</span><span class="sxs-lookup"><span data-stu-id="8e3b0-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e3b0-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="8e3b0-153">Relationships</span></span>

| <span data-ttu-id="8e3b0-154">Связь</span><span class="sxs-lookup"><span data-stu-id="8e3b0-154">Relationship</span></span> | <span data-ttu-id="8e3b0-155">Тип</span><span class="sxs-lookup"><span data-stu-id="8e3b0-155">Type</span></span>   | <span data-ttu-id="8e3b0-156">Описание</span><span class="sxs-lookup"><span data-stu-id="8e3b0-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8e3b0-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="8e3b0-157">appDefinitions</span></span>|<span data-ttu-id="8e3b0-158">Коллекция [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e3b0-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="8e3b0-159">Сведения о каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="8e3b0-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8e3b0-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8e3b0-160">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8e3b0-161">См. также</span><span class="sxs-lookup"><span data-stu-id="8e3b0-161">See also</span></span>

- [<span data-ttu-id="8e3b0-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8e3b0-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="8e3b0-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="8e3b0-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="8e3b0-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8e3b0-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

