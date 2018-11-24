# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="99fb9-101">Тип ресурса deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="99fb9-101">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="99fb9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="99fb9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99fb9-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="99fb9-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="99fb9-104">Методы</span><span class="sxs-lookup"><span data-stu-id="99fb9-104">Methods</span></span>
|<span data-ttu-id="99fb9-105">Метод</span><span class="sxs-lookup"><span data-stu-id="99fb9-105">Method</span></span>|<span data-ttu-id="99fb9-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="99fb9-106">Return Type</span></span>|<span data-ttu-id="99fb9-107">Описание</span><span class="sxs-lookup"><span data-stu-id="99fb9-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="99fb9-108">Получение объекта deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="99fb9-108">Get deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_get.md)|[<span data-ttu-id="99fb9-109">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="99fb9-109">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="99fb9-110">Чтение свойств и связей объекта [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="99fb9-110">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="99fb9-111">Обновление объекта deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="99fb9-111">Update deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_update.md)|[<span data-ttu-id="99fb9-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="99fb9-112">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="99fb9-113">Обновление свойств объекта [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="99fb9-113">Update the properties of a [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="99fb9-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="99fb9-114">Properties</span></span>
|<span data-ttu-id="99fb9-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="99fb9-115">Property</span></span>|<span data-ttu-id="99fb9-116">Тип</span><span class="sxs-lookup"><span data-stu-id="99fb9-116">Type</span></span>|<span data-ttu-id="99fb9-117">Описание</span><span class="sxs-lookup"><span data-stu-id="99fb9-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99fb9-118">id</span><span class="sxs-lookup"><span data-stu-id="99fb9-118">id</span></span>|<span data-ttu-id="99fb9-119">String</span><span class="sxs-lookup"><span data-stu-id="99fb9-119">String</span></span>|<span data-ttu-id="99fb9-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="99fb9-120">Key of the entity.</span></span>|
|<span data-ttu-id="99fb9-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="99fb9-121">pendingCount</span></span>|<span data-ttu-id="99fb9-122">Int32</span><span class="sxs-lookup"><span data-stu-id="99fb9-122">Int32</span></span>|<span data-ttu-id="99fb9-123">Количество ожидающих пользователей</span><span class="sxs-lookup"><span data-stu-id="99fb9-123">Number of pending Users</span></span>|
|<span data-ttu-id="99fb9-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="99fb9-124">notApplicableCount</span></span>|<span data-ttu-id="99fb9-125">Int32</span><span class="sxs-lookup"><span data-stu-id="99fb9-125">Int32</span></span>|<span data-ttu-id="99fb9-126">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="99fb9-126">Number of not applicable users</span></span>|
|<span data-ttu-id="99fb9-127">successCount</span><span class="sxs-lookup"><span data-stu-id="99fb9-127">successCount</span></span>|<span data-ttu-id="99fb9-128">Int32</span><span class="sxs-lookup"><span data-stu-id="99fb9-128">Int32</span></span>|<span data-ttu-id="99fb9-129">Количество успешных пользователей</span><span class="sxs-lookup"><span data-stu-id="99fb9-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="99fb9-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="99fb9-130">errorCount</span></span>|<span data-ttu-id="99fb9-131">Int32</span><span class="sxs-lookup"><span data-stu-id="99fb9-131">Int32</span></span>|<span data-ttu-id="99fb9-132">Количество пользователей с устройствами</span><span class="sxs-lookup"><span data-stu-id="99fb9-132">Number of error Users</span></span>|
|<span data-ttu-id="99fb9-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="99fb9-133">failedCount</span></span>|<span data-ttu-id="99fb9-134">Int32</span><span class="sxs-lookup"><span data-stu-id="99fb9-134">Int32</span></span>|<span data-ttu-id="99fb9-135">Количество пользователей со сбоями</span><span class="sxs-lookup"><span data-stu-id="99fb9-135">Number of failed Users</span></span>|
|<span data-ttu-id="99fb9-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="99fb9-136">lastUpdateDateTime</span></span>|<span data-ttu-id="99fb9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99fb9-137">DateTimeOffset</span></span>|<span data-ttu-id="99fb9-138">Время последнего обновления</span><span class="sxs-lookup"><span data-stu-id="99fb9-138">Last update time</span></span>|
|<span data-ttu-id="99fb9-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="99fb9-139">configurationVersion</span></span>|<span data-ttu-id="99fb9-140">Int32</span><span class="sxs-lookup"><span data-stu-id="99fb9-140">Int32</span></span>|<span data-ttu-id="99fb9-141">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="99fb9-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="99fb9-142">Связи</span><span class="sxs-lookup"><span data-stu-id="99fb9-142">Relationships</span></span>
<span data-ttu-id="99fb9-143">Нет</span><span class="sxs-lookup"><span data-stu-id="99fb9-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="99fb9-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99fb9-144">JSON Representation</span></span>
<span data-ttu-id="99fb9-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99fb9-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
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



