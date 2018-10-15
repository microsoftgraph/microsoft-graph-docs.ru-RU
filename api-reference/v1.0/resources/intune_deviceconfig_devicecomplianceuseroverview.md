# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="4d361-101">Тип ресурса deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="4d361-101">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="4d361-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4d361-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d361-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4d361-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="4d361-104">Методы</span><span class="sxs-lookup"><span data-stu-id="4d361-104">Methods</span></span>
|<span data-ttu-id="4d361-105">Метод</span><span class="sxs-lookup"><span data-stu-id="4d361-105">Method</span></span>|<span data-ttu-id="4d361-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4d361-106">Return Type</span></span>|<span data-ttu-id="4d361-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4d361-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4d361-108">Получение объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="4d361-108">Get deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_get.md)|[<span data-ttu-id="4d361-109">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="4d361-109">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="4d361-110">Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="4d361-110">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="4d361-111">Обновление объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="4d361-111">Update deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_update.md)|[<span data-ttu-id="4d361-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="4d361-112">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="4d361-113">Обновление свойств объекта [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="4d361-113">Update the properties of a [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4d361-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d361-114">Properties</span></span>
|<span data-ttu-id="4d361-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d361-115">Property</span></span>|<span data-ttu-id="4d361-116">Тип</span><span class="sxs-lookup"><span data-stu-id="4d361-116">Type</span></span>|<span data-ttu-id="4d361-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4d361-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d361-118">id</span><span class="sxs-lookup"><span data-stu-id="4d361-118">id</span></span>|<span data-ttu-id="4d361-119">Строка</span><span class="sxs-lookup"><span data-stu-id="4d361-119">String</span></span>|<span data-ttu-id="4d361-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4d361-120">Key of the entity.</span></span>|
|<span data-ttu-id="4d361-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="4d361-121">pendingCount</span></span>|<span data-ttu-id="4d361-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4d361-122">Int32</span></span>|<span data-ttu-id="4d361-123">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="4d361-123">Number of pending Users</span></span>|
|<span data-ttu-id="4d361-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4d361-124">notApplicableCount</span></span>|<span data-ttu-id="4d361-125">Int32</span><span class="sxs-lookup"><span data-stu-id="4d361-125">Int32</span></span>|<span data-ttu-id="4d361-126">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="4d361-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="4d361-127">successCount</span><span class="sxs-lookup"><span data-stu-id="4d361-127">successCount</span></span>|<span data-ttu-id="4d361-128">Int32</span><span class="sxs-lookup"><span data-stu-id="4d361-128">Int32</span></span>|<span data-ttu-id="4d361-129">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="4d361-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="4d361-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="4d361-130">errorCount</span></span>|<span data-ttu-id="4d361-131">Int32</span><span class="sxs-lookup"><span data-stu-id="4d361-131">Int32</span></span>|<span data-ttu-id="4d361-132">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="4d361-132">Number of error Users</span></span>|
|<span data-ttu-id="4d361-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="4d361-133">failedCount</span></span>|<span data-ttu-id="4d361-134">Int32</span><span class="sxs-lookup"><span data-stu-id="4d361-134">Int32</span></span>|<span data-ttu-id="4d361-135">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="4d361-135">Number of failed Users</span></span>|
|<span data-ttu-id="4d361-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4d361-136">lastUpdateDateTime</span></span>|<span data-ttu-id="4d361-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d361-137">DateTimeOffset</span></span>|<span data-ttu-id="4d361-138">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="4d361-138">Last update time</span></span>|
|<span data-ttu-id="4d361-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="4d361-139">configurationVersion</span></span>|<span data-ttu-id="4d361-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4d361-140">Int32</span></span>|<span data-ttu-id="4d361-141">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="4d361-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d361-142">Связи</span><span class="sxs-lookup"><span data-stu-id="4d361-142">Relationships</span></span>
<span data-ttu-id="4d361-143">Нет</span><span class="sxs-lookup"><span data-stu-id="4d361-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4d361-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d361-144">JSON Representation</span></span>
<span data-ttu-id="4d361-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d361-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}-->
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



