# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="72166-101">Тип ресурса deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="72166-101">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="72166-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="72166-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72166-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="72166-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="72166-104">Методы</span><span class="sxs-lookup"><span data-stu-id="72166-104">Methods</span></span>
|<span data-ttu-id="72166-105">Метод</span><span class="sxs-lookup"><span data-stu-id="72166-105">Method</span></span>|<span data-ttu-id="72166-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72166-106">Return Type</span></span>|<span data-ttu-id="72166-107">Описание</span><span class="sxs-lookup"><span data-stu-id="72166-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="72166-108">Получение объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="72166-108">Get deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_get.md)|[<span data-ttu-id="72166-109">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="72166-109">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="72166-110">Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="72166-110">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="72166-111">Обновление объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="72166-111">Update deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_update.md)|[<span data-ttu-id="72166-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="72166-112">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="72166-113">Обновление свойств объекта [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="72166-113">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="72166-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="72166-114">Properties</span></span>
|<span data-ttu-id="72166-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="72166-115">Property</span></span>|<span data-ttu-id="72166-116">Тип</span><span class="sxs-lookup"><span data-stu-id="72166-116">Type</span></span>|<span data-ttu-id="72166-117">Описание</span><span class="sxs-lookup"><span data-stu-id="72166-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72166-118">id</span><span class="sxs-lookup"><span data-stu-id="72166-118">id</span></span>|<span data-ttu-id="72166-119">String</span><span class="sxs-lookup"><span data-stu-id="72166-119">String</span></span>|<span data-ttu-id="72166-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="72166-120">Key of the setting.</span></span>|
|<span data-ttu-id="72166-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="72166-121">pendingCount</span></span>|<span data-ttu-id="72166-122">Int32</span><span class="sxs-lookup"><span data-stu-id="72166-122">Int32</span></span>|<span data-ttu-id="72166-123">Количество ожидающих пользователей</span><span class="sxs-lookup"><span data-stu-id="72166-123">Number of pending Users</span></span>|
|<span data-ttu-id="72166-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="72166-124">notApplicableCount</span></span>|<span data-ttu-id="72166-125">Int32</span><span class="sxs-lookup"><span data-stu-id="72166-125">Int32</span></span>|<span data-ttu-id="72166-126">Количество неприменимых устройств</span><span class="sxs-lookup"><span data-stu-id="72166-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="72166-127">successCount</span><span class="sxs-lookup"><span data-stu-id="72166-127">successCount</span></span>|<span data-ttu-id="72166-128">Int32</span><span class="sxs-lookup"><span data-stu-id="72166-128">Int32</span></span>|<span data-ttu-id="72166-129">Количество успешных пользователей</span><span class="sxs-lookup"><span data-stu-id="72166-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="72166-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="72166-130">errorCount</span></span>|<span data-ttu-id="72166-131">Int32</span><span class="sxs-lookup"><span data-stu-id="72166-131">Int32</span></span>|<span data-ttu-id="72166-132">Количество пользователей с устройствами</span><span class="sxs-lookup"><span data-stu-id="72166-132">Number of error Users</span></span>|
|<span data-ttu-id="72166-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="72166-133">failedCount</span></span>|<span data-ttu-id="72166-134">Int32</span><span class="sxs-lookup"><span data-stu-id="72166-134">Int32</span></span>|<span data-ttu-id="72166-135">Количество пользователей со сбоями</span><span class="sxs-lookup"><span data-stu-id="72166-135">Number of failed Users</span></span>|
|<span data-ttu-id="72166-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="72166-136">lastUpdateDateTime</span></span>|<span data-ttu-id="72166-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72166-137">DateTimeOffset</span></span>|<span data-ttu-id="72166-138">Время последнего обновления</span><span class="sxs-lookup"><span data-stu-id="72166-138">Last update time</span></span>|
|<span data-ttu-id="72166-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="72166-139">configurationVersion</span></span>|<span data-ttu-id="72166-140">Int32</span><span class="sxs-lookup"><span data-stu-id="72166-140">Int32</span></span>|<span data-ttu-id="72166-141">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="72166-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="72166-142">Связи</span><span class="sxs-lookup"><span data-stu-id="72166-142">Relationships</span></span>
<span data-ttu-id="72166-143">Нет</span><span class="sxs-lookup"><span data-stu-id="72166-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="72166-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72166-144">JSON Representation</span></span>
<span data-ttu-id="72166-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72166-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
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



