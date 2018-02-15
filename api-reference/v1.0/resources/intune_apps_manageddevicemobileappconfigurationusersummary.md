# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="066b5-101">Тип ресурса managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="066b5-101">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="066b5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="066b5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="066b5-103">Содержит свойства, унаследованные свойства и действия из сводки по состоянию конфигурации мобильных приложений MDM для пользователя.</span><span class="sxs-lookup"><span data-stu-id="066b5-103">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="066b5-104">Методы</span><span class="sxs-lookup"><span data-stu-id="066b5-104">Methods</span></span>
|<span data-ttu-id="066b5-105">Метод</span><span class="sxs-lookup"><span data-stu-id="066b5-105">Method</span></span>|<span data-ttu-id="066b5-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="066b5-106">Return Type</span></span>|<span data-ttu-id="066b5-107">Описание</span><span class="sxs-lookup"><span data-stu-id="066b5-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="066b5-108">Получение объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="066b5-108">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_get.md)|[<span data-ttu-id="066b5-109">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="066b5-109">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="066b5-110">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="066b5-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="066b5-111">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="066b5-111">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_update.md)|[<span data-ttu-id="066b5-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="066b5-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="066b5-113">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="066b5-113">Update the properties of a [calendar](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="066b5-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="066b5-114">Properties</span></span>
|<span data-ttu-id="066b5-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="066b5-115">Property</span></span>|<span data-ttu-id="066b5-116">Тип</span><span class="sxs-lookup"><span data-stu-id="066b5-116">Type</span></span>|<span data-ttu-id="066b5-117">Описание</span><span class="sxs-lookup"><span data-stu-id="066b5-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="066b5-118">id</span><span class="sxs-lookup"><span data-stu-id="066b5-118">id</span></span>|<span data-ttu-id="066b5-119">String</span><span class="sxs-lookup"><span data-stu-id="066b5-119">String</span></span>|<span data-ttu-id="066b5-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="066b5-120">Key of the setting.</span></span>|
|<span data-ttu-id="066b5-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="066b5-121">pendingCount</span></span>|<span data-ttu-id="066b5-122">Int32</span><span class="sxs-lookup"><span data-stu-id="066b5-122">Int32</span></span>|<span data-ttu-id="066b5-123">Количество ожидающих пользователей</span><span class="sxs-lookup"><span data-stu-id="066b5-123">Number of pending Users</span></span>|
|<span data-ttu-id="066b5-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="066b5-124">notApplicableCount</span></span>|<span data-ttu-id="066b5-125">Int32</span><span class="sxs-lookup"><span data-stu-id="066b5-125">Int32</span></span>|<span data-ttu-id="066b5-126">Количество неприменимых устройств</span><span class="sxs-lookup"><span data-stu-id="066b5-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="066b5-127">successCount</span><span class="sxs-lookup"><span data-stu-id="066b5-127">successCount</span></span>|<span data-ttu-id="066b5-128">Int32</span><span class="sxs-lookup"><span data-stu-id="066b5-128">Int32</span></span>|<span data-ttu-id="066b5-129">Количество успешных пользователей</span><span class="sxs-lookup"><span data-stu-id="066b5-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="066b5-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="066b5-130">errorCount</span></span>|<span data-ttu-id="066b5-131">Int32</span><span class="sxs-lookup"><span data-stu-id="066b5-131">Int32</span></span>|<span data-ttu-id="066b5-132">Количество пользователей с устройствами</span><span class="sxs-lookup"><span data-stu-id="066b5-132">Number of error Users</span></span>|
|<span data-ttu-id="066b5-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="066b5-133">failedCount</span></span>|<span data-ttu-id="066b5-134">Int32</span><span class="sxs-lookup"><span data-stu-id="066b5-134">Int32</span></span>|<span data-ttu-id="066b5-135">Количество пользователей со сбоями</span><span class="sxs-lookup"><span data-stu-id="066b5-135">Number of failed Users</span></span>|
|<span data-ttu-id="066b5-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="066b5-136">lastUpdateDateTime</span></span>|<span data-ttu-id="066b5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="066b5-137">DateTimeOffset</span></span>|<span data-ttu-id="066b5-138">Время последнего обновления</span><span class="sxs-lookup"><span data-stu-id="066b5-138">Last update time</span></span>|
|<span data-ttu-id="066b5-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="066b5-139">configurationVersion</span></span>|<span data-ttu-id="066b5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="066b5-140">Int32</span></span>|<span data-ttu-id="066b5-141">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="066b5-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="066b5-142">Связи</span><span class="sxs-lookup"><span data-stu-id="066b5-142">Relationships</span></span>
<span data-ttu-id="066b5-143">Нет</span><span class="sxs-lookup"><span data-stu-id="066b5-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="066b5-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="066b5-144">JSON Representation</span></span>
<span data-ttu-id="066b5-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="066b5-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
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



