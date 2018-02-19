# <a name="mobileapp-resource-type"></a><span data-ttu-id="aaab7-101">Тип ресурса mobileApp</span><span class="sxs-lookup"><span data-stu-id="aaab7-101">mobileApp resource type</span></span>

> <span data-ttu-id="aaab7-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aaab7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aaab7-103">Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="aaab7-103">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="aaab7-104">Методы</span><span class="sxs-lookup"><span data-stu-id="aaab7-104">Methods</span></span>
|<span data-ttu-id="aaab7-105">Метод</span><span class="sxs-lookup"><span data-stu-id="aaab7-105">Method</span></span>|<span data-ttu-id="aaab7-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aaab7-106">Return Type</span></span>|<span data-ttu-id="aaab7-107">Описание</span><span class="sxs-lookup"><span data-stu-id="aaab7-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aaab7-108">Список mobileApps</span><span class="sxs-lookup"><span data-stu-id="aaab7-108">List mobileApps</span></span>](../api/intune_apps_mobileapp_list.md)|<span data-ttu-id="aaab7-109">Коллекция [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aaab7-109">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="aaab7-110">Список свойств и связей объектов [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aaab7-110">List properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="aaab7-111">Получение объекта mobileApp</span><span class="sxs-lookup"><span data-stu-id="aaab7-111">Get mobileApp</span></span>](../api/intune_apps_mobileapp_get.md)|[<span data-ttu-id="aaab7-112">mobileApp</span><span class="sxs-lookup"><span data-stu-id="aaab7-112">mobileApp</span></span>](../resources/intune_apps_mobileapp.md)|<span data-ttu-id="aaab7-113">Чтение свойств и связей объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aaab7-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_mobileapp.md) object.</span></span>|
|[<span data-ttu-id="aaab7-114">assign action</span><span class="sxs-lookup"><span data-stu-id="aaab7-114">assign action</span></span>](../api/intune_apps_mobileapp_assign.md)|<span data-ttu-id="aaab7-115">Нет</span><span class="sxs-lookup"><span data-stu-id="aaab7-115">None</span></span>|<span data-ttu-id="aaab7-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="aaab7-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="aaab7-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="aaab7-117">Properties</span></span>
|<span data-ttu-id="aaab7-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="aaab7-118">Property</span></span>|<span data-ttu-id="aaab7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="aaab7-119">Type</span></span>|<span data-ttu-id="aaab7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aaab7-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaab7-121">id</span><span class="sxs-lookup"><span data-stu-id="aaab7-121">id</span></span>|<span data-ttu-id="aaab7-122">String</span><span class="sxs-lookup"><span data-stu-id="aaab7-122">String</span></span>|<span data-ttu-id="aaab7-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aaab7-123">Key of the setting.</span></span>|
|<span data-ttu-id="aaab7-124">displayName</span><span class="sxs-lookup"><span data-stu-id="aaab7-124">displayName</span></span>|<span data-ttu-id="aaab7-125">String</span><span class="sxs-lookup"><span data-stu-id="aaab7-125">String</span></span>|<span data-ttu-id="aaab7-126">Администратор предоставил или импортировал название приложения.</span><span class="sxs-lookup"><span data-stu-id="aaab7-126">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="aaab7-127">description</span><span class="sxs-lookup"><span data-stu-id="aaab7-127">description</span></span>|<span data-ttu-id="aaab7-128">String</span><span class="sxs-lookup"><span data-stu-id="aaab7-128">String</span></span>|<span data-ttu-id="aaab7-129">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="aaab7-129">The description of the app.</span></span>|
|<span data-ttu-id="aaab7-130">publisher</span><span class="sxs-lookup"><span data-stu-id="aaab7-130">Publisher</span></span>|<span data-ttu-id="aaab7-131">String</span><span class="sxs-lookup"><span data-stu-id="aaab7-131">String</span></span>|<span data-ttu-id="aaab7-132">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="aaab7-132">The name of the app.</span></span>|
|<span data-ttu-id="aaab7-133">largeIcon</span><span class="sxs-lookup"><span data-stu-id="aaab7-133">largeIcon</span></span>|[<span data-ttu-id="aaab7-134">mimeContent</span><span class="sxs-lookup"><span data-stu-id="aaab7-134">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="aaab7-135">Большой значок, отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="aaab7-135">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="aaab7-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aaab7-136">createdDateTime</span></span>|<span data-ttu-id="aaab7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaab7-137">DateTimeOffset</span></span>|<span data-ttu-id="aaab7-138">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="aaab7-138">The date and time the group was created.</span></span>|
|<span data-ttu-id="aaab7-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aaab7-139">lastModifiedDateTime</span></span>|<span data-ttu-id="aaab7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaab7-140">DateTimeOffset</span></span>|<span data-ttu-id="aaab7-141">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="aaab7-141">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="aaab7-142">isFeatured</span><span class="sxs-lookup"><span data-stu-id="aaab7-142">isFeatured</span></span>|<span data-ttu-id="aaab7-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="aaab7-143">Boolean</span></span>|<span data-ttu-id="aaab7-144">Значение, которое показывает, отмечено ли приложение как подобранное администратором.</span><span class="sxs-lookup"><span data-stu-id="aaab7-144">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="aaab7-145">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="aaab7-145">privacyInformationUrl</span></span>|<span data-ttu-id="aaab7-146">String</span><span class="sxs-lookup"><span data-stu-id="aaab7-146">String</span></span>|<span data-ttu-id="aaab7-147">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="aaab7-147">The privacy statement Url.</span></span>|
|<span data-ttu-id="aaab7-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="aaab7-148">informationUrl</span></span>|<span data-ttu-id="aaab7-149">String</span><span class="sxs-lookup"><span data-stu-id="aaab7-149">String</span></span>|<span data-ttu-id="aaab7-150">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="aaab7-150">The more information Url.</span></span>|
|<span data-ttu-id="aaab7-151">owner</span><span class="sxs-lookup"><span data-stu-id="aaab7-151">owner</span></span>|<span data-ttu-id="aaab7-152">String</span><span class="sxs-lookup"><span data-stu-id="aaab7-152">String</span></span>|<span data-ttu-id="aaab7-153">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="aaab7-153">The owner of the app.</span></span>|
|<span data-ttu-id="aaab7-154">developer</span><span class="sxs-lookup"><span data-stu-id="aaab7-154">developer</span></span>|<span data-ttu-id="aaab7-155">String</span><span class="sxs-lookup"><span data-stu-id="aaab7-155">String</span></span>|<span data-ttu-id="aaab7-156">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="aaab7-156">The name of the app.</span></span>|
|<span data-ttu-id="aaab7-157">notes</span><span class="sxs-lookup"><span data-stu-id="aaab7-157">Notes</span></span>|<span data-ttu-id="aaab7-158">String</span><span class="sxs-lookup"><span data-stu-id="aaab7-158">String</span></span>|<span data-ttu-id="aaab7-159">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="aaab7-159">Notes for the app.</span></span>|
|<span data-ttu-id="aaab7-160">publishingState</span><span class="sxs-lookup"><span data-stu-id="aaab7-160">publishingState</span></span>|<span data-ttu-id="aaab7-161">String</span><span class="sxs-lookup"><span data-stu-id="aaab7-161">String</span></span>|<span data-ttu-id="aaab7-162">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="aaab7-162">The publishing state for the app.</span></span> <span data-ttu-id="aaab7-163">Приложение не может быть назначено, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="aaab7-163">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="aaab7-164">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="aaab7-164">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaab7-165">Связи</span><span class="sxs-lookup"><span data-stu-id="aaab7-165">Relationships</span></span>
|<span data-ttu-id="aaab7-166">Связь</span><span class="sxs-lookup"><span data-stu-id="aaab7-166">Relationship</span></span>|<span data-ttu-id="aaab7-167">Тип</span><span class="sxs-lookup"><span data-stu-id="aaab7-167">Type</span></span>|<span data-ttu-id="aaab7-168">Описание</span><span class="sxs-lookup"><span data-stu-id="aaab7-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaab7-169">categories</span><span class="sxs-lookup"><span data-stu-id="aaab7-169">categories</span></span>|<span data-ttu-id="aaab7-170">Коллекция [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="aaab7-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="aaab7-171">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="aaab7-171">The list of categories for this app.</span></span>|
|<span data-ttu-id="aaab7-172">assignments</span><span class="sxs-lookup"><span data-stu-id="aaab7-172">assignments</span></span>|<span data-ttu-id="aaab7-173">Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aaab7-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="aaab7-174">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="aaab7-174">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aaab7-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aaab7-175">JSON Representation</span></span>
<span data-ttu-id="aaab7-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aaab7-176">Here is a JSON representation of the resource.</span></span>
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



