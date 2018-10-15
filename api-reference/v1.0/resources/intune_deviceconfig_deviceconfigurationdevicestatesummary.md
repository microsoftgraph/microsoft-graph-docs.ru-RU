# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="8c260-101">Тип ресурса deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="8c260-101">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="8c260-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8c260-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c260-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8c260-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="8c260-104">Методы</span><span class="sxs-lookup"><span data-stu-id="8c260-104">Methods</span></span>
|<span data-ttu-id="8c260-105">Метод</span><span class="sxs-lookup"><span data-stu-id="8c260-105">Method</span></span>|<span data-ttu-id="8c260-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8c260-106">Return Type</span></span>|<span data-ttu-id="8c260-107">Описание</span><span class="sxs-lookup"><span data-stu-id="8c260-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8c260-108">Получение объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="8c260-108">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_get.md)|[<span data-ttu-id="8c260-109">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="8c260-109">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="8c260-110">Чтение свойств и связей объекта [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8c260-110">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="8c260-111">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="8c260-111">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_update.md)|[<span data-ttu-id="8c260-112">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="8c260-112">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="8c260-113">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8c260-113">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c260-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c260-114">Properties</span></span>
|<span data-ttu-id="8c260-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c260-115">Property</span></span>|<span data-ttu-id="8c260-116">Тип</span><span class="sxs-lookup"><span data-stu-id="8c260-116">Type</span></span>|<span data-ttu-id="8c260-117">Описание</span><span class="sxs-lookup"><span data-stu-id="8c260-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c260-118">id</span><span class="sxs-lookup"><span data-stu-id="8c260-118">id</span></span>|<span data-ttu-id="8c260-119">Строка</span><span class="sxs-lookup"><span data-stu-id="8c260-119">String</span></span>|<span data-ttu-id="8c260-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8c260-120">Key of the entity.</span></span>|
|<span data-ttu-id="8c260-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8c260-121">unknownDeviceCount</span></span>|<span data-ttu-id="8c260-122">Int32</span><span class="sxs-lookup"><span data-stu-id="8c260-122">Int32</span></span>|<span data-ttu-id="8c260-123">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="8c260-123">Number of unknown devices</span></span>|
|<span data-ttu-id="8c260-124">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8c260-124">notApplicableDeviceCount</span></span>|<span data-ttu-id="8c260-125">Int32</span><span class="sxs-lookup"><span data-stu-id="8c260-125">Int32</span></span>|<span data-ttu-id="8c260-126">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="8c260-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="8c260-127">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8c260-127">compliantDeviceCount</span></span>|<span data-ttu-id="8c260-128">Int32</span><span class="sxs-lookup"><span data-stu-id="8c260-128">Int32</span></span>|<span data-ttu-id="8c260-129">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="8c260-129">Number of compliant devices</span></span>|
|<span data-ttu-id="8c260-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8c260-130">remediatedDeviceCount</span></span>|<span data-ttu-id="8c260-131">Int32</span><span class="sxs-lookup"><span data-stu-id="8c260-131">Int32</span></span>|<span data-ttu-id="8c260-132">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="8c260-132">Number of remediated devices</span></span>|
|<span data-ttu-id="8c260-133">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8c260-133">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8c260-134">Int32</span><span class="sxs-lookup"><span data-stu-id="8c260-134">Int32</span></span>|<span data-ttu-id="8c260-135">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="8c260-135">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="8c260-136">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8c260-136">errorDeviceCount</span></span>|<span data-ttu-id="8c260-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8c260-137">Int32</span></span>|<span data-ttu-id="8c260-138">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="8c260-138">Number of error devices</span></span>|
|<span data-ttu-id="8c260-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8c260-139">conflictDeviceCount</span></span>|<span data-ttu-id="8c260-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8c260-140">Int32</span></span>|<span data-ttu-id="8c260-141">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="8c260-141">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c260-142">Связи</span><span class="sxs-lookup"><span data-stu-id="8c260-142">Relationships</span></span>
<span data-ttu-id="8c260-143">Нет</span><span class="sxs-lookup"><span data-stu-id="8c260-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c260-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c260-144">JSON Representation</span></span>
<span data-ttu-id="8c260-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c260-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}-->
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



