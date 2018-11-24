# <a name="teamsapp-resource-type"></a><span data-ttu-id="f1421-101">Тип ресурса teamsApp</span><span class="sxs-lookup"><span data-stu-id="f1421-101">teamsApp resource type</span></span>



<span data-ttu-id="f1421-102">Приложение в каталоге приложений [Группами Майкрософт](teams_api_overview.md) .</span><span class="sxs-lookup"><span data-stu-id="f1421-102">An app in the [Microsoft Teams](teams_api_overview.md) app catalog.</span></span>

<span data-ttu-id="f1421-103">Пользователи могут видеть эти приложения в магазине группами Майкрософт, и эти приложения может быть установлена с [группами](team.md) с помощью метода [Add приложения в группу](../api/teamsappinstallation_add.md) .</span><span class="sxs-lookup"><span data-stu-id="f1421-103">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation_add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="f1421-104">Методы</span><span class="sxs-lookup"><span data-stu-id="f1421-104">Methods</span></span>

| <span data-ttu-id="f1421-105">Метод</span><span class="sxs-lookup"><span data-stu-id="f1421-105">Method</span></span>       | <span data-ttu-id="f1421-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f1421-106">Return Type</span></span>  |<span data-ttu-id="f1421-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f1421-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f1421-108">Список опубликованных приложений</span><span class="sxs-lookup"><span data-stu-id="f1421-108">List published apps</span></span>](../api/teamsapp_list.md) | <span data-ttu-id="f1421-109">[teamsApp](teamsApp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f1421-109">[teamsApp](teamsApp.md) collection</span></span> | <span data-ttu-id="f1421-110">Список опубликованных приложений из каталога приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="f1421-110">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="f1421-111">Публикация приложения</span><span class="sxs-lookup"><span data-stu-id="f1421-111">Publish an app</span></span>](../api/teamsapp_publish.md) | [<span data-ttu-id="f1421-112">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f1421-112">teamsApp</span></span>](teamsApp.md) | <span data-ttu-id="f1421-113">Публикация приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="f1421-113">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="f1421-114">Обновление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="f1421-114">Update a published app</span></span>](../api/teamsapp_update.md) | [<span data-ttu-id="f1421-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f1421-115">teamsApp</span></span>](teamsApp.md) | <span data-ttu-id="f1421-116">Обновление опубликованного приложения в каталоге приложений организации.</span><span class="sxs-lookup"><span data-stu-id="f1421-116">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="f1421-117">Удаление опубликованного приложения</span><span class="sxs-lookup"><span data-stu-id="f1421-117">Remove a published app</span></span>](../api/teamsapp_delete.md) | <span data-ttu-id="f1421-118">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="f1421-118">None</span></span> | <span data-ttu-id="f1421-119">Удаление опубликованного приложения из каталога приложений вашей организации.</span><span class="sxs-lookup"><span data-stu-id="f1421-119">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="f1421-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1421-120">Properties</span></span>

| <span data-ttu-id="f1421-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1421-121">Property</span></span>            | <span data-ttu-id="f1421-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f1421-122">Type</span></span>     | <span data-ttu-id="f1421-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f1421-123">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="f1421-124">id</span><span class="sxs-lookup"><span data-stu-id="f1421-124">id</span></span>                  | <span data-ttu-id="f1421-125">строка</span><span class="sxs-lookup"><span data-stu-id="f1421-125">string</span></span>   | <span data-ttu-id="f1421-126">Приложения каталога созданный код приложения (отличный от предоставленного для разработчиков ID в [пакет приложения zip группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="f1421-126">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="f1421-127">externalId</span><span class="sxs-lookup"><span data-stu-id="f1421-127">externalId</span></span>          | <span data-ttu-id="f1421-128">string</span><span class="sxs-lookup"><span data-stu-id="f1421-128">string</span></span>   | <span data-ttu-id="f1421-129">Идентификатор каталога, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="f1421-129">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="f1421-130">displayName</span><span class="sxs-lookup"><span data-stu-id="f1421-130">displayName</span></span>                | <span data-ttu-id="f1421-131">строка</span><span class="sxs-lookup"><span data-stu-id="f1421-131">string</span></span>   | <span data-ttu-id="f1421-132">Имя каталога приложения, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="f1421-132">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="f1421-133">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="f1421-133">distributionMethod</span></span>  | <span data-ttu-id="f1421-134">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="f1421-134">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="f1421-135">Метод распространения для приложения.</span><span class="sxs-lookup"><span data-stu-id="f1421-135">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="f1421-136">teamsAppDistributionMethod значения</span><span class="sxs-lookup"><span data-stu-id="f1421-136">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="f1421-137">Элемент</span><span class="sxs-lookup"><span data-stu-id="f1421-137">Member</span></span>|<span data-ttu-id="f1421-138">Значение</span><span class="sxs-lookup"><span data-stu-id="f1421-138">Value</span></span>|<span data-ttu-id="f1421-139">Описание</span><span class="sxs-lookup"><span data-stu-id="f1421-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1421-140">хранилище</span><span class="sxs-lookup"><span data-stu-id="f1421-140">store</span></span>|<span data-ttu-id="f1421-141">0</span><span class="sxs-lookup"><span data-stu-id="f1421-141">0</span></span>| <span data-ttu-id="f1421-142">Приложение доступно для всех клиентов через хранилище приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="f1421-142">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="f1421-143">organization;</span><span class="sxs-lookup"><span data-stu-id="f1421-143">organization</span></span>|<span data-ttu-id="f1421-144">1</span><span class="sxs-lookup"><span data-stu-id="f1421-144">1</span></span>|<span data-ttu-id="f1421-145">Приложение доступно только при этом клиента.</span><span class="sxs-lookup"><span data-stu-id="f1421-145">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="f1421-146">sideloaded</span><span class="sxs-lookup"><span data-stu-id="f1421-146">sideloaded</span></span>|<span data-ttu-id="f1421-147">2</span><span class="sxs-lookup"><span data-stu-id="f1421-147">2</span></span>|<span data-ttu-id="f1421-148">Приложение будет доступно только для пользователей/групп его установленных для.</span><span class="sxs-lookup"><span data-stu-id="f1421-148">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1421-149">Связи</span><span class="sxs-lookup"><span data-stu-id="f1421-149">Relationships</span></span>

| <span data-ttu-id="f1421-150">Связь</span><span class="sxs-lookup"><span data-stu-id="f1421-150">Relationship</span></span> | <span data-ttu-id="f1421-151">Тип</span><span class="sxs-lookup"><span data-stu-id="f1421-151">Type</span></span>   | <span data-ttu-id="f1421-152">Описание</span><span class="sxs-lookup"><span data-stu-id="f1421-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f1421-153">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="f1421-153">appDefinitions</span></span>|<span data-ttu-id="f1421-154">[teamsAppDefinition](teamsappdefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f1421-154">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="f1421-155">Подробные сведения для каждой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="f1421-155">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1421-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1421-156">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="f1421-157">См. также</span><span class="sxs-lookup"><span data-stu-id="f1421-157">See also</span></span>

- [<span data-ttu-id="f1421-158">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f1421-158">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="f1421-159">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="f1421-159">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="f1421-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="f1421-160">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

