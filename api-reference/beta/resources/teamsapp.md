---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4a890cea9763bd8615495d4d9597601a508fafc6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046603"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="8eb45-103">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="8eb45-103">teamsApp resource type</span></span>

<span data-ttu-id="8eb45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eb45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8eb45-105">Представляет приложение в каталоге приложений [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8eb45-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="8eb45-106">Пользователи могут видеть эти приложения в магазине Microsoft Teams, а эти приложения можно устанавливать в [командах](team.md), используя метод [добавления приложения в команду](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="8eb45-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="8eb45-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8eb45-107">Methods</span></span>

| <span data-ttu-id="8eb45-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8eb45-108">Method</span></span>       | <span data-ttu-id="8eb45-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8eb45-109">Return Type</span></span>  |<span data-ttu-id="8eb45-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb45-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8eb45-111">Список опубликованных приложений</span><span class="sxs-lookup"><span data-stu-id="8eb45-111">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="8eb45-112">Коллекция [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eb45-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="8eb45-113">Список опубликованных приложений из каталога приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8eb45-113">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="8eb45-114">Публикация приложения</span><span class="sxs-lookup"><span data-stu-id="8eb45-114">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="8eb45-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8eb45-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="8eb45-116">Публикация приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="8eb45-116">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="8eb45-117">Обновление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="8eb45-117">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="8eb45-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8eb45-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="8eb45-119">Обновление опубликованного приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="8eb45-119">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="8eb45-120">Удаление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="8eb45-120">Delete a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="8eb45-121">Нет</span><span class="sxs-lookup"><span data-stu-id="8eb45-121">None</span></span> | <span data-ttu-id="8eb45-122">Удаление опубликованного приложения из каталога приложений организации.</span><span class="sxs-lookup"><span data-stu-id="8eb45-122">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="8eb45-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="8eb45-123">Properties</span></span>

| <span data-ttu-id="8eb45-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="8eb45-124">Property</span></span>            | <span data-ttu-id="8eb45-125">Тип</span><span class="sxs-lookup"><span data-stu-id="8eb45-125">Type</span></span>     | <span data-ttu-id="8eb45-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb45-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="8eb45-127">id</span><span class="sxs-lookup"><span data-stu-id="8eb45-127">id</span></span>                  | <span data-ttu-id="8eb45-128">string</span><span class="sxs-lookup"><span data-stu-id="8eb45-128">string</span></span>   | <span data-ttu-id="8eb45-129">Сгенерированный идентификатор приложения из каталога приложений (отличающийся от предоставленного разработчиком идентификатора в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8eb45-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="8eb45-130">externalId</span><span class="sxs-lookup"><span data-stu-id="8eb45-130">externalId</span></span>          | <span data-ttu-id="8eb45-131">строка</span><span class="sxs-lookup"><span data-stu-id="8eb45-131">string</span></span>   | <span data-ttu-id="8eb45-132">Идентификатор каталога, предоставленный разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8eb45-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="8eb45-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8eb45-133">displayName</span></span>                | <span data-ttu-id="8eb45-134">string</span><span class="sxs-lookup"><span data-stu-id="8eb45-134">string</span></span>   | <span data-ttu-id="8eb45-135">Название приложения каталога, предоставленное разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8eb45-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="8eb45-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="8eb45-136">distributionMethod</span></span>  | <span data-ttu-id="8eb45-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="8eb45-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="8eb45-138">Метод распространения приложения.</span><span class="sxs-lookup"><span data-stu-id="8eb45-138">The method of distribution for the app.</span></span> <span data-ttu-id="8eb45-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8eb45-139">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="8eb45-140">Значения teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="8eb45-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="8eb45-141">Элемент</span><span class="sxs-lookup"><span data-stu-id="8eb45-141">Member</span></span>|<span data-ttu-id="8eb45-142">Значение</span><span class="sxs-lookup"><span data-stu-id="8eb45-142">Value</span></span>|<span data-ttu-id="8eb45-143">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb45-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eb45-144">store</span><span class="sxs-lookup"><span data-stu-id="8eb45-144">store</span></span>|<span data-ttu-id="8eb45-145">0</span><span class="sxs-lookup"><span data-stu-id="8eb45-145">0</span></span>| <span data-ttu-id="8eb45-146">Приложение доступно всем клиентам через магазин приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8eb45-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="8eb45-147">organization</span><span class="sxs-lookup"><span data-stu-id="8eb45-147">organization</span></span>|<span data-ttu-id="8eb45-148">1</span><span class="sxs-lookup"><span data-stu-id="8eb45-148">1</span></span>|<span data-ttu-id="8eb45-149">Приложение доступно только в этом клиенте</span><span class="sxs-lookup"><span data-stu-id="8eb45-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="8eb45-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="8eb45-150">sideloaded</span></span>|<span data-ttu-id="8eb45-151">2</span><span class="sxs-lookup"><span data-stu-id="8eb45-151">2</span></span>|<span data-ttu-id="8eb45-152">Приложение доступно только тому пользователю или той команде, где оно установлено.</span><span class="sxs-lookup"><span data-stu-id="8eb45-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8eb45-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="8eb45-153">Relationships</span></span>

| <span data-ttu-id="8eb45-154">Связь</span><span class="sxs-lookup"><span data-stu-id="8eb45-154">Relationship</span></span> | <span data-ttu-id="8eb45-155">Тип</span><span class="sxs-lookup"><span data-stu-id="8eb45-155">Type</span></span>   | <span data-ttu-id="8eb45-156">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb45-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8eb45-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="8eb45-157">appDefinitions</span></span>|<span data-ttu-id="8eb45-158">Коллекция [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8eb45-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="8eb45-159">Сведения о каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="8eb45-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8eb45-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8eb45-160">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8eb45-161">См. также</span><span class="sxs-lookup"><span data-stu-id="8eb45-161">See also</span></span>

- [<span data-ttu-id="8eb45-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8eb45-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="8eb45-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="8eb45-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="8eb45-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8eb45-164">teamsTab</span></span>](../resources/teamstab.md)

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



