---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f4f13bf13b34c41c7c15c3356cc67636e6f441c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519927"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="e924d-103">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="e924d-103">teamsApp resource type</span></span>

<span data-ttu-id="e924d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e924d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e924d-105">Приложение в каталоге приложений [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e924d-105">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="e924d-106">Пользователи могут видеть эти приложения в магазине Microsoft Teams, а эти приложения можно устанавливать в [командах](team.md), используя метод [добавления приложения в команду](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="e924d-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="e924d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e924d-107">Methods</span></span>

| <span data-ttu-id="e924d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e924d-108">Method</span></span>       | <span data-ttu-id="e924d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e924d-109">Return Type</span></span>  |<span data-ttu-id="e924d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e924d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e924d-111">Список опубликованных приложений</span><span class="sxs-lookup"><span data-stu-id="e924d-111">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="e924d-112">Коллекция [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="e924d-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="e924d-113">Список опубликованных приложений из каталога приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e924d-113">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="e924d-114">Публикация приложения</span><span class="sxs-lookup"><span data-stu-id="e924d-114">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="e924d-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e924d-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="e924d-116">Публикация приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="e924d-116">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="e924d-117">Обновление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="e924d-117">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="e924d-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e924d-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="e924d-119">Обновление опубликованного приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="e924d-119">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="e924d-120">Удаление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="e924d-120">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="e924d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="e924d-121">None</span></span> | <span data-ttu-id="e924d-122">Удаление опубликованного приложения из каталога приложений организации.</span><span class="sxs-lookup"><span data-stu-id="e924d-122">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="e924d-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="e924d-123">Properties</span></span>

| <span data-ttu-id="e924d-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="e924d-124">Property</span></span>            | <span data-ttu-id="e924d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e924d-125">Type</span></span>     | <span data-ttu-id="e924d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e924d-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="e924d-127">id</span><span class="sxs-lookup"><span data-stu-id="e924d-127">id</span></span>                  | <span data-ttu-id="e924d-128">string</span><span class="sxs-lookup"><span data-stu-id="e924d-128">string</span></span>   | <span data-ttu-id="e924d-129">Сгенерированный идентификатор приложения из каталога приложений (отличающийся от предоставленного разработчиком идентификатора в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="e924d-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="e924d-130">externalId</span><span class="sxs-lookup"><span data-stu-id="e924d-130">externalId</span></span>          | <span data-ttu-id="e924d-131">строка</span><span class="sxs-lookup"><span data-stu-id="e924d-131">string</span></span>   | <span data-ttu-id="e924d-132">Идентификатор каталога, предоставленный разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="e924d-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="e924d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e924d-133">displayName</span></span>                | <span data-ttu-id="e924d-134">string</span><span class="sxs-lookup"><span data-stu-id="e924d-134">string</span></span>   | <span data-ttu-id="e924d-135">Название приложения каталога, предоставленное разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="e924d-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="e924d-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="e924d-136">distributionMethod</span></span>  | <span data-ttu-id="e924d-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="e924d-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="e924d-138">Метод распространения приложения.</span><span class="sxs-lookup"><span data-stu-id="e924d-138">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="e924d-139">Значения teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="e924d-139">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="e924d-140">Элемент</span><span class="sxs-lookup"><span data-stu-id="e924d-140">Member</span></span>|<span data-ttu-id="e924d-141">Значение</span><span class="sxs-lookup"><span data-stu-id="e924d-141">Value</span></span>|<span data-ttu-id="e924d-142">Описание</span><span class="sxs-lookup"><span data-stu-id="e924d-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e924d-143">store</span><span class="sxs-lookup"><span data-stu-id="e924d-143">store</span></span>|<span data-ttu-id="e924d-144">нуль</span><span class="sxs-lookup"><span data-stu-id="e924d-144">0</span></span>| <span data-ttu-id="e924d-145">Приложение доступно всем клиентам через магазин приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e924d-145">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="e924d-146">organization</span><span class="sxs-lookup"><span data-stu-id="e924d-146">organization</span></span>|<span data-ttu-id="e924d-147">1 </span><span class="sxs-lookup"><span data-stu-id="e924d-147">1</span></span>|<span data-ttu-id="e924d-148">Приложение доступно только в этом клиенте</span><span class="sxs-lookup"><span data-stu-id="e924d-148">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="e924d-149">sideloaded</span><span class="sxs-lookup"><span data-stu-id="e924d-149">sideloaded</span></span>|<span data-ttu-id="e924d-150">2 </span><span class="sxs-lookup"><span data-stu-id="e924d-150">2</span></span>|<span data-ttu-id="e924d-151">Приложение доступно только тому пользователю или той команде, где оно установлено.</span><span class="sxs-lookup"><span data-stu-id="e924d-151">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e924d-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="e924d-152">Relationships</span></span>

| <span data-ttu-id="e924d-153">Связь</span><span class="sxs-lookup"><span data-stu-id="e924d-153">Relationship</span></span> | <span data-ttu-id="e924d-154">Тип</span><span class="sxs-lookup"><span data-stu-id="e924d-154">Type</span></span>   | <span data-ttu-id="e924d-155">Описание</span><span class="sxs-lookup"><span data-stu-id="e924d-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e924d-156">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="e924d-156">appDefinitions</span></span>|<span data-ttu-id="e924d-157">Коллекция [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e924d-157">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="e924d-158">Сведения о каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="e924d-158">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e924d-159">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e924d-159">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

## <a name="see-also"></a><span data-ttu-id="e924d-160">См. также</span><span class="sxs-lookup"><span data-stu-id="e924d-160">See also</span></span>

- [<span data-ttu-id="e924d-161">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e924d-161">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="e924d-162">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e924d-162">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="e924d-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e924d-163">teamsTab</span></span>](../resources/teamstab.md)

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

