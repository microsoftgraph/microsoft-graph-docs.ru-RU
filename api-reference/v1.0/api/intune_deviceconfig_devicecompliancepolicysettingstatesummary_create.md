# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="39b8b-101">Создание объекта deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="39b8b-101">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="39b8b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="39b8b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39b8b-103">Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="39b8b-103">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39b8b-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="39b8b-104">Prerequisites</span></span>
<span data-ttu-id="39b8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="39b8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="39b8b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39b8b-107">Permission type</span></span>|<span data-ttu-id="39b8b-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39b8b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39b8b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39b8b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="39b8b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39b8b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39b8b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39b8b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39b8b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39b8b-112">Not supported.</span></span>|
|<span data-ttu-id="39b8b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39b8b-113">Application</span></span>|<span data-ttu-id="39b8b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39b8b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39b8b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39b8b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="39b8b-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39b8b-116">Request headers</span></span>
|<span data-ttu-id="39b8b-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39b8b-117">Header</span></span>|<span data-ttu-id="39b8b-118">Значение</span><span class="sxs-lookup"><span data-stu-id="39b8b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39b8b-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39b8b-119">Authorization</span></span>|<span data-ttu-id="39b8b-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="39b8b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39b8b-121">Подтверждение</span><span class="sxs-lookup"><span data-stu-id="39b8b-121">Accept</span></span>|<span data-ttu-id="39b8b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="39b8b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39b8b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39b8b-123">Request body</span></span>
<span data-ttu-id="39b8b-124">В теле запроса добавьте представление объекта deviceCompliancePolicySettingStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39b8b-124">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="39b8b-125">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="39b8b-125">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="39b8b-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="39b8b-126">Property</span></span>|<span data-ttu-id="39b8b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="39b8b-127">Type</span></span>|<span data-ttu-id="39b8b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="39b8b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39b8b-129">setting</span><span class="sxs-lookup"><span data-stu-id="39b8b-129">setting</span></span>|<span data-ttu-id="39b8b-130">String</span><span class="sxs-lookup"><span data-stu-id="39b8b-130">String</span></span>|<span data-ttu-id="39b8b-131">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="39b8b-131">The setting class name and property name.</span></span>|
|<span data-ttu-id="39b8b-132">settingName</span><span class="sxs-lookup"><span data-stu-id="39b8b-132">settingName</span></span>|<span data-ttu-id="39b8b-133">String</span><span class="sxs-lookup"><span data-stu-id="39b8b-133">String</span></span>|<span data-ttu-id="39b8b-134">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="39b8b-134">Name of the setting.</span></span>|
|<span data-ttu-id="39b8b-135">platformType</span><span class="sxs-lookup"><span data-stu-id="39b8b-135">platformType</span></span>|[<span data-ttu-id="39b8b-136">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="39b8b-136">policyPlatformType</span></span>](../resources/intune_deviceconfig_policyplatformtype.md)|<span data-ttu-id="39b8b-137">Платформа настройки.</span><span class="sxs-lookup"><span data-stu-id="39b8b-137">Setting platform.</span></span> <span data-ttu-id="39b8b-138">Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="39b8b-138">The possible values are `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`, , , , or .</span></span>|
|<span data-ttu-id="39b8b-139">id</span><span class="sxs-lookup"><span data-stu-id="39b8b-139">id</span></span>|<span data-ttu-id="39b8b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="39b8b-140">String</span></span>|<span data-ttu-id="39b8b-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="39b8b-141">Key of the entity.</span></span>|
|<span data-ttu-id="39b8b-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39b8b-142">unknownDeviceCount</span></span>|<span data-ttu-id="39b8b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="39b8b-143">Int32</span></span>|<span data-ttu-id="39b8b-144">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="39b8b-144">Number of unknown devices</span></span>|
|<span data-ttu-id="39b8b-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39b8b-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="39b8b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="39b8b-146">Int32</span></span>|<span data-ttu-id="39b8b-147">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="39b8b-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="39b8b-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39b8b-148">compliantDeviceCount</span></span>|<span data-ttu-id="39b8b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="39b8b-149">Int32</span></span>|<span data-ttu-id="39b8b-150">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="39b8b-150">Number of compliant devices</span></span>|
|<span data-ttu-id="39b8b-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39b8b-151">remediatedDeviceCount</span></span>|<span data-ttu-id="39b8b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="39b8b-152">Int32</span></span>|<span data-ttu-id="39b8b-153">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="39b8b-153">Number of remediated devices</span></span>|
|<span data-ttu-id="39b8b-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39b8b-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="39b8b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="39b8b-155">Int32</span></span>|<span data-ttu-id="39b8b-156">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="39b8b-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="39b8b-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39b8b-157">errorDeviceCount</span></span>|<span data-ttu-id="39b8b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="39b8b-158">Int32</span></span>|<span data-ttu-id="39b8b-159">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="39b8b-159">Number of error devices</span></span>|
|<span data-ttu-id="39b8b-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39b8b-160">conflictDeviceCount</span></span>|<span data-ttu-id="39b8b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="39b8b-161">Int32</span></span>|<span data-ttu-id="39b8b-162">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="39b8b-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="39b8b-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="39b8b-163">Response</span></span>
<span data-ttu-id="39b8b-164">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="39b8b-164">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39b8b-165">Пример</span><span class="sxs-lookup"><span data-stu-id="39b8b-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="39b8b-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="39b8b-166">Request</span></span>
<span data-ttu-id="39b8b-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39b8b-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="39b8b-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="39b8b-168">Response</span></span>
<span data-ttu-id="39b8b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39b8b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



