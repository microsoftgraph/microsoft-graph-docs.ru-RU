# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="56f49-101">Тип ресурса managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="56f49-101">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="56f49-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="56f49-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56f49-103">Содержит свойства, унаследованные свойства и действия из сводки по состоянию конфигурации мобильных приложений MDM для пользователя.</span><span class="sxs-lookup"><span data-stu-id="56f49-103">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="56f49-104">Методы</span><span class="sxs-lookup"><span data-stu-id="56f49-104">Methods</span></span>
|<span data-ttu-id="56f49-105">Метод</span><span class="sxs-lookup"><span data-stu-id="56f49-105">Method</span></span>|<span data-ttu-id="56f49-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="56f49-106">Return Type</span></span>|<span data-ttu-id="56f49-107">Описание</span><span class="sxs-lookup"><span data-stu-id="56f49-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56f49-108">Получение объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="56f49-108">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_get.md)|[<span data-ttu-id="56f49-109">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="56f49-109">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="56f49-110">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="56f49-110">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="56f49-111">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="56f49-111">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_update.md)|[<span data-ttu-id="56f49-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="56f49-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="56f49-113">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="56f49-113">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="56f49-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="56f49-114">Properties</span></span>
|<span data-ttu-id="56f49-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="56f49-115">Property</span></span>|<span data-ttu-id="56f49-116">Тип</span><span class="sxs-lookup"><span data-stu-id="56f49-116">Type</span></span>|<span data-ttu-id="56f49-117">Описание</span><span class="sxs-lookup"><span data-stu-id="56f49-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56f49-118">ИД</span><span class="sxs-lookup"><span data-stu-id="56f49-118">id</span></span>|<span data-ttu-id="56f49-119">Строка</span><span class="sxs-lookup"><span data-stu-id="56f49-119">String</span></span>|<span data-ttu-id="56f49-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="56f49-120">Key of the entity.</span></span>|
|<span data-ttu-id="56f49-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="56f49-121">pendingCount</span></span>|<span data-ttu-id="56f49-122">Int32</span><span class="sxs-lookup"><span data-stu-id="56f49-122">Int32</span></span>|<span data-ttu-id="56f49-123">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="56f49-123">Number of pending Users</span></span>|
|<span data-ttu-id="56f49-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="56f49-124">notApplicableCount</span></span>|<span data-ttu-id="56f49-125">Int32</span><span class="sxs-lookup"><span data-stu-id="56f49-125">Int32</span></span>|<span data-ttu-id="56f49-126">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="56f49-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="56f49-127">successCount</span><span class="sxs-lookup"><span data-stu-id="56f49-127">successCount</span></span>|<span data-ttu-id="56f49-128">Int32</span><span class="sxs-lookup"><span data-stu-id="56f49-128">Int32</span></span>|<span data-ttu-id="56f49-129">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="56f49-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="56f49-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="56f49-130">errorCount</span></span>|<span data-ttu-id="56f49-131">Int32</span><span class="sxs-lookup"><span data-stu-id="56f49-131">Int32</span></span>|<span data-ttu-id="56f49-132">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="56f49-132">Number of error Users</span></span>|
|<span data-ttu-id="56f49-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="56f49-133">failedCount</span></span>|<span data-ttu-id="56f49-134">Int32</span><span class="sxs-lookup"><span data-stu-id="56f49-134">Int32</span></span>|<span data-ttu-id="56f49-135">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="56f49-135">Number of failed Users</span></span>|
|<span data-ttu-id="56f49-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="56f49-136">lastUpdateDateTime</span></span>|<span data-ttu-id="56f49-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56f49-137">DateTimeOffset</span></span>|<span data-ttu-id="56f49-138">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="56f49-138">Last update time</span></span>|
|<span data-ttu-id="56f49-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="56f49-139">configurationVersion</span></span>|<span data-ttu-id="56f49-140">Int32</span><span class="sxs-lookup"><span data-stu-id="56f49-140">Int32</span></span>|<span data-ttu-id="56f49-141">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="56f49-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="56f49-142">Связи</span><span class="sxs-lookup"><span data-stu-id="56f49-142">Relationships</span></span>
<span data-ttu-id="56f49-143">Нет</span><span class="sxs-lookup"><span data-stu-id="56f49-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="56f49-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56f49-144">JSON Representation</span></span>
<span data-ttu-id="56f49-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56f49-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}-->
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








