# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="943b3-101">Create deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="943b3-101">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="943b3-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="943b3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="943b3-103">Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="943b3-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="943b3-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="943b3-104">Prerequisites</span></span>
<span data-ttu-id="943b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="943b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="943b3-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="943b3-107">Permission type</span></span>|<span data-ttu-id="943b3-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="943b3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="943b3-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="943b3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="943b3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="943b3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="943b3-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="943b3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="943b3-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="943b3-112">Not supported.</span></span>|
|<span data-ttu-id="943b3-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="943b3-113">Application</span></span>|<span data-ttu-id="943b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="943b3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="943b3-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="943b3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="943b3-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="943b3-116">Request headers</span></span>
|<span data-ttu-id="943b3-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="943b3-117">Header</span></span>|<span data-ttu-id="943b3-118">Значение</span><span class="sxs-lookup"><span data-stu-id="943b3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="943b3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="943b3-119">Authorization</span></span>|<span data-ttu-id="943b3-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="943b3-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="943b3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="943b3-121">Accept</span></span>|<span data-ttu-id="943b3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="943b3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="943b3-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="943b3-123">Request body</span></span>
<span data-ttu-id="943b3-124">В теле запроса добавьте представление объекта deviceCompliancePolicySettingStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="943b3-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="943b3-125">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="943b3-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="943b3-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="943b3-126">Property</span></span>|<span data-ttu-id="943b3-127">Тип</span><span class="sxs-lookup"><span data-stu-id="943b3-127">Type</span></span>|<span data-ttu-id="943b3-128">Описание</span><span class="sxs-lookup"><span data-stu-id="943b3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="943b3-129">setting</span><span class="sxs-lookup"><span data-stu-id="943b3-129">setting</span></span>|<span data-ttu-id="943b3-130">String</span><span class="sxs-lookup"><span data-stu-id="943b3-130">String</span></span>|<span data-ttu-id="943b3-131">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="943b3-131">The setting class name and property name.</span></span>|
|<span data-ttu-id="943b3-132">settingName</span><span class="sxs-lookup"><span data-stu-id="943b3-132">settingName</span></span>|<span data-ttu-id="943b3-133">String</span><span class="sxs-lookup"><span data-stu-id="943b3-133">String</span></span>|<span data-ttu-id="943b3-134">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="943b3-134">Name of the setting.</span></span>|
|<span data-ttu-id="943b3-135">platformType</span><span class="sxs-lookup"><span data-stu-id="943b3-135">PlatformType</span></span>|<span data-ttu-id="943b3-136">String</span><span class="sxs-lookup"><span data-stu-id="943b3-136">String</span></span>|<span data-ttu-id="943b3-137">Выбор платформы. Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span><span class="sxs-lookup"><span data-stu-id="943b3-137">Setting platform Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="943b3-138">id</span><span class="sxs-lookup"><span data-stu-id="943b3-138">id</span></span>|<span data-ttu-id="943b3-139">String</span><span class="sxs-lookup"><span data-stu-id="943b3-139">String</span></span>|<span data-ttu-id="943b3-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="943b3-140">Key of the setting.</span></span>|
|<span data-ttu-id="943b3-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="943b3-141">unknownDeviceCount</span></span>|<span data-ttu-id="943b3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="943b3-142">Int32</span></span>|<span data-ttu-id="943b3-143">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="943b3-143">Number of unknown devices</span></span>|
|<span data-ttu-id="943b3-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="943b3-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="943b3-145">Int32</span><span class="sxs-lookup"><span data-stu-id="943b3-145">Int32</span></span>|<span data-ttu-id="943b3-146">Количество неприменимых устройств</span><span class="sxs-lookup"><span data-stu-id="943b3-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="943b3-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="943b3-147">compliantDeviceCount</span></span>|<span data-ttu-id="943b3-148">Int32</span><span class="sxs-lookup"><span data-stu-id="943b3-148">Int32</span></span>|<span data-ttu-id="943b3-149">Количество устройств, соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="943b3-149">Number of compliant devices</span></span>|
|<span data-ttu-id="943b3-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="943b3-150">remediatedDeviceCount</span></span>|<span data-ttu-id="943b3-151">Int32</span><span class="sxs-lookup"><span data-stu-id="943b3-151">Int32</span></span>|<span data-ttu-id="943b3-152">Количество исправленных устройств</span><span class="sxs-lookup"><span data-stu-id="943b3-152">Number of remediated devices</span></span>|
|<span data-ttu-id="943b3-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="943b3-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="943b3-154">Int32</span><span class="sxs-lookup"><span data-stu-id="943b3-154">Int32</span></span>|<span data-ttu-id="943b3-155">Количество устройств, не соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="943b3-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="943b3-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="943b3-156">errorDeviceCount</span></span>|<span data-ttu-id="943b3-157">Int32</span><span class="sxs-lookup"><span data-stu-id="943b3-157">Int32</span></span>|<span data-ttu-id="943b3-158">Количество устройств с ошибками</span><span class="sxs-lookup"><span data-stu-id="943b3-158">Number of error devices</span></span>|
|<span data-ttu-id="943b3-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="943b3-159">conflictDeviceCount</span></span>|<span data-ttu-id="943b3-160">Int32</span><span class="sxs-lookup"><span data-stu-id="943b3-160">Int32</span></span>|<span data-ttu-id="943b3-161">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="943b3-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="943b3-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="943b3-162">Response</span></span>
<span data-ttu-id="943b3-163">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="943b3-163">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="943b3-164">Пример</span><span class="sxs-lookup"><span data-stu-id="943b3-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="943b3-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="943b3-165">Request</span></span>
<span data-ttu-id="943b3-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="943b3-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="943b3-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="943b3-167">Response</span></span>
<span data-ttu-id="943b3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="943b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



