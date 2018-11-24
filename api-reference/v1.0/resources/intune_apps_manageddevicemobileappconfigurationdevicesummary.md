# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="cd852-101">Тип ресурса managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="cd852-101">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="cd852-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cd852-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd852-103">Содержит свойства, унаследованные свойства и действия из сводки по состоянию конфигурации мобильных приложений MDM для устройства.</span><span class="sxs-lookup"><span data-stu-id="cd852-103">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="cd852-104">Методы</span><span class="sxs-lookup"><span data-stu-id="cd852-104">Methods</span></span>
|<span data-ttu-id="cd852-105">Метод</span><span class="sxs-lookup"><span data-stu-id="cd852-105">Method</span></span>|<span data-ttu-id="cd852-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd852-106">Return Type</span></span>|<span data-ttu-id="cd852-107">Описание</span><span class="sxs-lookup"><span data-stu-id="cd852-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cd852-108">Получение объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="cd852-108">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_get.md)|[<span data-ttu-id="cd852-109">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="cd852-109">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="cd852-110">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="cd852-110">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="cd852-111">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="cd852-111">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_update.md)|[<span data-ttu-id="cd852-112">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="cd852-112">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="cd852-113">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="cd852-113">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd852-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd852-114">Properties</span></span>
|<span data-ttu-id="cd852-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd852-115">Property</span></span>|<span data-ttu-id="cd852-116">Тип</span><span class="sxs-lookup"><span data-stu-id="cd852-116">Type</span></span>|<span data-ttu-id="cd852-117">Описание</span><span class="sxs-lookup"><span data-stu-id="cd852-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd852-118">id</span><span class="sxs-lookup"><span data-stu-id="cd852-118">id</span></span>|<span data-ttu-id="cd852-119">String</span><span class="sxs-lookup"><span data-stu-id="cd852-119">String</span></span>|<span data-ttu-id="cd852-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cd852-120">Key of the entity.</span></span>|
|<span data-ttu-id="cd852-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="cd852-121">pendingCount</span></span>|<span data-ttu-id="cd852-122">Int32</span><span class="sxs-lookup"><span data-stu-id="cd852-122">Int32</span></span>|<span data-ttu-id="cd852-123">Количество ожидающих устройств</span><span class="sxs-lookup"><span data-stu-id="cd852-123">Number of pending devices</span></span>|
|<span data-ttu-id="cd852-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="cd852-124">notApplicableCount</span></span>|<span data-ttu-id="cd852-125">Int32</span><span class="sxs-lookup"><span data-stu-id="cd852-125">Int32</span></span>|<span data-ttu-id="cd852-126">Количество неприменимых устройств</span><span class="sxs-lookup"><span data-stu-id="cd852-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="cd852-127">successCount</span><span class="sxs-lookup"><span data-stu-id="cd852-127">successCount</span></span>|<span data-ttu-id="cd852-128">Int32</span><span class="sxs-lookup"><span data-stu-id="cd852-128">Int32</span></span>|<span data-ttu-id="cd852-129">Количество успешных устройств</span><span class="sxs-lookup"><span data-stu-id="cd852-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="cd852-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="cd852-130">errorCount</span></span>|<span data-ttu-id="cd852-131">Int32</span><span class="sxs-lookup"><span data-stu-id="cd852-131">Int32</span></span>|<span data-ttu-id="cd852-132">Количество устройств с ошибками</span><span class="sxs-lookup"><span data-stu-id="cd852-132">Number of error devices</span></span>|
|<span data-ttu-id="cd852-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="cd852-133">failedCount</span></span>|<span data-ttu-id="cd852-134">Int32</span><span class="sxs-lookup"><span data-stu-id="cd852-134">Int32</span></span>|<span data-ttu-id="cd852-135">Количество устройств со сбоями</span><span class="sxs-lookup"><span data-stu-id="cd852-135">Number of failed devices</span></span>|
|<span data-ttu-id="cd852-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="cd852-136">lastUpdateDateTime</span></span>|<span data-ttu-id="cd852-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd852-137">DateTimeOffset</span></span>|<span data-ttu-id="cd852-138">Время последнего обновления</span><span class="sxs-lookup"><span data-stu-id="cd852-138">Last update time</span></span>|
|<span data-ttu-id="cd852-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="cd852-139">configurationVersion</span></span>|<span data-ttu-id="cd852-140">Int32</span><span class="sxs-lookup"><span data-stu-id="cd852-140">Int32</span></span>|<span data-ttu-id="cd852-141">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="cd852-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd852-142">Связи</span><span class="sxs-lookup"><span data-stu-id="cd852-142">Relationships</span></span>
<span data-ttu-id="cd852-143">Нет</span><span class="sxs-lookup"><span data-stu-id="cd852-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cd852-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd852-144">JSON Representation</span></span>
<span data-ttu-id="cd852-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd852-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
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



