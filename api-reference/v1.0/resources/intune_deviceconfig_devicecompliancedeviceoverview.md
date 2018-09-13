# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="d2040-101">Тип ресурса deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d2040-101">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="d2040-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d2040-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2040-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d2040-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="d2040-104">Методы</span><span class="sxs-lookup"><span data-stu-id="d2040-104">Methods</span></span>
|<span data-ttu-id="d2040-105">Метод</span><span class="sxs-lookup"><span data-stu-id="d2040-105">Method</span></span>|<span data-ttu-id="d2040-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d2040-106">Return Type</span></span>|<span data-ttu-id="d2040-107">Описание</span><span class="sxs-lookup"><span data-stu-id="d2040-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2040-108">Получение объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d2040-108">Get deviceComplianceDeviceOverview</span></span>](../api/intune_deviceconfig_devicecompliancedeviceoverview_get.md)|[<span data-ttu-id="d2040-109">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d2040-109">deviceComplianceDeviceOverview</span></span>](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|<span data-ttu-id="d2040-110">Чтение свойств и связей объекта [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="d2040-110">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="d2040-111">Обновление объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d2040-111">Update deviceComplianceDeviceOverview</span></span>](../api/intune_deviceconfig_devicecompliancedeviceoverview_update.md)|[<span data-ttu-id="d2040-112">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d2040-112">deviceComplianceDeviceOverview</span></span>](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|<span data-ttu-id="d2040-113">Обновление свойств объекта [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="d2040-113">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2040-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2040-114">Properties</span></span>
|<span data-ttu-id="d2040-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2040-115">Property</span></span>|<span data-ttu-id="d2040-116">Тип</span><span class="sxs-lookup"><span data-stu-id="d2040-116">Type</span></span>|<span data-ttu-id="d2040-117">Описание</span><span class="sxs-lookup"><span data-stu-id="d2040-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2040-118">id</span><span class="sxs-lookup"><span data-stu-id="d2040-118">id</span></span>|<span data-ttu-id="d2040-119">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d2040-119">String</span></span>|<span data-ttu-id="d2040-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d2040-120">Key of the entity.</span></span>|
|<span data-ttu-id="d2040-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="d2040-121">pendingCount</span></span>|<span data-ttu-id="d2040-122">Int32</span><span class="sxs-lookup"><span data-stu-id="d2040-122">Int32</span></span>|<span data-ttu-id="d2040-123">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="d2040-123">Number of pending devices</span></span>|
|<span data-ttu-id="d2040-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d2040-124">notApplicableCount</span></span>|<span data-ttu-id="d2040-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d2040-125">Int32</span></span>|<span data-ttu-id="d2040-126">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="d2040-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="d2040-127">successCount</span><span class="sxs-lookup"><span data-stu-id="d2040-127">successCount</span></span>|<span data-ttu-id="d2040-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d2040-128">Int32</span></span>|<span data-ttu-id="d2040-129">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="d2040-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="d2040-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="d2040-130">errorCount</span></span>|<span data-ttu-id="d2040-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d2040-131">Int32</span></span>|<span data-ttu-id="d2040-132">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="d2040-132">Number of error devices</span></span>|
|<span data-ttu-id="d2040-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="d2040-133">failedCount</span></span>|<span data-ttu-id="d2040-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d2040-134">Int32</span></span>|<span data-ttu-id="d2040-135">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="d2040-135">Number of failed devices</span></span>|
|<span data-ttu-id="d2040-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d2040-136">lastUpdateDateTime</span></span>|<span data-ttu-id="d2040-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2040-137">DateTimeOffset</span></span>|<span data-ttu-id="d2040-138">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="d2040-138">Last update time</span></span>|
|<span data-ttu-id="d2040-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="d2040-139">configurationVersion</span></span>|<span data-ttu-id="d2040-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d2040-140">Int32</span></span>|<span data-ttu-id="d2040-141">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="d2040-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2040-142">Связи</span><span class="sxs-lookup"><span data-stu-id="d2040-142">Relationships</span></span>
<span data-ttu-id="d2040-143">Нет</span><span class="sxs-lookup"><span data-stu-id="d2040-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2040-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2040-144">JSON Representation</span></span>
<span data-ttu-id="d2040-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2040-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
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








