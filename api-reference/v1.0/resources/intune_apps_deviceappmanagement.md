# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="57549-101">Тип ресурса deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="57549-101">deviceAppManagement resource type</span></span>

> <span data-ttu-id="57549-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="57549-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57549-103">Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.</span><span class="sxs-lookup"><span data-stu-id="57549-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="57549-104">Методы</span><span class="sxs-lookup"><span data-stu-id="57549-104">Methods</span></span>
|<span data-ttu-id="57549-105">Метод</span><span class="sxs-lookup"><span data-stu-id="57549-105">Method</span></span>|<span data-ttu-id="57549-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="57549-106">Return Type</span></span>|<span data-ttu-id="57549-107">Описание</span><span class="sxs-lookup"><span data-stu-id="57549-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="57549-108">Получение объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="57549-108">Get deviceAppManagement</span></span>](../api/intune_apps_deviceappmanagement_get.md)|[<span data-ttu-id="57549-109">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="57549-109">deviceAppManagement</span></span>](../resources/intune_apps_deviceappmanagement.md)|<span data-ttu-id="57549-110">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="57549-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="57549-111">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="57549-111">Update deviceAppManagement</span></span>](../api/intune_apps_deviceappmanagement_update.md)|[<span data-ttu-id="57549-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="57549-112">deviceAppManagement</span></span>](../resources/intune_apps_deviceappmanagement.md)|<span data-ttu-id="57549-113">Обновление свойств объекта [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="57549-113">Update the properties of a [calendar](../resources/intune_apps_deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="57549-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="57549-114">Properties</span></span>
|<span data-ttu-id="57549-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="57549-115">Property</span></span>|<span data-ttu-id="57549-116">Тип</span><span class="sxs-lookup"><span data-stu-id="57549-116">Type</span></span>|<span data-ttu-id="57549-117">Описание</span><span class="sxs-lookup"><span data-stu-id="57549-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57549-118">id</span><span class="sxs-lookup"><span data-stu-id="57549-118">id</span></span>|<span data-ttu-id="57549-119">String</span><span class="sxs-lookup"><span data-stu-id="57549-119">String</span></span>|<span data-ttu-id="57549-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="57549-120">Key of the setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57549-121">Связи</span><span class="sxs-lookup"><span data-stu-id="57549-121">Relationships</span></span>
|<span data-ttu-id="57549-122">Связь</span><span class="sxs-lookup"><span data-stu-id="57549-122">Relationship</span></span>|<span data-ttu-id="57549-123">Тип</span><span class="sxs-lookup"><span data-stu-id="57549-123">Type</span></span>|<span data-ttu-id="57549-124">Описание</span><span class="sxs-lookup"><span data-stu-id="57549-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57549-125">mobileApps</span><span class="sxs-lookup"><span data-stu-id="57549-125">mobileApps</span></span>|<span data-ttu-id="57549-126">Коллекция [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="57549-126">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="57549-127">Мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="57549-127">The mobile apps.</span></span>|
|<span data-ttu-id="57549-128">mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="57549-128">mobileAppCategories</span></span>|<span data-ttu-id="57549-129">Коллекция [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="57549-129">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="57549-130">Категории мобильных приложений</span><span class="sxs-lookup"><span data-stu-id="57549-130">The mobile app categories.</span></span>|
|<span data-ttu-id="57549-131">mobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="57549-131">mobileAppConfigurations</span></span>|<span data-ttu-id="57549-132">Коллекция [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57549-132">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="57549-133">Конфигурации мобильных приложений для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="57549-133">The Managed Device Mobile Application Configurations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57549-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57549-134">JSON Representation</span></span>
<span data-ttu-id="57549-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57549-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



