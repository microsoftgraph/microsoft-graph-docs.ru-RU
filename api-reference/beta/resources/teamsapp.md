---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f629851225570426b5785911bbbdb3337f43149f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964510"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="9fe5f-103">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="9fe5f-103">teamsApp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fe5f-104">Приложение в каталоге приложений [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9fe5f-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="9fe5f-105">Пользователи могут видеть эти приложения в магазине Microsoft Teams, а эти приложения можно устанавливать в [командах](team.md), используя метод [добавления приложения в команду](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="9fe5f-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="9fe5f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9fe5f-106">Methods</span></span>

| <span data-ttu-id="9fe5f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9fe5f-107">Method</span></span>       | <span data-ttu-id="9fe5f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9fe5f-108">Return Type</span></span>  |<span data-ttu-id="9fe5f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9fe5f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9fe5f-110">Список опубликованных приложений</span><span class="sxs-lookup"><span data-stu-id="9fe5f-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="9fe5f-111">Коллекция [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fe5f-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="9fe5f-112">Список опубликованных приложений из каталога приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9fe5f-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="9fe5f-113">Публикация приложения</span><span class="sxs-lookup"><span data-stu-id="9fe5f-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="9fe5f-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9fe5f-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="9fe5f-115">Публикация приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="9fe5f-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="9fe5f-116">Обновление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="9fe5f-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="9fe5f-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9fe5f-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="9fe5f-118">Обновление опубликованного приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="9fe5f-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="9fe5f-119">Удаление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="9fe5f-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="9fe5f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9fe5f-120">None</span></span> | <span data-ttu-id="9fe5f-121">Удаление опубликованного приложения из каталога приложений организации.</span><span class="sxs-lookup"><span data-stu-id="9fe5f-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="9fe5f-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fe5f-122">Properties</span></span>

| <span data-ttu-id="9fe5f-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fe5f-123">Property</span></span>            | <span data-ttu-id="9fe5f-124">Тип</span><span class="sxs-lookup"><span data-stu-id="9fe5f-124">Type</span></span>     | <span data-ttu-id="9fe5f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="9fe5f-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="9fe5f-126">id</span><span class="sxs-lookup"><span data-stu-id="9fe5f-126">id</span></span>                  | <span data-ttu-id="9fe5f-127">string</span><span class="sxs-lookup"><span data-stu-id="9fe5f-127">string</span></span>   | <span data-ttu-id="9fe5f-128">Сгенерированный идентификатор приложения из каталога приложений (отличающийся от предоставленного разработчиком идентификатора в [ZIP-пакете приложения Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="9fe5f-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="9fe5f-129">externalId</span><span class="sxs-lookup"><span data-stu-id="9fe5f-129">externalId</span></span>          | <span data-ttu-id="9fe5f-130">строка</span><span class="sxs-lookup"><span data-stu-id="9fe5f-130">string</span></span>   | <span data-ttu-id="9fe5f-131">Идентификатор каталога, предоставленный разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="9fe5f-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="9fe5f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="9fe5f-132">displayName</span></span>                | <span data-ttu-id="9fe5f-133">string</span><span class="sxs-lookup"><span data-stu-id="9fe5f-133">string</span></span>   | <span data-ttu-id="9fe5f-134">Название приложения каталога, предоставленное разработчиком приложения в [ZIP-пакете приложения Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="9fe5f-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="9fe5f-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="9fe5f-135">distributionMethod</span></span>  | <span data-ttu-id="9fe5f-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="9fe5f-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="9fe5f-137">Метод распространения приложения.</span><span class="sxs-lookup"><span data-stu-id="9fe5f-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="9fe5f-138">Значения teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="9fe5f-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="9fe5f-139">Элемент</span><span class="sxs-lookup"><span data-stu-id="9fe5f-139">Member</span></span>|<span data-ttu-id="9fe5f-140">Значение</span><span class="sxs-lookup"><span data-stu-id="9fe5f-140">Value</span></span>|<span data-ttu-id="9fe5f-141">Описание</span><span class="sxs-lookup"><span data-stu-id="9fe5f-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fe5f-142">store</span><span class="sxs-lookup"><span data-stu-id="9fe5f-142">store</span></span>|<span data-ttu-id="9fe5f-143">0</span><span class="sxs-lookup"><span data-stu-id="9fe5f-143">0</span></span>| <span data-ttu-id="9fe5f-144">Приложение доступно всем клиентам через магазин приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9fe5f-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="9fe5f-145">organization</span><span class="sxs-lookup"><span data-stu-id="9fe5f-145">organization</span></span>|<span data-ttu-id="9fe5f-146">1</span><span class="sxs-lookup"><span data-stu-id="9fe5f-146">1</span></span>|<span data-ttu-id="9fe5f-147">Приложение доступно только в этом клиенте</span><span class="sxs-lookup"><span data-stu-id="9fe5f-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="9fe5f-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="9fe5f-148">sideloaded</span></span>|<span data-ttu-id="9fe5f-149">2</span><span class="sxs-lookup"><span data-stu-id="9fe5f-149">2</span></span>|<span data-ttu-id="9fe5f-150">Приложение доступно только тому пользователю или той команде, где оно установлено.</span><span class="sxs-lookup"><span data-stu-id="9fe5f-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fe5f-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="9fe5f-151">Relationships</span></span>

| <span data-ttu-id="9fe5f-152">Отношение</span><span class="sxs-lookup"><span data-stu-id="9fe5f-152">Relationship</span></span> | <span data-ttu-id="9fe5f-153">Тип</span><span class="sxs-lookup"><span data-stu-id="9fe5f-153">Type</span></span>   | <span data-ttu-id="9fe5f-154">Описание</span><span class="sxs-lookup"><span data-stu-id="9fe5f-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9fe5f-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="9fe5f-155">appDefinitions</span></span>|<span data-ttu-id="9fe5f-156">Коллекция [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9fe5f-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="9fe5f-157">Сведения о каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="9fe5f-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9fe5f-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9fe5f-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="9fe5f-159">См. также</span><span class="sxs-lookup"><span data-stu-id="9fe5f-159">See also</span></span>

- [<span data-ttu-id="9fe5f-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="9fe5f-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="9fe5f-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="9fe5f-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="9fe5f-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9fe5f-162">teamsTab</span></span>](../resources/teamstab.md)

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

