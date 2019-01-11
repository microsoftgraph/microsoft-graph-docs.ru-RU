---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений группами Майкрософт.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: b02af5148e40cddd6079de3479767110a9877e4f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841575"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="5e254-103">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="5e254-103">teamsApp resource type</span></span>

> <span data-ttu-id="5e254-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e254-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e254-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e254-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e254-106">Приложение в каталоге приложений [Группами Майкрософт](teams-api-overview.md) .</span><span class="sxs-lookup"><span data-stu-id="5e254-106">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="5e254-107">Пользователи могут видеть эти приложения в магазине группами Майкрософт, и эти приложения может быть установлена с [группами](team.md) с помощью метода [Add приложения в группу](../api/teamsappinstallation-add.md) .</span><span class="sxs-lookup"><span data-stu-id="5e254-107">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="5e254-108">Методы</span><span class="sxs-lookup"><span data-stu-id="5e254-108">Methods</span></span>

| <span data-ttu-id="5e254-109">Метод</span><span class="sxs-lookup"><span data-stu-id="5e254-109">Method</span></span>       | <span data-ttu-id="5e254-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e254-110">Return Type</span></span>  |<span data-ttu-id="5e254-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5e254-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e254-112">Список опубликованных приложений</span><span class="sxs-lookup"><span data-stu-id="5e254-112">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="5e254-113">[teamsApp](teamsapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5e254-113">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="5e254-114">Список опубликованных приложений из каталога приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5e254-114">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="5e254-115">Публикация приложения</span><span class="sxs-lookup"><span data-stu-id="5e254-115">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="5e254-116">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5e254-116">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="5e254-117">Публикация приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="5e254-117">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="5e254-118">Обновление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="5e254-118">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="5e254-119">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5e254-119">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="5e254-120">Обновление опубликованного приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="5e254-120">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="5e254-121">Удаление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="5e254-121">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="5e254-122">Нет</span><span class="sxs-lookup"><span data-stu-id="5e254-122">None</span></span> | <span data-ttu-id="5e254-123">Удаление опубликованного приложения из каталога приложений вашей организации.</span><span class="sxs-lookup"><span data-stu-id="5e254-123">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e254-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e254-124">Properties</span></span>

| <span data-ttu-id="5e254-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e254-125">Property</span></span>            | <span data-ttu-id="5e254-126">Тип</span><span class="sxs-lookup"><span data-stu-id="5e254-126">Type</span></span>     | <span data-ttu-id="5e254-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5e254-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="5e254-128">id</span><span class="sxs-lookup"><span data-stu-id="5e254-128">id</span></span>                  | <span data-ttu-id="5e254-129">строка</span><span class="sxs-lookup"><span data-stu-id="5e254-129">string</span></span>   | <span data-ttu-id="5e254-130">Приложения каталога созданный код приложения (отличный от предоставленного для разработчиков ID в [пакет приложения zip группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="5e254-130">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="5e254-131">externalId</span><span class="sxs-lookup"><span data-stu-id="5e254-131">externalId</span></span>          | <span data-ttu-id="5e254-132">string</span><span class="sxs-lookup"><span data-stu-id="5e254-132">string</span></span>   | <span data-ttu-id="5e254-133">Идентификатор каталога, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="5e254-133">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="5e254-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5e254-134">displayName</span></span>                | <span data-ttu-id="5e254-135">строка</span><span class="sxs-lookup"><span data-stu-id="5e254-135">string</span></span>   | <span data-ttu-id="5e254-136">Имя каталога приложения, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="5e254-136">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="5e254-137">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="5e254-137">distributionMethod</span></span>  | <span data-ttu-id="5e254-138">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="5e254-138">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="5e254-139">Метод распространения для приложения.</span><span class="sxs-lookup"><span data-stu-id="5e254-139">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="5e254-140">teamsAppDistributionMethod значения</span><span class="sxs-lookup"><span data-stu-id="5e254-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="5e254-141">Член</span><span class="sxs-lookup"><span data-stu-id="5e254-141">Member</span></span>|<span data-ttu-id="5e254-142">Значение</span><span class="sxs-lookup"><span data-stu-id="5e254-142">Value</span></span>|<span data-ttu-id="5e254-143">Описание</span><span class="sxs-lookup"><span data-stu-id="5e254-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e254-144">хранилище</span><span class="sxs-lookup"><span data-stu-id="5e254-144">store</span></span>|<span data-ttu-id="5e254-145">0</span><span class="sxs-lookup"><span data-stu-id="5e254-145">0</span></span>| <span data-ttu-id="5e254-146">Приложение доступно для всех клиентов через хранилище приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5e254-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="5e254-147">organization;</span><span class="sxs-lookup"><span data-stu-id="5e254-147">organization</span></span>|<span data-ttu-id="5e254-148">1</span><span class="sxs-lookup"><span data-stu-id="5e254-148">1</span></span>|<span data-ttu-id="5e254-149">Приложение доступно только при этом клиента.</span><span class="sxs-lookup"><span data-stu-id="5e254-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="5e254-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="5e254-150">sideloaded</span></span>|<span data-ttu-id="5e254-151">2</span><span class="sxs-lookup"><span data-stu-id="5e254-151">2</span></span>|<span data-ttu-id="5e254-152">Приложение будет доступно только для пользователей/групп его установленных для.</span><span class="sxs-lookup"><span data-stu-id="5e254-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e254-153">Связи</span><span class="sxs-lookup"><span data-stu-id="5e254-153">Relationships</span></span>

| <span data-ttu-id="5e254-154">Связь</span><span class="sxs-lookup"><span data-stu-id="5e254-154">Relationship</span></span> | <span data-ttu-id="5e254-155">Тип</span><span class="sxs-lookup"><span data-stu-id="5e254-155">Type</span></span>   | <span data-ttu-id="5e254-156">Описание</span><span class="sxs-lookup"><span data-stu-id="5e254-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5e254-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="5e254-157">appDefinitions</span></span>|<span data-ttu-id="5e254-158">[teamsAppDefinition](teamsappdefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5e254-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="5e254-159">Подробные сведения для каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="5e254-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5e254-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e254-160">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="5e254-161">См. также</span><span class="sxs-lookup"><span data-stu-id="5e254-161">See also</span></span>

- [<span data-ttu-id="5e254-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="5e254-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="5e254-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="5e254-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="5e254-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5e254-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

