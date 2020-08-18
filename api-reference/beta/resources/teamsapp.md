---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f623a71a7d07a019615cfb43a664d875b8dd2def
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791612"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="889fa-103">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="889fa-103">teamsApp resource type</span></span>

<span data-ttu-id="889fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="889fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="889fa-105">Представляет приложение в каталоге приложений [Microsoft Teams](teams-api-overview.md) .</span><span class="sxs-lookup"><span data-stu-id="889fa-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="889fa-106">Пользователи могут видеть эти приложения в магазине Microsoft Teams, а эти приложения можно устанавливать в [командах](team.md), используя метод [добавления приложения в команду](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="889fa-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="889fa-107">Методы</span><span class="sxs-lookup"><span data-stu-id="889fa-107">Methods</span></span>

| <span data-ttu-id="889fa-108">Метод</span><span class="sxs-lookup"><span data-stu-id="889fa-108">Method</span></span>       | <span data-ttu-id="889fa-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="889fa-109">Return Type</span></span>  |<span data-ttu-id="889fa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="889fa-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="889fa-111">Список опубликованных приложений</span><span class="sxs-lookup"><span data-stu-id="889fa-111">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="889fa-112">Коллекция [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="889fa-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="889fa-113">Список опубликованных приложений из каталога приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="889fa-113">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="889fa-114">Публикация приложения</span><span class="sxs-lookup"><span data-stu-id="889fa-114">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="889fa-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="889fa-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="889fa-116">Публикация приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="889fa-116">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="889fa-117">Обновление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="889fa-117">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="889fa-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="889fa-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="889fa-119">Обновление опубликованного приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="889fa-119">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="889fa-120">Удаление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="889fa-120">Delete a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="889fa-121">Нет</span><span class="sxs-lookup"><span data-stu-id="889fa-121">None</span></span> | <span data-ttu-id="889fa-122">Удаление опубликованного приложения из каталога приложений организации.</span><span class="sxs-lookup"><span data-stu-id="889fa-122">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="889fa-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="889fa-123">Properties</span></span>

| <span data-ttu-id="889fa-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="889fa-124">Property</span></span>            | <span data-ttu-id="889fa-125">Тип</span><span class="sxs-lookup"><span data-stu-id="889fa-125">Type</span></span>     | <span data-ttu-id="889fa-126">Описание</span><span class="sxs-lookup"><span data-stu-id="889fa-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="889fa-127">id</span><span class="sxs-lookup"><span data-stu-id="889fa-127">id</span></span>                  | <span data-ttu-id="889fa-128">string</span><span class="sxs-lookup"><span data-stu-id="889fa-128">string</span></span>   | <span data-ttu-id="889fa-129">Сгенерированный идентификатор приложения из каталога приложений (отличающийся от предоставленного разработчиком идентификатора в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="889fa-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="889fa-130">externalId</span><span class="sxs-lookup"><span data-stu-id="889fa-130">externalId</span></span>          | <span data-ttu-id="889fa-131">строка</span><span class="sxs-lookup"><span data-stu-id="889fa-131">string</span></span>   | <span data-ttu-id="889fa-132">Идентификатор каталога, предоставленный разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="889fa-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="889fa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="889fa-133">displayName</span></span>                | <span data-ttu-id="889fa-134">string</span><span class="sxs-lookup"><span data-stu-id="889fa-134">string</span></span>   | <span data-ttu-id="889fa-135">Название приложения каталога, предоставленное разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="889fa-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="889fa-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="889fa-136">distributionMethod</span></span>  | <span data-ttu-id="889fa-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="889fa-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="889fa-138">Метод распространения приложения.</span><span class="sxs-lookup"><span data-stu-id="889fa-138">The method of distribution for the app.</span></span> <span data-ttu-id="889fa-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="889fa-139">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="889fa-140">Значения teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="889fa-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="889fa-141">Элемент</span><span class="sxs-lookup"><span data-stu-id="889fa-141">Member</span></span>|<span data-ttu-id="889fa-142">Значение</span><span class="sxs-lookup"><span data-stu-id="889fa-142">Value</span></span>|<span data-ttu-id="889fa-143">Описание</span><span class="sxs-lookup"><span data-stu-id="889fa-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="889fa-144">store</span><span class="sxs-lookup"><span data-stu-id="889fa-144">store</span></span>|<span data-ttu-id="889fa-145">нуль</span><span class="sxs-lookup"><span data-stu-id="889fa-145">0</span></span>| <span data-ttu-id="889fa-146">Приложение доступно всем клиентам через магазин приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="889fa-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="889fa-147">organization</span><span class="sxs-lookup"><span data-stu-id="889fa-147">organization</span></span>|<span data-ttu-id="889fa-148">1,1</span><span class="sxs-lookup"><span data-stu-id="889fa-148">1</span></span>|<span data-ttu-id="889fa-149">Приложение доступно только в этом клиенте</span><span class="sxs-lookup"><span data-stu-id="889fa-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="889fa-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="889fa-150">sideloaded</span></span>|<span data-ttu-id="889fa-151">2</span><span class="sxs-lookup"><span data-stu-id="889fa-151">2</span></span>|<span data-ttu-id="889fa-152">Приложение доступно только тому пользователю или той команде, где оно установлено.</span><span class="sxs-lookup"><span data-stu-id="889fa-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="889fa-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="889fa-153">Relationships</span></span>

| <span data-ttu-id="889fa-154">Связь</span><span class="sxs-lookup"><span data-stu-id="889fa-154">Relationship</span></span> | <span data-ttu-id="889fa-155">Тип</span><span class="sxs-lookup"><span data-stu-id="889fa-155">Type</span></span>   | <span data-ttu-id="889fa-156">Описание</span><span class="sxs-lookup"><span data-stu-id="889fa-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="889fa-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="889fa-157">appDefinitions</span></span>|<span data-ttu-id="889fa-158">Коллекция [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="889fa-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="889fa-159">Сведения о каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="889fa-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="889fa-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="889fa-160">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="889fa-161">См. также</span><span class="sxs-lookup"><span data-stu-id="889fa-161">See also</span></span>

- [<span data-ttu-id="889fa-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="889fa-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="889fa-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="889fa-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="889fa-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="889fa-164">teamsTab</span></span>](../resources/teamstab.md)

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

