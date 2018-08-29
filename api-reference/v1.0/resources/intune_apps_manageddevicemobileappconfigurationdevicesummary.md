# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="e9008-101">Тип ресурса managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e9008-101">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="e9008-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e9008-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9008-103">Содержит свойства, унаследованные свойства и действия из сводки по состоянию конфигурации мобильных приложений MDM для устройства.</span><span class="sxs-lookup"><span data-stu-id="e9008-103">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="e9008-104">Методы</span><span class="sxs-lookup"><span data-stu-id="e9008-104">Methods</span></span>
|<span data-ttu-id="e9008-105">Метод</span><span class="sxs-lookup"><span data-stu-id="e9008-105">Method</span></span>|<span data-ttu-id="e9008-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e9008-106">Return Type</span></span>|<span data-ttu-id="e9008-107">Описание</span><span class="sxs-lookup"><span data-stu-id="e9008-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e9008-108">Получение объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e9008-108">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_get.md)|[<span data-ttu-id="e9008-109">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e9008-109">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="e9008-110">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e9008-110">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="e9008-111">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e9008-111">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_update.md)|[<span data-ttu-id="e9008-112">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e9008-112">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="e9008-113">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e9008-113">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e9008-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9008-114">Properties</span></span>
|<span data-ttu-id="e9008-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9008-115">Property</span></span>|<span data-ttu-id="e9008-116">Тип</span><span class="sxs-lookup"><span data-stu-id="e9008-116">Type</span></span>|<span data-ttu-id="e9008-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e9008-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9008-118">id</span><span class="sxs-lookup"><span data-stu-id="e9008-118">id</span></span>|<span data-ttu-id="e9008-119">Строка</span><span class="sxs-lookup"><span data-stu-id="e9008-119">String</span></span>|<span data-ttu-id="e9008-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e9008-120">Key of the entity.</span></span>|
|<span data-ttu-id="e9008-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e9008-121">pendingCount</span></span>|<span data-ttu-id="e9008-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e9008-122">Int32</span></span>|<span data-ttu-id="e9008-123">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="e9008-123">Number of pending devices</span></span>|
|<span data-ttu-id="e9008-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e9008-124">notApplicableCount</span></span>|<span data-ttu-id="e9008-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e9008-125">Int32</span></span>|<span data-ttu-id="e9008-126">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="e9008-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="e9008-127">successCount</span><span class="sxs-lookup"><span data-stu-id="e9008-127">successCount</span></span>|<span data-ttu-id="e9008-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e9008-128">Int32</span></span>|<span data-ttu-id="e9008-129">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="e9008-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="e9008-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="e9008-130">errorCount</span></span>|<span data-ttu-id="e9008-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e9008-131">Int32</span></span>|<span data-ttu-id="e9008-132">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e9008-132">Number of error devices</span></span>|
|<span data-ttu-id="e9008-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="e9008-133">failedCount</span></span>|<span data-ttu-id="e9008-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e9008-134">Int32</span></span>|<span data-ttu-id="e9008-135">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="e9008-135">Number of failed devices</span></span>|
|<span data-ttu-id="e9008-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e9008-136">lastUpdateDateTime</span></span>|<span data-ttu-id="e9008-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9008-137">DateTimeOffset</span></span>|<span data-ttu-id="e9008-138">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="e9008-138">Last update time</span></span>|
|<span data-ttu-id="e9008-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e9008-139">configurationVersion</span></span>|<span data-ttu-id="e9008-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e9008-140">Int32</span></span>|<span data-ttu-id="e9008-141">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="e9008-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9008-142">Связи</span><span class="sxs-lookup"><span data-stu-id="e9008-142">Relationships</span></span>
<span data-ttu-id="e9008-143">Нет</span><span class="sxs-lookup"><span data-stu-id="e9008-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e9008-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9008-144">JSON Representation</span></span>
<span data-ttu-id="e9008-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9008-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
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



