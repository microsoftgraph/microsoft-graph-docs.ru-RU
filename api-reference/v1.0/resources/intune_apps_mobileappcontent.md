# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="ebf46-101">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebf46-101">mobileAppContent resource type</span></span>

> <span data-ttu-id="ebf46-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ebf46-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebf46-103">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="ebf46-103">Contains content properties for a specific app version.</span></span> <span data-ttu-id="ebf46-104">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="ebf46-104">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="ebf46-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ebf46-105">Methods</span></span>
|<span data-ttu-id="ebf46-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ebf46-106">Method</span></span>|<span data-ttu-id="ebf46-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ebf46-107">Return Type</span></span>|<span data-ttu-id="ebf46-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ebf46-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebf46-109">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="ebf46-109">List mobileAppContents</span></span>](../api/intune_apps_mobileappcontent_list.md)|<span data-ttu-id="ebf46-110">Коллекция [mobileAppContent](../resources/intune_apps_mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="ebf46-110">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) collection</span></span>|<span data-ttu-id="ebf46-111">Список свойств и связей объектов [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ebf46-111">List properties and relationships of the [mobileAppContent](../resources/intune_apps_mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="ebf46-112">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebf46-112">Get mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_get.md)|[<span data-ttu-id="ebf46-113">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebf46-113">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="ebf46-114">Чтение свойств и связей объекта [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ebf46-114">Read properties and relationships of the [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ebf46-115">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebf46-115">Create mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_create.md)|[<span data-ttu-id="ebf46-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebf46-116">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="ebf46-117">Создание объекта [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ebf46-117">Create a new [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ebf46-118">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebf46-118">Delete mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_delete.md)|<span data-ttu-id="ebf46-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ebf46-119">None</span></span>|<span data-ttu-id="ebf46-120">Удаляет объект [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ebf46-120">Deletes a [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span></span>|
|[<span data-ttu-id="ebf46-121">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebf46-121">Update mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_update.md)|[<span data-ttu-id="ebf46-122">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebf46-122">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="ebf46-123">Обновление свойств объекта [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ebf46-123">Update the properties of a [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ebf46-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebf46-124">Properties</span></span>
|<span data-ttu-id="ebf46-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebf46-125">Property</span></span>|<span data-ttu-id="ebf46-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ebf46-126">Type</span></span>|<span data-ttu-id="ebf46-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ebf46-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebf46-128">id</span><span class="sxs-lookup"><span data-stu-id="ebf46-128">id</span></span>|<span data-ttu-id="ebf46-129">String</span><span class="sxs-lookup"><span data-stu-id="ebf46-129">String</span></span>|<span data-ttu-id="ebf46-130">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="ebf46-130">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebf46-131">Связи</span><span class="sxs-lookup"><span data-stu-id="ebf46-131">Relationships</span></span>
|<span data-ttu-id="ebf46-132">Связь</span><span class="sxs-lookup"><span data-stu-id="ebf46-132">Relationship</span></span>|<span data-ttu-id="ebf46-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ebf46-133">Type</span></span>|<span data-ttu-id="ebf46-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ebf46-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebf46-135">files</span><span class="sxs-lookup"><span data-stu-id="ebf46-135">files</span></span>|<span data-ttu-id="ebf46-136">Коллекция [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="ebf46-136">[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="ebf46-137">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="ebf46-137">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebf46-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebf46-138">JSON Representation</span></span>
<span data-ttu-id="ebf46-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebf46-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```



