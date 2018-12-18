---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений группами Майкрософт.
author: nkramer
ms.openlocfilehash: b0f3bb42bb90c2c3f0211c5a7092fa7fdb9b10b5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305329"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="bbef7-103">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="bbef7-103">teamsApp resource type</span></span>

> <span data-ttu-id="bbef7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bbef7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbef7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbef7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bbef7-106">Приложение в каталоге приложений [Группами Майкрософт](teams-api-overview.md) .</span><span class="sxs-lookup"><span data-stu-id="bbef7-106">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="bbef7-107">Пользователи могут видеть эти приложения в магазине группами Майкрософт, и эти приложения может быть установлена с [группами](team.md) с помощью метода [Add приложения в группу](../api/teamsappinstallation-add.md) .</span><span class="sxs-lookup"><span data-stu-id="bbef7-107">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="bbef7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="bbef7-108">Methods</span></span>

| <span data-ttu-id="bbef7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="bbef7-109">Method</span></span>       | <span data-ttu-id="bbef7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bbef7-110">Return Type</span></span>  |<span data-ttu-id="bbef7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bbef7-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bbef7-112">Список опубликованных приложений</span><span class="sxs-lookup"><span data-stu-id="bbef7-112">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="bbef7-113">[teamsApp](teamsapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bbef7-113">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="bbef7-114">Список опубликованных приложений из каталога приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bbef7-114">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="bbef7-115">Публикация приложения</span><span class="sxs-lookup"><span data-stu-id="bbef7-115">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="bbef7-116">teamsApp</span><span class="sxs-lookup"><span data-stu-id="bbef7-116">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="bbef7-117">Публикация приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="bbef7-117">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="bbef7-118">Обновление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="bbef7-118">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="bbef7-119">teamsApp</span><span class="sxs-lookup"><span data-stu-id="bbef7-119">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="bbef7-120">Обновление опубликованного приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="bbef7-120">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="bbef7-121">Удаление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="bbef7-121">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="bbef7-122">Нет</span><span class="sxs-lookup"><span data-stu-id="bbef7-122">None</span></span> | <span data-ttu-id="bbef7-123">Удаление опубликованного приложения из каталога приложений вашей организации.</span><span class="sxs-lookup"><span data-stu-id="bbef7-123">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="bbef7-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbef7-124">Properties</span></span>

| <span data-ttu-id="bbef7-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbef7-125">Property</span></span>            | <span data-ttu-id="bbef7-126">Тип</span><span class="sxs-lookup"><span data-stu-id="bbef7-126">Type</span></span>     | <span data-ttu-id="bbef7-127">Описание</span><span class="sxs-lookup"><span data-stu-id="bbef7-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="bbef7-128">id</span><span class="sxs-lookup"><span data-stu-id="bbef7-128">id</span></span>                  | <span data-ttu-id="bbef7-129">строка</span><span class="sxs-lookup"><span data-stu-id="bbef7-129">string</span></span>   | <span data-ttu-id="bbef7-130">Приложения каталога созданный код приложения (отличный от предоставленного для разработчиков ID в [пакет приложения zip группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="bbef7-130">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="bbef7-131">externalId</span><span class="sxs-lookup"><span data-stu-id="bbef7-131">externalId</span></span>          | <span data-ttu-id="bbef7-132">string</span><span class="sxs-lookup"><span data-stu-id="bbef7-132">string</span></span>   | <span data-ttu-id="bbef7-133">Идентификатор каталога, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="bbef7-133">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="bbef7-134">displayName</span><span class="sxs-lookup"><span data-stu-id="bbef7-134">displayName</span></span>                | <span data-ttu-id="bbef7-135">строка</span><span class="sxs-lookup"><span data-stu-id="bbef7-135">string</span></span>   | <span data-ttu-id="bbef7-136">Имя каталога приложения, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="bbef7-136">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="bbef7-137">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="bbef7-137">distributionMethod</span></span>  | <span data-ttu-id="bbef7-138">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="bbef7-138">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="bbef7-139">Метод распространения для приложения.</span><span class="sxs-lookup"><span data-stu-id="bbef7-139">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="bbef7-140">teamsAppDistributionMethod значения</span><span class="sxs-lookup"><span data-stu-id="bbef7-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="bbef7-141">Member</span><span class="sxs-lookup"><span data-stu-id="bbef7-141">Member</span></span>|<span data-ttu-id="bbef7-142">Значение</span><span class="sxs-lookup"><span data-stu-id="bbef7-142">Value</span></span>|<span data-ttu-id="bbef7-143">Описание</span><span class="sxs-lookup"><span data-stu-id="bbef7-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbef7-144">хранилище</span><span class="sxs-lookup"><span data-stu-id="bbef7-144">store</span></span>|<span data-ttu-id="bbef7-145">0</span><span class="sxs-lookup"><span data-stu-id="bbef7-145">0</span></span>| <span data-ttu-id="bbef7-146">Приложение доступно для всех клиентов через хранилище приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bbef7-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="bbef7-147">organization;</span><span class="sxs-lookup"><span data-stu-id="bbef7-147">organization</span></span>|<span data-ttu-id="bbef7-148">1</span><span class="sxs-lookup"><span data-stu-id="bbef7-148">1</span></span>|<span data-ttu-id="bbef7-149">Приложение доступно только при этом клиента.</span><span class="sxs-lookup"><span data-stu-id="bbef7-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="bbef7-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="bbef7-150">sideloaded</span></span>|<span data-ttu-id="bbef7-151">2</span><span class="sxs-lookup"><span data-stu-id="bbef7-151">2</span></span>|<span data-ttu-id="bbef7-152">Приложение будет доступно только для пользователей/групп его установленных для.</span><span class="sxs-lookup"><span data-stu-id="bbef7-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbef7-153">Связи</span><span class="sxs-lookup"><span data-stu-id="bbef7-153">Relationships</span></span>

| <span data-ttu-id="bbef7-154">Связь</span><span class="sxs-lookup"><span data-stu-id="bbef7-154">Relationship</span></span> | <span data-ttu-id="bbef7-155">Тип</span><span class="sxs-lookup"><span data-stu-id="bbef7-155">Type</span></span>   | <span data-ttu-id="bbef7-156">Описание</span><span class="sxs-lookup"><span data-stu-id="bbef7-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bbef7-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="bbef7-157">appDefinitions</span></span>|<span data-ttu-id="bbef7-158">[teamsAppDefinition](teamsappdefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bbef7-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="bbef7-159">Подробные сведения для каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="bbef7-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bbef7-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbef7-160">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="bbef7-161">См. также</span><span class="sxs-lookup"><span data-stu-id="bbef7-161">See also</span></span>

- [<span data-ttu-id="bbef7-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="bbef7-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="bbef7-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="bbef7-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="bbef7-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="bbef7-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

