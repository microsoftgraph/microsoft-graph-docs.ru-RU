# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="4507e-101">Тип ресурса managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4507e-101">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="4507e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4507e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4507e-103">Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="4507e-103">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="4507e-104">Методы</span><span class="sxs-lookup"><span data-stu-id="4507e-104">Methods</span></span>
|<span data-ttu-id="4507e-105">Метод</span><span class="sxs-lookup"><span data-stu-id="4507e-105">Method</span></span>|<span data-ttu-id="4507e-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4507e-106">Return Type</span></span>|<span data-ttu-id="4507e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4507e-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4507e-108">Список managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="4507e-108">List managedDeviceMobileAppConfigurations</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_list.md)|<span data-ttu-id="4507e-109">Коллекция [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4507e-109">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="4507e-110">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4507e-110">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="4507e-111">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4507e-111">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_get.md)|[<span data-ttu-id="4507e-112">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4507e-112">managedDeviceMobileAppConfiguration</span></span>](../resources/intune_apps_manageddevicemobileappconfiguration.md)|<span data-ttu-id="4507e-113">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4507e-113">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4507e-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="4507e-114">Properties</span></span>
|<span data-ttu-id="4507e-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="4507e-115">Property</span></span>|<span data-ttu-id="4507e-116">Тип</span><span class="sxs-lookup"><span data-stu-id="4507e-116">Type</span></span>|<span data-ttu-id="4507e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4507e-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4507e-118">id</span><span class="sxs-lookup"><span data-stu-id="4507e-118">id</span></span>|<span data-ttu-id="4507e-119">Строка</span><span class="sxs-lookup"><span data-stu-id="4507e-119">String</span></span>|<span data-ttu-id="4507e-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4507e-120">Key of the entity.</span></span>|
|<span data-ttu-id="4507e-121">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="4507e-121">targetedMobileApps</span></span>|<span data-ttu-id="4507e-122">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4507e-122">String collection</span></span>|<span data-ttu-id="4507e-123">Связанное приложение.</span><span class="sxs-lookup"><span data-stu-id="4507e-123">the associated app.</span></span>|
|<span data-ttu-id="4507e-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4507e-124">createdDateTime</span></span>|<span data-ttu-id="4507e-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4507e-125">DateTimeOffset</span></span>|<span data-ttu-id="4507e-126">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4507e-126">DateTime the object was created.</span></span>|
|<span data-ttu-id="4507e-127">description</span><span class="sxs-lookup"><span data-stu-id="4507e-127">description</span></span>|<span data-ttu-id="4507e-128">Строка</span><span class="sxs-lookup"><span data-stu-id="4507e-128">String</span></span>|<span data-ttu-id="4507e-129">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4507e-129">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="4507e-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4507e-130">lastModifiedDateTime</span></span>|<span data-ttu-id="4507e-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4507e-131">DateTimeOffset</span></span>|<span data-ttu-id="4507e-132">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4507e-132">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4507e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="4507e-133">displayName</span></span>|<span data-ttu-id="4507e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4507e-134">String</span></span>|<span data-ttu-id="4507e-135">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4507e-135">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="4507e-136">version</span><span class="sxs-lookup"><span data-stu-id="4507e-136">version</span></span>|<span data-ttu-id="4507e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4507e-137">Int32</span></span>|<span data-ttu-id="4507e-138">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4507e-138">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4507e-139">Связи</span><span class="sxs-lookup"><span data-stu-id="4507e-139">Relationships</span></span>
|<span data-ttu-id="4507e-140">Связь</span><span class="sxs-lookup"><span data-stu-id="4507e-140">Relationship</span></span>|<span data-ttu-id="4507e-141">Тип</span><span class="sxs-lookup"><span data-stu-id="4507e-141">Type</span></span>|<span data-ttu-id="4507e-142">Описание</span><span class="sxs-lookup"><span data-stu-id="4507e-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4507e-143">assignments</span><span class="sxs-lookup"><span data-stu-id="4507e-143">assignments</span></span>|<span data-ttu-id="4507e-144">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4507e-144">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4507e-145">Список заданий группы для настройки приложения.</span><span class="sxs-lookup"><span data-stu-id="4507e-145">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="4507e-146">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="4507e-146">deviceStatuses</span></span>|<span data-ttu-id="4507e-147">Коллекция [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="4507e-147">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="4507e-148">Список объектов ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="4507e-148">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="4507e-149">userStatuses</span><span class="sxs-lookup"><span data-stu-id="4507e-149">userStatuses</span></span>|<span data-ttu-id="4507e-150">Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="4507e-150">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="4507e-151">Список объектов ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="4507e-151">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="4507e-152">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="4507e-152">deviceStatusSummary</span></span>|[<span data-ttu-id="4507e-153">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="4507e-153">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="4507e-154">Общие сведения о состоянии устройства, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="4507e-154">App configuration device status summary.</span></span>|
|<span data-ttu-id="4507e-155">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="4507e-155">userStatusSummary</span></span>|[<span data-ttu-id="4507e-156">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="4507e-156">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="4507e-157">Общие сведения о состоянии пользователя, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="4507e-157">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4507e-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4507e-158">JSON Representation</span></span>
<span data-ttu-id="4507e-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4507e-159">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```








