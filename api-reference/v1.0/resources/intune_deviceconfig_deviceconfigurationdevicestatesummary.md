# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="acc0e-101">Тип ресурса deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="acc0e-101">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="acc0e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="acc0e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acc0e-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="acc0e-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="acc0e-104">Методы</span><span class="sxs-lookup"><span data-stu-id="acc0e-104">Methods</span></span>
|<span data-ttu-id="acc0e-105">Метод</span><span class="sxs-lookup"><span data-stu-id="acc0e-105">Method</span></span>|<span data-ttu-id="acc0e-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="acc0e-106">Return Type</span></span>|<span data-ttu-id="acc0e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="acc0e-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="acc0e-108">Получение объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="acc0e-108">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_get.md)|[<span data-ttu-id="acc0e-109">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="acc0e-109">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="acc0e-110">Чтение свойств и связей объекта [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="acc0e-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="acc0e-111">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="acc0e-111">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_update.md)|[<span data-ttu-id="acc0e-112">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="acc0e-112">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="acc0e-113">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="acc0e-113">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="acc0e-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="acc0e-114">Properties</span></span>
|<span data-ttu-id="acc0e-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="acc0e-115">Property</span></span>|<span data-ttu-id="acc0e-116">Тип</span><span class="sxs-lookup"><span data-stu-id="acc0e-116">Type</span></span>|<span data-ttu-id="acc0e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="acc0e-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acc0e-118">id</span><span class="sxs-lookup"><span data-stu-id="acc0e-118">id</span></span>|<span data-ttu-id="acc0e-119">String</span><span class="sxs-lookup"><span data-stu-id="acc0e-119">String</span></span>|<span data-ttu-id="acc0e-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="acc0e-120">Key of the setting.</span></span>|
|<span data-ttu-id="acc0e-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acc0e-121">unknownDeviceCount</span></span>|<span data-ttu-id="acc0e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="acc0e-122">Int32</span></span>|<span data-ttu-id="acc0e-123">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="acc0e-123">Number of unknown devices</span></span>|
|<span data-ttu-id="acc0e-124">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acc0e-124">notApplicableDeviceCount</span></span>|<span data-ttu-id="acc0e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="acc0e-125">Int32</span></span>|<span data-ttu-id="acc0e-126">Количество неприменимых устройств</span><span class="sxs-lookup"><span data-stu-id="acc0e-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="acc0e-127">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acc0e-127">compliantDeviceCount</span></span>|<span data-ttu-id="acc0e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="acc0e-128">Int32</span></span>|<span data-ttu-id="acc0e-129">Количество устройств, соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="acc0e-129">Number of compliant devices</span></span>|
|<span data-ttu-id="acc0e-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acc0e-130">remediatedDeviceCount</span></span>|<span data-ttu-id="acc0e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="acc0e-131">Int32</span></span>|<span data-ttu-id="acc0e-132">Количество исправленных устройств</span><span class="sxs-lookup"><span data-stu-id="acc0e-132">Number of remediated devices</span></span>|
|<span data-ttu-id="acc0e-133">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acc0e-133">nonCompliantDeviceCount</span></span>|<span data-ttu-id="acc0e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="acc0e-134">Int32</span></span>|<span data-ttu-id="acc0e-135">Количество устройств, не соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="acc0e-135">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="acc0e-136">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acc0e-136">errorDeviceCount</span></span>|<span data-ttu-id="acc0e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="acc0e-137">Int32</span></span>|<span data-ttu-id="acc0e-138">Количество устройств с ошибками</span><span class="sxs-lookup"><span data-stu-id="acc0e-138">Number of error devices</span></span>|
|<span data-ttu-id="acc0e-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acc0e-139">conflictDeviceCount</span></span>|<span data-ttu-id="acc0e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="acc0e-140">Int32</span></span>|<span data-ttu-id="acc0e-141">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="acc0e-141">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="acc0e-142">Связи</span><span class="sxs-lookup"><span data-stu-id="acc0e-142">Relationships</span></span>
<span data-ttu-id="acc0e-143">Нет</span><span class="sxs-lookup"><span data-stu-id="acc0e-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="acc0e-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="acc0e-144">JSON Representation</span></span>
<span data-ttu-id="acc0e-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acc0e-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



