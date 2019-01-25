---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений группами Майкрософт.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe60222ae6c5d8475722e18e69555df2d3892759
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529945"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="b50b2-103">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="b50b2-103">teamsApp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b50b2-104">Приложение в каталоге приложений [Группами Майкрософт](teams-api-overview.md) .</span><span class="sxs-lookup"><span data-stu-id="b50b2-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="b50b2-105">Пользователи могут видеть эти приложения в магазине группами Майкрософт, и эти приложения может быть установлена с [группами](team.md) с помощью метода [Add приложения в группу](../api/teamsappinstallation-add.md) .</span><span class="sxs-lookup"><span data-stu-id="b50b2-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="b50b2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b50b2-106">Methods</span></span>

| <span data-ttu-id="b50b2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b50b2-107">Method</span></span>       | <span data-ttu-id="b50b2-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b50b2-108">Return Type</span></span>  |<span data-ttu-id="b50b2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b50b2-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b50b2-110">Список опубликованных приложений</span><span class="sxs-lookup"><span data-stu-id="b50b2-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="b50b2-111">[teamsApp](teamsapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b50b2-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="b50b2-112">Список опубликованных приложений из каталога приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b50b2-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="b50b2-113">Публикация приложения</span><span class="sxs-lookup"><span data-stu-id="b50b2-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="b50b2-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b50b2-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="b50b2-115">Публикация приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="b50b2-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="b50b2-116">Обновление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="b50b2-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="b50b2-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b50b2-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="b50b2-118">Обновление опубликованного приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="b50b2-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="b50b2-119">Удаление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="b50b2-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="b50b2-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b50b2-120">None</span></span> | <span data-ttu-id="b50b2-121">Удаление опубликованного приложения из каталога приложений вашей организации.</span><span class="sxs-lookup"><span data-stu-id="b50b2-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="b50b2-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="b50b2-122">Properties</span></span>

| <span data-ttu-id="b50b2-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="b50b2-123">Property</span></span>            | <span data-ttu-id="b50b2-124">Тип</span><span class="sxs-lookup"><span data-stu-id="b50b2-124">Type</span></span>     | <span data-ttu-id="b50b2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b50b2-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="b50b2-126">id</span><span class="sxs-lookup"><span data-stu-id="b50b2-126">id</span></span>                  | <span data-ttu-id="b50b2-127">string</span><span class="sxs-lookup"><span data-stu-id="b50b2-127">string</span></span>   | <span data-ttu-id="b50b2-128">Приложения каталога созданный код приложения (отличный от предоставленного для разработчиков ID в [пакет приложения zip группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="b50b2-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="b50b2-129">externalId</span><span class="sxs-lookup"><span data-stu-id="b50b2-129">externalId</span></span>          | <span data-ttu-id="b50b2-130">string</span><span class="sxs-lookup"><span data-stu-id="b50b2-130">string</span></span>   | <span data-ttu-id="b50b2-131">Идентификатор каталога, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="b50b2-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="b50b2-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b50b2-132">displayName</span></span>                | <span data-ttu-id="b50b2-133">строка</span><span class="sxs-lookup"><span data-stu-id="b50b2-133">string</span></span>   | <span data-ttu-id="b50b2-134">Имя каталога приложения, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="b50b2-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="b50b2-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="b50b2-135">distributionMethod</span></span>  | <span data-ttu-id="b50b2-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="b50b2-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="b50b2-137">Метод распространения для приложения.</span><span class="sxs-lookup"><span data-stu-id="b50b2-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="b50b2-138">teamsAppDistributionMethod значения</span><span class="sxs-lookup"><span data-stu-id="b50b2-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="b50b2-139">Member</span><span class="sxs-lookup"><span data-stu-id="b50b2-139">Member</span></span>|<span data-ttu-id="b50b2-140">Значение</span><span class="sxs-lookup"><span data-stu-id="b50b2-140">Value</span></span>|<span data-ttu-id="b50b2-141">Описание</span><span class="sxs-lookup"><span data-stu-id="b50b2-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b50b2-142">Store</span><span class="sxs-lookup"><span data-stu-id="b50b2-142">store</span></span>|<span data-ttu-id="b50b2-143">(0)</span><span class="sxs-lookup"><span data-stu-id="b50b2-143">0</span></span>| <span data-ttu-id="b50b2-144">Приложение доступно для всех клиентов через хранилище приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b50b2-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="b50b2-145">organization;</span><span class="sxs-lookup"><span data-stu-id="b50b2-145">organization</span></span>|<span data-ttu-id="b50b2-146">$1</span><span class="sxs-lookup"><span data-stu-id="b50b2-146">1</span></span>|<span data-ttu-id="b50b2-147">Приложение доступно только при этом клиента.</span><span class="sxs-lookup"><span data-stu-id="b50b2-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="b50b2-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="b50b2-148">sideloaded</span></span>|<span data-ttu-id="b50b2-149">–2</span><span class="sxs-lookup"><span data-stu-id="b50b2-149">2</span></span>|<span data-ttu-id="b50b2-150">Приложение будет доступно только для пользователей/групп его установленных для.</span><span class="sxs-lookup"><span data-stu-id="b50b2-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b50b2-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="b50b2-151">Relationships</span></span>

| <span data-ttu-id="b50b2-152">Связь</span><span class="sxs-lookup"><span data-stu-id="b50b2-152">Relationship</span></span> | <span data-ttu-id="b50b2-153">Тип</span><span class="sxs-lookup"><span data-stu-id="b50b2-153">Type</span></span>   | <span data-ttu-id="b50b2-154">object</span><span class="sxs-lookup"><span data-stu-id="b50b2-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b50b2-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="b50b2-155">appDefinitions</span></span>|<span data-ttu-id="b50b2-156">[teamsAppDefinition](teamsappdefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b50b2-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="b50b2-157">Подробные сведения для каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="b50b2-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b50b2-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b50b2-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="b50b2-159">См. также</span><span class="sxs-lookup"><span data-stu-id="b50b2-159">See also</span></span>

- [<span data-ttu-id="b50b2-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b50b2-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="b50b2-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="b50b2-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="b50b2-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b50b2-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsapp.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

