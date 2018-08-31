# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="81f17-101">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="81f17-101">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="81f17-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81f17-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81f17-103">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="81f17-103">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="81f17-104">Методы</span><span class="sxs-lookup"><span data-stu-id="81f17-104">Methods</span></span>
|<span data-ttu-id="81f17-105">Метод</span><span class="sxs-lookup"><span data-stu-id="81f17-105">Method</span></span>|<span data-ttu-id="81f17-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="81f17-106">Return Type</span></span>|<span data-ttu-id="81f17-107">Описание</span><span class="sxs-lookup"><span data-stu-id="81f17-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81f17-108">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="81f17-108">Get managedDeviceOverview</span></span>](../api/intune_devices_manageddeviceoverview_get.md)|[<span data-ttu-id="81f17-109">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="81f17-109">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="81f17-110">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="81f17-110">Read properties and relationships of the [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="81f17-111">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="81f17-111">Update managedDeviceOverview</span></span>](../api/intune_devices_manageddeviceoverview_update.md)|[<span data-ttu-id="81f17-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="81f17-112">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="81f17-113">Обновление свойств объекта [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="81f17-113">Update the properties of a [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81f17-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="81f17-114">Properties</span></span>
|<span data-ttu-id="81f17-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="81f17-115">Property</span></span>|<span data-ttu-id="81f17-116">Тип</span><span class="sxs-lookup"><span data-stu-id="81f17-116">Type</span></span>|<span data-ttu-id="81f17-117">Описание</span><span class="sxs-lookup"><span data-stu-id="81f17-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81f17-118">id</span><span class="sxs-lookup"><span data-stu-id="81f17-118">id</span></span>|<span data-ttu-id="81f17-119">String (строка)</span><span class="sxs-lookup"><span data-stu-id="81f17-119">String</span></span>|<span data-ttu-id="81f17-120">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="81f17-120">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="81f17-121">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="81f17-121">enrolledDeviceCount</span></span>|<span data-ttu-id="81f17-122">Int32</span><span class="sxs-lookup"><span data-stu-id="81f17-122">Int32</span></span>|<span data-ttu-id="81f17-123">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="81f17-123">Total enrolled device count.</span></span> <span data-ttu-id="81f17-124">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="81f17-124">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="81f17-125">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="81f17-125">mdmEnrolledCount</span></span>|<span data-ttu-id="81f17-126">Int32</span><span class="sxs-lookup"><span data-stu-id="81f17-126">Int32</span></span>|<span data-ttu-id="81f17-127">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="81f17-127">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="81f17-128">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="81f17-128">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="81f17-129">Int32</span><span class="sxs-lookup"><span data-stu-id="81f17-129">Int32</span></span>|<span data-ttu-id="81f17-130">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="81f17-130">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="81f17-131">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="81f17-131">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="81f17-132">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="81f17-132">deviceOperatingSystemSummary</span></span>](../resources/intune_devices_deviceoperatingsystemsummary.md)|<span data-ttu-id="81f17-133">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="81f17-133">Device operating system summary.</span></span>|
|<span data-ttu-id="81f17-134">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="81f17-134">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="81f17-135">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="81f17-135">deviceExchangeAccessStateSummary</span></span>](../resources/intune_devices_deviceexchangeaccessstatesummary.md)|<span data-ttu-id="81f17-136">Распределение состояния доступа Exchange Access State в Intune</span><span class="sxs-lookup"><span data-stu-id="81f17-136">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="81f17-137">Связи</span><span class="sxs-lookup"><span data-stu-id="81f17-137">Relationships</span></span>
<span data-ttu-id="81f17-138">Нет</span><span class="sxs-lookup"><span data-stu-id="81f17-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81f17-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81f17-139">JSON Representation</span></span>
<span data-ttu-id="81f17-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81f17-140">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```



