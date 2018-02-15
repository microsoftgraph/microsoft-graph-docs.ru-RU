# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="15964-101">Тип ресурса deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="15964-101">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="15964-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="15964-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15964-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="15964-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="15964-104">Методы</span><span class="sxs-lookup"><span data-stu-id="15964-104">Methods</span></span>
|<span data-ttu-id="15964-105">Метод</span><span class="sxs-lookup"><span data-stu-id="15964-105">Method</span></span>|<span data-ttu-id="15964-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="15964-106">Return Type</span></span>|<span data-ttu-id="15964-107">Описание</span><span class="sxs-lookup"><span data-stu-id="15964-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15964-108">Получение объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="15964-108">Get deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_get.md)|[<span data-ttu-id="15964-109">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="15964-109">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="15964-110">Чтение свойств и связей объекта [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="15964-110">Read properties and relationships of [plannerPlanDetails](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="15964-111">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="15964-111">Update deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_update.md)|[<span data-ttu-id="15964-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="15964-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="15964-113">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="15964-113">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="15964-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="15964-114">Properties</span></span>
|<span data-ttu-id="15964-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="15964-115">Property</span></span>|<span data-ttu-id="15964-116">Тип</span><span class="sxs-lookup"><span data-stu-id="15964-116">Type</span></span>|<span data-ttu-id="15964-117">Описание</span><span class="sxs-lookup"><span data-stu-id="15964-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15964-118">id</span><span class="sxs-lookup"><span data-stu-id="15964-118">id</span></span>|<span data-ttu-id="15964-119">String</span><span class="sxs-lookup"><span data-stu-id="15964-119">String</span></span>|<span data-ttu-id="15964-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="15964-120">Key of the setting.</span></span>|
|<span data-ttu-id="15964-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="15964-121">pendingCount</span></span>|<span data-ttu-id="15964-122">Int32</span><span class="sxs-lookup"><span data-stu-id="15964-122">Int32</span></span>|<span data-ttu-id="15964-123">Количество ожидающих устройств</span><span class="sxs-lookup"><span data-stu-id="15964-123">Number of pending devices</span></span>|
|<span data-ttu-id="15964-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="15964-124">notApplicableCount</span></span>|<span data-ttu-id="15964-125">Int32</span><span class="sxs-lookup"><span data-stu-id="15964-125">Int32</span></span>|<span data-ttu-id="15964-126">Количество неприменимых устройств</span><span class="sxs-lookup"><span data-stu-id="15964-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="15964-127">successCount</span><span class="sxs-lookup"><span data-stu-id="15964-127">successCount</span></span>|<span data-ttu-id="15964-128">Int32</span><span class="sxs-lookup"><span data-stu-id="15964-128">Int32</span></span>|<span data-ttu-id="15964-129">Количество успешных устройств</span><span class="sxs-lookup"><span data-stu-id="15964-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="15964-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="15964-130">errorCount</span></span>|<span data-ttu-id="15964-131">Int32</span><span class="sxs-lookup"><span data-stu-id="15964-131">Int32</span></span>|<span data-ttu-id="15964-132">Количество устройств с ошибками</span><span class="sxs-lookup"><span data-stu-id="15964-132">Number of error devices</span></span>|
|<span data-ttu-id="15964-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="15964-133">failedCount</span></span>|<span data-ttu-id="15964-134">Int32</span><span class="sxs-lookup"><span data-stu-id="15964-134">Int32</span></span>|<span data-ttu-id="15964-135">Количество устройств со сбоями</span><span class="sxs-lookup"><span data-stu-id="15964-135">Number of failed devices</span></span>|
|<span data-ttu-id="15964-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="15964-136">lastUpdateDateTime</span></span>|<span data-ttu-id="15964-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15964-137">DateTimeOffset</span></span>|<span data-ttu-id="15964-138">Время последнего обновления</span><span class="sxs-lookup"><span data-stu-id="15964-138">Last update time</span></span>|
|<span data-ttu-id="15964-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="15964-139">configurationVersion</span></span>|<span data-ttu-id="15964-140">Int32</span><span class="sxs-lookup"><span data-stu-id="15964-140">Int32</span></span>|<span data-ttu-id="15964-141">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="15964-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="15964-142">Связи</span><span class="sxs-lookup"><span data-stu-id="15964-142">Relationships</span></span>
<span data-ttu-id="15964-143">Нет</span><span class="sxs-lookup"><span data-stu-id="15964-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15964-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15964-144">JSON Representation</span></span>
<span data-ttu-id="15964-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15964-145">Here is a JSON representation of the resource.</span></span>
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



