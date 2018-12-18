---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений группами Майкрософт.
author: nkramer
ms.openlocfilehash: 207974800e44e0db29b8c42f260a1ac16a18902f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359586"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="f8eca-103">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="f8eca-103">teamsApp resource type</span></span>



<span data-ttu-id="f8eca-104">Приложение в каталоге приложений [Группами Майкрософт](teams-api-overview.md) .</span><span class="sxs-lookup"><span data-stu-id="f8eca-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="f8eca-105">Пользователи могут видеть эти приложения в магазине группами Майкрософт, и эти приложения может быть установлена с [группами](team.md) с помощью метода [Add приложения в группу](../api/teamsappinstallation-add.md) .</span><span class="sxs-lookup"><span data-stu-id="f8eca-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="f8eca-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f8eca-106">Methods</span></span>

| <span data-ttu-id="f8eca-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f8eca-107">Method</span></span>       | <span data-ttu-id="f8eca-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f8eca-108">Return Type</span></span>  |<span data-ttu-id="f8eca-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f8eca-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f8eca-110">Список опубликованных приложений</span><span class="sxs-lookup"><span data-stu-id="f8eca-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="f8eca-111">[teamsApp](teamsapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f8eca-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="f8eca-112">Список опубликованных приложений из каталога приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="f8eca-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="f8eca-113">Публикация приложения</span><span class="sxs-lookup"><span data-stu-id="f8eca-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="f8eca-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f8eca-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="f8eca-115">Публикация приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="f8eca-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="f8eca-116">Обновление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="f8eca-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="f8eca-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f8eca-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="f8eca-118">Обновление опубликованного приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="f8eca-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="f8eca-119">Удаление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="f8eca-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="f8eca-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f8eca-120">None</span></span> | <span data-ttu-id="f8eca-121">Удаление опубликованного приложения из каталога приложений вашей организации.</span><span class="sxs-lookup"><span data-stu-id="f8eca-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="f8eca-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8eca-122">Properties</span></span>

| <span data-ttu-id="f8eca-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8eca-123">Property</span></span>            | <span data-ttu-id="f8eca-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f8eca-124">Type</span></span>     | <span data-ttu-id="f8eca-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f8eca-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="f8eca-126">id</span><span class="sxs-lookup"><span data-stu-id="f8eca-126">id</span></span>                  | <span data-ttu-id="f8eca-127">строка</span><span class="sxs-lookup"><span data-stu-id="f8eca-127">string</span></span>   | <span data-ttu-id="f8eca-128">Приложения каталога созданный код приложения (отличный от предоставленного для разработчиков ID в [пакет приложения zip группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="f8eca-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="f8eca-129">externalId</span><span class="sxs-lookup"><span data-stu-id="f8eca-129">externalId</span></span>          | <span data-ttu-id="f8eca-130">string</span><span class="sxs-lookup"><span data-stu-id="f8eca-130">string</span></span>   | <span data-ttu-id="f8eca-131">Идентификатор каталога, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="f8eca-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="f8eca-132">displayName</span><span class="sxs-lookup"><span data-stu-id="f8eca-132">displayName</span></span>                | <span data-ttu-id="f8eca-133">строка</span><span class="sxs-lookup"><span data-stu-id="f8eca-133">string</span></span>   | <span data-ttu-id="f8eca-134">Имя каталога приложения, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="f8eca-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="f8eca-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="f8eca-135">distributionMethod</span></span>  | <span data-ttu-id="f8eca-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="f8eca-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="f8eca-137">Метод распространения для приложения.</span><span class="sxs-lookup"><span data-stu-id="f8eca-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="f8eca-138">teamsAppDistributionMethod значения</span><span class="sxs-lookup"><span data-stu-id="f8eca-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="f8eca-139">Member</span><span class="sxs-lookup"><span data-stu-id="f8eca-139">Member</span></span>|<span data-ttu-id="f8eca-140">Значение</span><span class="sxs-lookup"><span data-stu-id="f8eca-140">Value</span></span>|<span data-ttu-id="f8eca-141">Описание</span><span class="sxs-lookup"><span data-stu-id="f8eca-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8eca-142">хранилище</span><span class="sxs-lookup"><span data-stu-id="f8eca-142">store</span></span>|<span data-ttu-id="f8eca-143">0</span><span class="sxs-lookup"><span data-stu-id="f8eca-143">0</span></span>| <span data-ttu-id="f8eca-144">Приложение доступно для всех клиентов через хранилище приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="f8eca-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="f8eca-145">organization;</span><span class="sxs-lookup"><span data-stu-id="f8eca-145">organization</span></span>|<span data-ttu-id="f8eca-146">1</span><span class="sxs-lookup"><span data-stu-id="f8eca-146">1</span></span>|<span data-ttu-id="f8eca-147">Приложение доступно только при этом клиента.</span><span class="sxs-lookup"><span data-stu-id="f8eca-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="f8eca-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="f8eca-148">sideloaded</span></span>|<span data-ttu-id="f8eca-149">2</span><span class="sxs-lookup"><span data-stu-id="f8eca-149">2</span></span>|<span data-ttu-id="f8eca-150">Приложение будет доступно только для пользователей/групп его установленных для.</span><span class="sxs-lookup"><span data-stu-id="f8eca-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8eca-151">Связи</span><span class="sxs-lookup"><span data-stu-id="f8eca-151">Relationships</span></span>

| <span data-ttu-id="f8eca-152">Связь</span><span class="sxs-lookup"><span data-stu-id="f8eca-152">Relationship</span></span> | <span data-ttu-id="f8eca-153">Тип</span><span class="sxs-lookup"><span data-stu-id="f8eca-153">Type</span></span>   | <span data-ttu-id="f8eca-154">Описание</span><span class="sxs-lookup"><span data-stu-id="f8eca-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f8eca-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="f8eca-155">appDefinitions</span></span>|<span data-ttu-id="f8eca-156">[teamsAppDefinition](teamsappdefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f8eca-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="f8eca-157">Подробные сведения для каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="f8eca-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f8eca-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8eca-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="f8eca-159">См. также</span><span class="sxs-lookup"><span data-stu-id="f8eca-159">See also</span></span>

- [<span data-ttu-id="f8eca-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f8eca-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="f8eca-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="f8eca-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="f8eca-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="f8eca-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

