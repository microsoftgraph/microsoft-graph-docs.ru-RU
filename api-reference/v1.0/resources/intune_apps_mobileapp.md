# <a name="mobileapp-resource-type"></a><span data-ttu-id="9a392-101">Тип ресурса mobileApp</span><span class="sxs-lookup"><span data-stu-id="9a392-101">mobileApp resource type</span></span>

> <span data-ttu-id="9a392-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9a392-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a392-103">Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="9a392-103">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="9a392-104">Методы</span><span class="sxs-lookup"><span data-stu-id="9a392-104">Methods</span></span>
|<span data-ttu-id="9a392-105">Метод</span><span class="sxs-lookup"><span data-stu-id="9a392-105">Method</span></span>|<span data-ttu-id="9a392-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9a392-106">Return Type</span></span>|<span data-ttu-id="9a392-107">Описание</span><span class="sxs-lookup"><span data-stu-id="9a392-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9a392-108">Список mobileApps</span><span class="sxs-lookup"><span data-stu-id="9a392-108">List mobileApps</span></span>](../api/intune_apps_mobileapp_list.md)|<span data-ttu-id="9a392-109">Коллекция [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a392-109">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="9a392-110">Список свойств и связей объектов [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a392-110">List properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="9a392-111">Получение объекта mobileApp</span><span class="sxs-lookup"><span data-stu-id="9a392-111">Get mobileApp</span></span>](../api/intune_apps_mobileapp_get.md)|[<span data-ttu-id="9a392-112">mobileApp</span><span class="sxs-lookup"><span data-stu-id="9a392-112">mobileApp</span></span>](../resources/intune_apps_mobileapp.md)|<span data-ttu-id="9a392-113">Чтение свойств и связей объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a392-113">Read properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) object.</span></span>|
|[<span data-ttu-id="9a392-114">assign action</span><span class="sxs-lookup"><span data-stu-id="9a392-114">assign action</span></span>](../api/intune_apps_mobileapp_assign.md)|<span data-ttu-id="9a392-115">Нет</span><span class="sxs-lookup"><span data-stu-id="9a392-115">None</span></span>|<span data-ttu-id="9a392-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9a392-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9a392-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a392-117">Properties</span></span>
|<span data-ttu-id="9a392-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a392-118">Property</span></span>|<span data-ttu-id="9a392-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9a392-119">Type</span></span>|<span data-ttu-id="9a392-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9a392-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a392-121">id</span><span class="sxs-lookup"><span data-stu-id="9a392-121">id</span></span>|<span data-ttu-id="9a392-122">String</span><span class="sxs-lookup"><span data-stu-id="9a392-122">String</span></span>|<span data-ttu-id="9a392-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9a392-123">Key of the entity.</span></span>|
|<span data-ttu-id="9a392-124">displayName</span><span class="sxs-lookup"><span data-stu-id="9a392-124">displayName</span></span>|<span data-ttu-id="9a392-125">String</span><span class="sxs-lookup"><span data-stu-id="9a392-125">String</span></span>|<span data-ttu-id="9a392-126">Администратор предоставил или импортировал название приложения.</span><span class="sxs-lookup"><span data-stu-id="9a392-126">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="9a392-127">description</span><span class="sxs-lookup"><span data-stu-id="9a392-127">description</span></span>|<span data-ttu-id="9a392-128">String</span><span class="sxs-lookup"><span data-stu-id="9a392-128">String</span></span>|<span data-ttu-id="9a392-129">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9a392-129">The description of the app.</span></span>|
|<span data-ttu-id="9a392-130">publisher</span><span class="sxs-lookup"><span data-stu-id="9a392-130">publisher</span></span>|<span data-ttu-id="9a392-131">String</span><span class="sxs-lookup"><span data-stu-id="9a392-131">String</span></span>|<span data-ttu-id="9a392-132">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9a392-132">The publisher of the app.</span></span>|
|<span data-ttu-id="9a392-133">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9a392-133">largeIcon</span></span>|[<span data-ttu-id="9a392-134">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9a392-134">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="9a392-135">Большой значок, отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9a392-135">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="9a392-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a392-136">createdDateTime</span></span>|<span data-ttu-id="9a392-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a392-137">DateTimeOffset</span></span>|<span data-ttu-id="9a392-138">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9a392-138">The date and time the app was created.</span></span>|
|<span data-ttu-id="9a392-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a392-139">lastModifiedDateTime</span></span>|<span data-ttu-id="9a392-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a392-140">DateTimeOffset</span></span>|<span data-ttu-id="9a392-141">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9a392-141">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="9a392-142">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9a392-142">isFeatured</span></span>|<span data-ttu-id="9a392-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a392-143">Boolean</span></span>|<span data-ttu-id="9a392-144">Значение, которое показывает, отмечено ли приложение как подобранное администратором.</span><span class="sxs-lookup"><span data-stu-id="9a392-144">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="9a392-145">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9a392-145">privacyInformationUrl</span></span>|<span data-ttu-id="9a392-146">String</span><span class="sxs-lookup"><span data-stu-id="9a392-146">String</span></span>|<span data-ttu-id="9a392-147">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9a392-147">The privacy statement Url.</span></span>|
|<span data-ttu-id="9a392-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9a392-148">informationUrl</span></span>|<span data-ttu-id="9a392-149">String</span><span class="sxs-lookup"><span data-stu-id="9a392-149">String</span></span>|<span data-ttu-id="9a392-150">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9a392-150">The more information Url.</span></span>|
|<span data-ttu-id="9a392-151">owner</span><span class="sxs-lookup"><span data-stu-id="9a392-151">owner</span></span>|<span data-ttu-id="9a392-152">String</span><span class="sxs-lookup"><span data-stu-id="9a392-152">String</span></span>|<span data-ttu-id="9a392-153">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9a392-153">The owner of the app.</span></span>|
|<span data-ttu-id="9a392-154">developer</span><span class="sxs-lookup"><span data-stu-id="9a392-154">developer</span></span>|<span data-ttu-id="9a392-155">String</span><span class="sxs-lookup"><span data-stu-id="9a392-155">String</span></span>|<span data-ttu-id="9a392-156">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9a392-156">The developer of the app.</span></span>|
|<span data-ttu-id="9a392-157">notes</span><span class="sxs-lookup"><span data-stu-id="9a392-157">notes</span></span>|<span data-ttu-id="9a392-158">String</span><span class="sxs-lookup"><span data-stu-id="9a392-158">String</span></span>|<span data-ttu-id="9a392-159">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9a392-159">Notes for the app.</span></span>|
|<span data-ttu-id="9a392-160">publishingState</span><span class="sxs-lookup"><span data-stu-id="9a392-160">publishingState</span></span>|[<span data-ttu-id="9a392-161">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9a392-161">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="9a392-162">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="9a392-162">The publishing state for the app.</span></span> <span data-ttu-id="9a392-163">Приложение не может быть назначено, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9a392-163">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9a392-164">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9a392-164">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a392-165">Связи</span><span class="sxs-lookup"><span data-stu-id="9a392-165">Relationships</span></span>
|<span data-ttu-id="9a392-166">Связь</span><span class="sxs-lookup"><span data-stu-id="9a392-166">Relationship</span></span>|<span data-ttu-id="9a392-167">Тип</span><span class="sxs-lookup"><span data-stu-id="9a392-167">Type</span></span>|<span data-ttu-id="9a392-168">Описание</span><span class="sxs-lookup"><span data-stu-id="9a392-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a392-169">categories</span><span class="sxs-lookup"><span data-stu-id="9a392-169">categories</span></span>|<span data-ttu-id="9a392-170">Коллекция [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="9a392-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="9a392-171">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="9a392-171">The list of categories for this app.</span></span>|
|<span data-ttu-id="9a392-172">assignments</span><span class="sxs-lookup"><span data-stu-id="9a392-172">assignments</span></span>|<span data-ttu-id="9a392-173">Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9a392-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="9a392-174">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9a392-174">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a392-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a392-175">JSON Representation</span></span>
<span data-ttu-id="9a392-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a392-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String"
}
```



