# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="dd05f-101">Тип ресурса softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="dd05f-101">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="dd05f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dd05f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd05f-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dd05f-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="dd05f-104">Методы</span><span class="sxs-lookup"><span data-stu-id="dd05f-104">Methods</span></span>
|<span data-ttu-id="dd05f-105">Метод</span><span class="sxs-lookup"><span data-stu-id="dd05f-105">Method</span></span>|<span data-ttu-id="dd05f-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dd05f-106">Return Type</span></span>|<span data-ttu-id="dd05f-107">Описание</span><span class="sxs-lookup"><span data-stu-id="dd05f-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dd05f-108">Получение объекта softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="dd05f-108">Get softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_get.md)|[<span data-ttu-id="dd05f-109">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="dd05f-109">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="dd05f-110">Чтение свойств и связей объекта [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="dd05f-110">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="dd05f-111">Обновление объекта softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="dd05f-111">Update softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_update.md)|[<span data-ttu-id="dd05f-112">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="dd05f-112">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="dd05f-113">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="dd05f-113">Update the properties of a [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dd05f-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd05f-114">Properties</span></span>
|<span data-ttu-id="dd05f-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd05f-115">Property</span></span>|<span data-ttu-id="dd05f-116">Тип</span><span class="sxs-lookup"><span data-stu-id="dd05f-116">Type</span></span>|<span data-ttu-id="dd05f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="dd05f-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd05f-118">id</span><span class="sxs-lookup"><span data-stu-id="dd05f-118">id</span></span>|<span data-ttu-id="dd05f-119">String</span><span class="sxs-lookup"><span data-stu-id="dd05f-119">String</span></span>|<span data-ttu-id="dd05f-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd05f-120">Key of the entity.</span></span>|
|<span data-ttu-id="dd05f-121">displayName</span><span class="sxs-lookup"><span data-stu-id="dd05f-121">displayName</span></span>|<span data-ttu-id="dd05f-122">String</span><span class="sxs-lookup"><span data-stu-id="dd05f-122">String</span></span>|<span data-ttu-id="dd05f-123">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="dd05f-123">The name of the policy.</span></span>|
|<span data-ttu-id="dd05f-124">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-124">compliantDeviceCount</span></span>|<span data-ttu-id="dd05f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-125">Int32</span></span>|<span data-ttu-id="dd05f-126">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="dd05f-126">Number of compliant devices.</span></span>|
|<span data-ttu-id="dd05f-127">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-127">nonCompliantDeviceCount</span></span>|<span data-ttu-id="dd05f-128">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-128">Int32</span></span>|<span data-ttu-id="dd05f-129">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="dd05f-129">Number of non compliant devices.</span></span>|
|<span data-ttu-id="dd05f-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-130">remediatedDeviceCount</span></span>|<span data-ttu-id="dd05f-131">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-131">Int32</span></span>|<span data-ttu-id="dd05f-132">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="dd05f-132">Number of remediated devices.</span></span>|
|<span data-ttu-id="dd05f-133">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-133">errorDeviceCount</span></span>|<span data-ttu-id="dd05f-134">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-134">Int32</span></span>|<span data-ttu-id="dd05f-135">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="dd05f-135">Number of devices had error.</span></span>|
|<span data-ttu-id="dd05f-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-136">unknownDeviceCount</span></span>|<span data-ttu-id="dd05f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-137">Int32</span></span>|<span data-ttu-id="dd05f-138">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="dd05f-138">Number of unknown devices.</span></span>|
|<span data-ttu-id="dd05f-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-139">conflictDeviceCount</span></span>|<span data-ttu-id="dd05f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-140">Int32</span></span>|<span data-ttu-id="dd05f-141">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="dd05f-141">Number of conflict devices.</span></span>|
|<span data-ttu-id="dd05f-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="dd05f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-143">Int32</span></span>|<span data-ttu-id="dd05f-144">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="dd05f-144">Number of not applicable devices.</span></span>|
|<span data-ttu-id="dd05f-145">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-145">compliantUserCount</span></span>|<span data-ttu-id="dd05f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-146">Int32</span></span>|<span data-ttu-id="dd05f-147">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="dd05f-147">Number of compliant users.</span></span>|
|<span data-ttu-id="dd05f-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-148">nonCompliantUserCount</span></span>|<span data-ttu-id="dd05f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-149">Int32</span></span>|<span data-ttu-id="dd05f-150">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="dd05f-150">Number of non compliant users.</span></span>|
|<span data-ttu-id="dd05f-151">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-151">remediatedUserCount</span></span>|<span data-ttu-id="dd05f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-152">Int32</span></span>|<span data-ttu-id="dd05f-153">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="dd05f-153">Number of remediated users.</span></span>|
|<span data-ttu-id="dd05f-154">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-154">errorUserCount</span></span>|<span data-ttu-id="dd05f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-155">Int32</span></span>|<span data-ttu-id="dd05f-156">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="dd05f-156">Number of users had error.</span></span>|
|<span data-ttu-id="dd05f-157">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-157">unknownUserCount</span></span>|<span data-ttu-id="dd05f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-158">Int32</span></span>|<span data-ttu-id="dd05f-159">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="dd05f-159">Number of unknown users.</span></span>|
|<span data-ttu-id="dd05f-160">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-160">conflictUserCount</span></span>|<span data-ttu-id="dd05f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-161">Int32</span></span>|<span data-ttu-id="dd05f-162">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="dd05f-162">Number of conflict users.</span></span>|
|<span data-ttu-id="dd05f-163">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="dd05f-163">notApplicableUserCount</span></span>|<span data-ttu-id="dd05f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="dd05f-164">Int32</span></span>|<span data-ttu-id="dd05f-165">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="dd05f-165">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd05f-166">Связи</span><span class="sxs-lookup"><span data-stu-id="dd05f-166">Relationships</span></span>
<span data-ttu-id="dd05f-167">Нет</span><span class="sxs-lookup"><span data-stu-id="dd05f-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dd05f-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd05f-168">JSON Representation</span></span>
<span data-ttu-id="dd05f-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd05f-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```



