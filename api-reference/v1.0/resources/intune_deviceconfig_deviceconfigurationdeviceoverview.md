# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="7e512-101">Тип ресурса deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7e512-101">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="7e512-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7e512-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e512-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7e512-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="7e512-104">Методы</span><span class="sxs-lookup"><span data-stu-id="7e512-104">Methods</span></span>
|<span data-ttu-id="7e512-105">Метод</span><span class="sxs-lookup"><span data-stu-id="7e512-105">Method</span></span>|<span data-ttu-id="7e512-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7e512-106">Return Type</span></span>|<span data-ttu-id="7e512-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7e512-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e512-108">Получение объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7e512-108">Get deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_get.md)|[<span data-ttu-id="7e512-109">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7e512-109">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="7e512-110">Чтение свойств и связей объекта [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="7e512-110">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="7e512-111">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7e512-111">Update deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_update.md)|[<span data-ttu-id="7e512-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7e512-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="7e512-113">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="7e512-113">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e512-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e512-114">Properties</span></span>
|<span data-ttu-id="7e512-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e512-115">Property</span></span>|<span data-ttu-id="7e512-116">Тип</span><span class="sxs-lookup"><span data-stu-id="7e512-116">Type</span></span>|<span data-ttu-id="7e512-117">Описание</span><span class="sxs-lookup"><span data-stu-id="7e512-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e512-118">id</span><span class="sxs-lookup"><span data-stu-id="7e512-118">id</span></span>|<span data-ttu-id="7e512-119">String</span><span class="sxs-lookup"><span data-stu-id="7e512-119">String</span></span>|<span data-ttu-id="7e512-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7e512-120">Key of the entity.</span></span>|
|<span data-ttu-id="7e512-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="7e512-121">pendingCount</span></span>|<span data-ttu-id="7e512-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7e512-122">Int32</span></span>|<span data-ttu-id="7e512-123">Количество ожидающих устройств</span><span class="sxs-lookup"><span data-stu-id="7e512-123">Number of pending devices</span></span>|
|<span data-ttu-id="7e512-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="7e512-124">notApplicableCount</span></span>|<span data-ttu-id="7e512-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7e512-125">Int32</span></span>|<span data-ttu-id="7e512-126">Количество неприменимых устройств</span><span class="sxs-lookup"><span data-stu-id="7e512-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="7e512-127">successCount</span><span class="sxs-lookup"><span data-stu-id="7e512-127">successCount</span></span>|<span data-ttu-id="7e512-128">Int32</span><span class="sxs-lookup"><span data-stu-id="7e512-128">Int32</span></span>|<span data-ttu-id="7e512-129">Количество успешных устройств</span><span class="sxs-lookup"><span data-stu-id="7e512-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="7e512-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="7e512-130">errorCount</span></span>|<span data-ttu-id="7e512-131">Int32</span><span class="sxs-lookup"><span data-stu-id="7e512-131">Int32</span></span>|<span data-ttu-id="7e512-132">Количество устройств с ошибками</span><span class="sxs-lookup"><span data-stu-id="7e512-132">Number of error devices</span></span>|
|<span data-ttu-id="7e512-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="7e512-133">failedCount</span></span>|<span data-ttu-id="7e512-134">Int32</span><span class="sxs-lookup"><span data-stu-id="7e512-134">Int32</span></span>|<span data-ttu-id="7e512-135">Количество устройств со сбоями</span><span class="sxs-lookup"><span data-stu-id="7e512-135">Number of failed devices</span></span>|
|<span data-ttu-id="7e512-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="7e512-136">lastUpdateDateTime</span></span>|<span data-ttu-id="7e512-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e512-137">DateTimeOffset</span></span>|<span data-ttu-id="7e512-138">Время последнего обновления</span><span class="sxs-lookup"><span data-stu-id="7e512-138">Last update time</span></span>|
|<span data-ttu-id="7e512-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="7e512-139">configurationVersion</span></span>|<span data-ttu-id="7e512-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7e512-140">Int32</span></span>|<span data-ttu-id="7e512-141">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="7e512-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e512-142">Связи</span><span class="sxs-lookup"><span data-stu-id="7e512-142">Relationships</span></span>
<span data-ttu-id="7e512-143">Нет</span><span class="sxs-lookup"><span data-stu-id="7e512-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7e512-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e512-144">JSON Representation</span></span>
<span data-ttu-id="7e512-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e512-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



