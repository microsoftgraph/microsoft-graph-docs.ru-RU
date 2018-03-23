# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="65fa8-101">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="65fa8-101">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="65fa8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="65fa8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65fa8-103">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="65fa8-103">Update the properties of a [calendar](../resources/intune_deviceconfig_settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65fa8-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="65fa8-104">Prerequisites</span></span>
<span data-ttu-id="65fa8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65fa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65fa8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65fa8-107">Permission type</span></span>|<span data-ttu-id="65fa8-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65fa8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65fa8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65fa8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="65fa8-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65fa8-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65fa8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65fa8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65fa8-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65fa8-112">Not supported.</span></span>|
|<span data-ttu-id="65fa8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65fa8-113">Application</span></span>|<span data-ttu-id="65fa8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65fa8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65fa8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65fa8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="65fa8-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65fa8-116">Request headers</span></span>
|<span data-ttu-id="65fa8-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65fa8-117">Header</span></span>|<span data-ttu-id="65fa8-118">Значение</span><span class="sxs-lookup"><span data-stu-id="65fa8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65fa8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="65fa8-119">Authorization</span></span>|<span data-ttu-id="65fa8-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65fa8-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="65fa8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="65fa8-121">Accept</span></span>|<span data-ttu-id="65fa8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="65fa8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65fa8-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65fa8-123">Request body</span></span>
<span data-ttu-id="65fa8-124">В теле запроса добавьте представление объекта [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65fa8-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="65fa8-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="65fa8-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="65fa8-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="65fa8-126">Property</span></span>|<span data-ttu-id="65fa8-127">Тип</span><span class="sxs-lookup"><span data-stu-id="65fa8-127">Type</span></span>|<span data-ttu-id="65fa8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="65fa8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65fa8-129">id</span><span class="sxs-lookup"><span data-stu-id="65fa8-129">id</span></span>|<span data-ttu-id="65fa8-130">String</span><span class="sxs-lookup"><span data-stu-id="65fa8-130">String</span></span>|<span data-ttu-id="65fa8-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="65fa8-131">Key of the setting.</span></span>|
|<span data-ttu-id="65fa8-132">settingName</span><span class="sxs-lookup"><span data-stu-id="65fa8-132">settingName</span></span>|<span data-ttu-id="65fa8-133">String</span><span class="sxs-lookup"><span data-stu-id="65fa8-133">String</span></span>|<span data-ttu-id="65fa8-134">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="65fa8-134">Name of the setting.</span></span>|
|<span data-ttu-id="65fa8-135">instancePath</span><span class="sxs-lookup"><span data-stu-id="65fa8-135">instancePath</span></span>|<span data-ttu-id="65fa8-136">String</span><span class="sxs-lookup"><span data-stu-id="65fa8-136">String</span></span>|<span data-ttu-id="65fa8-137">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="65fa8-137">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="65fa8-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65fa8-138">unknownDeviceCount</span></span>|<span data-ttu-id="65fa8-139">Int32</span><span class="sxs-lookup"><span data-stu-id="65fa8-139">Int32</span></span>|<span data-ttu-id="65fa8-140">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="65fa8-140">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="65fa8-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65fa8-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="65fa8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="65fa8-142">Int32</span></span>|<span data-ttu-id="65fa8-143">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="65fa8-143">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="65fa8-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65fa8-144">compliantDeviceCount</span></span>|<span data-ttu-id="65fa8-145">Int32</span><span class="sxs-lookup"><span data-stu-id="65fa8-145">Int32</span></span>|<span data-ttu-id="65fa8-146">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="65fa8-146">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="65fa8-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65fa8-147">remediatedDeviceCount</span></span>|<span data-ttu-id="65fa8-148">Int32</span><span class="sxs-lookup"><span data-stu-id="65fa8-148">Int32</span></span>|<span data-ttu-id="65fa8-149">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="65fa8-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="65fa8-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65fa8-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="65fa8-151">Int32</span><span class="sxs-lookup"><span data-stu-id="65fa8-151">Int32</span></span>|<span data-ttu-id="65fa8-152">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="65fa8-152">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="65fa8-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65fa8-153">errorDeviceCount</span></span>|<span data-ttu-id="65fa8-154">Int32</span><span class="sxs-lookup"><span data-stu-id="65fa8-154">Int32</span></span>|<span data-ttu-id="65fa8-155">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="65fa8-155">Device error count for the setting</span></span>|
|<span data-ttu-id="65fa8-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65fa8-156">conflictDeviceCount</span></span>|<span data-ttu-id="65fa8-157">Int32</span><span class="sxs-lookup"><span data-stu-id="65fa8-157">Int32</span></span>|<span data-ttu-id="65fa8-158">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="65fa8-158">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="65fa8-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="65fa8-159">Response</span></span>
<span data-ttu-id="65fa8-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="65fa8-160">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65fa8-161">Пример</span><span class="sxs-lookup"><span data-stu-id="65fa8-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="65fa8-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="65fa8-162">Request</span></span>
<span data-ttu-id="65fa8-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65fa8-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 296

{
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="65fa8-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="65fa8-164">Response</span></span>
<span data-ttu-id="65fa8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="65fa8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



