# <a name="devicemanagement-resource-type"></a><span data-ttu-id="0907e-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="0907e-101">deviceManagement resource type</span></span>

> <span data-ttu-id="0907e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0907e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0907e-103">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="0907e-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="0907e-104">Методы</span><span class="sxs-lookup"><span data-stu-id="0907e-104">Methods</span></span>
|<span data-ttu-id="0907e-105">Метод</span><span class="sxs-lookup"><span data-stu-id="0907e-105">Method</span></span>|<span data-ttu-id="0907e-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0907e-106">Return Type</span></span>|<span data-ttu-id="0907e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="0907e-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0907e-108">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="0907e-108">Get deviceManagement</span></span>](../api/intune_devices_devicemanagement_get.md)|[<span data-ttu-id="0907e-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="0907e-109">deviceManagement</span></span>](../resources/intune_devices_devicemanagement.md)|<span data-ttu-id="0907e-110">Чтение свойств и связей объекта [deviceManagement](../resources/intune_devices_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="0907e-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_devices_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="0907e-111">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="0907e-111">Update deviceManagement</span></span>](../api/intune_devices_devicemanagement_update.md)|[<span data-ttu-id="0907e-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="0907e-112">deviceManagement</span></span>](../resources/intune_devices_devicemanagement.md)|<span data-ttu-id="0907e-113">Обновление свойств объекта [deviceManagement](../resources/intune_devices_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="0907e-113">Update the properties of a [calendar](../resources/intune_devices_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0907e-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="0907e-114">Properties</span></span>
|<span data-ttu-id="0907e-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="0907e-115">Property</span></span>|<span data-ttu-id="0907e-116">Тип</span><span class="sxs-lookup"><span data-stu-id="0907e-116">Type</span></span>|<span data-ttu-id="0907e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="0907e-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0907e-118">id</span><span class="sxs-lookup"><span data-stu-id="0907e-118">id</span></span>|<span data-ttu-id="0907e-119">String</span><span class="sxs-lookup"><span data-stu-id="0907e-119">String</span></span>|<span data-ttu-id="0907e-120">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="0907e-120">Unique Identifier for the device</span></span>|
|<span data-ttu-id="0907e-121">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="0907e-121">subscriptionState</span></span>|<span data-ttu-id="0907e-122">String</span><span class="sxs-lookup"><span data-stu-id="0907e-122">String</span></span>|<span data-ttu-id="0907e-123">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="0907e-123">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="0907e-124">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="0907e-124">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0907e-125">Связи</span><span class="sxs-lookup"><span data-stu-id="0907e-125">Relationships</span></span>
|<span data-ttu-id="0907e-126">Связь</span><span class="sxs-lookup"><span data-stu-id="0907e-126">Relationship</span></span>|<span data-ttu-id="0907e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0907e-127">Type</span></span>|<span data-ttu-id="0907e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0907e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0907e-129">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0907e-129">applePushNotificationCertificate</span></span>|[<span data-ttu-id="0907e-130">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0907e-130">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="0907e-131">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="0907e-131">Apple push notification certificate.</span></span>|
|<span data-ttu-id="0907e-132">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0907e-132">managedDeviceOverview</span></span>|[<span data-ttu-id="0907e-133">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0907e-133">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="0907e-134">Обзор устройств</span><span class="sxs-lookup"><span data-stu-id="0907e-134">Device overview</span></span>|
|<span data-ttu-id="0907e-135">detectedApps</span><span class="sxs-lookup"><span data-stu-id="0907e-135">detectedApps</span></span>|<span data-ttu-id="0907e-136">Коллекция [detectedApp](../resources/intune_devices_detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="0907e-136">[detectedApp](../resources/intune_devices_detectedapp.md) collection</span></span>|<span data-ttu-id="0907e-137">Список обнаруженных приложений, связанных с устройством.</span><span class="sxs-lookup"><span data-stu-id="0907e-137">The list of detected apps associated with a device.</span></span>|
|<span data-ttu-id="0907e-138">managedDevices</span><span class="sxs-lookup"><span data-stu-id="0907e-138">managedDevices</span></span>|<span data-ttu-id="0907e-139">Коллекция [managedDevice](../resources/intune_devices_manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="0907e-139">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="0907e-140">Список управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="0907e-140">The list of managed devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0907e-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0907e-141">JSON Representation</span></span>
<span data-ttu-id="0907e-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0907e-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```



