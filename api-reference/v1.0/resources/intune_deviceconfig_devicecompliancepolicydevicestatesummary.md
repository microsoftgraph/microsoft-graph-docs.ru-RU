# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="7e5fa-101">Тип ресурса deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7e5fa-101">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="7e5fa-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7e5fa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e5fa-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7e5fa-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="7e5fa-104">Методы</span><span class="sxs-lookup"><span data-stu-id="7e5fa-104">Methods</span></span>
|<span data-ttu-id="7e5fa-105">Метод</span><span class="sxs-lookup"><span data-stu-id="7e5fa-105">Method</span></span>|<span data-ttu-id="7e5fa-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7e5fa-106">Return Type</span></span>|<span data-ttu-id="7e5fa-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7e5fa-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e5fa-108">Получение объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7e5fa-108">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_get.md)|[<span data-ttu-id="7e5fa-109">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7e5fa-109">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="7e5fa-110">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7e5fa-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="7e5fa-111">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7e5fa-111">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_update.md)|[<span data-ttu-id="7e5fa-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7e5fa-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="7e5fa-113">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7e5fa-113">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e5fa-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e5fa-114">Properties</span></span>
|<span data-ttu-id="7e5fa-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e5fa-115">Property</span></span>|<span data-ttu-id="7e5fa-116">Тип</span><span class="sxs-lookup"><span data-stu-id="7e5fa-116">Type</span></span>|<span data-ttu-id="7e5fa-117">Описание</span><span class="sxs-lookup"><span data-stu-id="7e5fa-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e5fa-118">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="7e5fa-118">inGracePeriodCount</span></span>|<span data-ttu-id="7e5fa-119">Int32</span><span class="sxs-lookup"><span data-stu-id="7e5fa-119">Int32</span></span>|<span data-ttu-id="7e5fa-120">Количество устройств, для которых действует льготный период</span><span class="sxs-lookup"><span data-stu-id="7e5fa-120">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="7e5fa-121">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="7e5fa-121">configManagerCount</span></span>|<span data-ttu-id="7e5fa-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7e5fa-122">Int32</span></span>|<span data-ttu-id="7e5fa-123">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="7e5fa-123">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="7e5fa-124">id</span><span class="sxs-lookup"><span data-stu-id="7e5fa-124">id</span></span>|<span data-ttu-id="7e5fa-125">String</span><span class="sxs-lookup"><span data-stu-id="7e5fa-125">String</span></span>|<span data-ttu-id="7e5fa-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7e5fa-126">Key of the setting.</span></span>|
|<span data-ttu-id="7e5fa-127">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e5fa-127">unknownDeviceCount</span></span>|<span data-ttu-id="7e5fa-128">Int32</span><span class="sxs-lookup"><span data-stu-id="7e5fa-128">Int32</span></span>|<span data-ttu-id="7e5fa-129">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="7e5fa-129">Number of unknown devices</span></span>|
|<span data-ttu-id="7e5fa-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e5fa-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="7e5fa-131">Int32</span><span class="sxs-lookup"><span data-stu-id="7e5fa-131">Int32</span></span>|<span data-ttu-id="7e5fa-132">Количество неприменимых устройств</span><span class="sxs-lookup"><span data-stu-id="7e5fa-132">Number of not applicable devices</span></span>|
|<span data-ttu-id="7e5fa-133">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e5fa-133">compliantDeviceCount</span></span>|<span data-ttu-id="7e5fa-134">Int32</span><span class="sxs-lookup"><span data-stu-id="7e5fa-134">Int32</span></span>|<span data-ttu-id="7e5fa-135">Количество устройств, соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="7e5fa-135">Number of compliant devices</span></span>|
|<span data-ttu-id="7e5fa-136">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e5fa-136">remediatedDeviceCount</span></span>|<span data-ttu-id="7e5fa-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7e5fa-137">Int32</span></span>|<span data-ttu-id="7e5fa-138">Количество исправленных устройств</span><span class="sxs-lookup"><span data-stu-id="7e5fa-138">Number of remediated devices</span></span>|
|<span data-ttu-id="7e5fa-139">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e5fa-139">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7e5fa-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7e5fa-140">Int32</span></span>|<span data-ttu-id="7e5fa-141">Количество устройств, не соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="7e5fa-141">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="7e5fa-142">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e5fa-142">errorDeviceCount</span></span>|<span data-ttu-id="7e5fa-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7e5fa-143">Int32</span></span>|<span data-ttu-id="7e5fa-144">Количество устройств с ошибками</span><span class="sxs-lookup"><span data-stu-id="7e5fa-144">Number of error devices</span></span>|
|<span data-ttu-id="7e5fa-145">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e5fa-145">conflictDeviceCount</span></span>|<span data-ttu-id="7e5fa-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7e5fa-146">Int32</span></span>|<span data-ttu-id="7e5fa-147">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="7e5fa-147">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e5fa-148">Связи</span><span class="sxs-lookup"><span data-stu-id="7e5fa-148">Relationships</span></span>
<span data-ttu-id="7e5fa-149">Нет</span><span class="sxs-lookup"><span data-stu-id="7e5fa-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7e5fa-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e5fa-150">JSON Representation</span></span>
<span data-ttu-id="7e5fa-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e5fa-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
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



