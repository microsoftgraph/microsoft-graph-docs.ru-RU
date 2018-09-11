# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="0479e-101">Создание объекта deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="0479e-101">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="0479e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0479e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0479e-103">Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0479e-103">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0479e-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0479e-104">Prerequisites</span></span>
<span data-ttu-id="0479e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0479e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0479e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0479e-107">Permission type</span></span>|<span data-ttu-id="0479e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0479e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0479e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0479e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0479e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0479e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0479e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0479e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0479e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0479e-112">Not supported.</span></span>|
|<span data-ttu-id="0479e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0479e-113">Application</span></span>|<span data-ttu-id="0479e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0479e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0479e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0479e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="0479e-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0479e-116">Request headers</span></span>
|<span data-ttu-id="0479e-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0479e-117">Header</span></span>|<span data-ttu-id="0479e-118">Значение</span><span class="sxs-lookup"><span data-stu-id="0479e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0479e-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0479e-119">Authorization</span></span>|<span data-ttu-id="0479e-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="0479e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0479e-121">Подтверждение</span><span class="sxs-lookup"><span data-stu-id="0479e-121">Accept</span></span>|<span data-ttu-id="0479e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0479e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0479e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0479e-123">Request body</span></span>
<span data-ttu-id="0479e-124">В теле запроса добавьте представление объекта deviceCompliancePolicySettingStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0479e-124">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="0479e-125">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="0479e-125">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="0479e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="0479e-126">Property</span></span>|<span data-ttu-id="0479e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0479e-127">Type</span></span>|<span data-ttu-id="0479e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0479e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0479e-129">id</span><span class="sxs-lookup"><span data-stu-id="0479e-129">id</span></span>|<span data-ttu-id="0479e-130">String</span><span class="sxs-lookup"><span data-stu-id="0479e-130">String</span></span>|<span data-ttu-id="0479e-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0479e-131">Key of the entity.</span></span>|
|<span data-ttu-id="0479e-132">setting</span><span class="sxs-lookup"><span data-stu-id="0479e-132">setting</span></span>|<span data-ttu-id="0479e-133">String</span><span class="sxs-lookup"><span data-stu-id="0479e-133">String</span></span>|<span data-ttu-id="0479e-134">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="0479e-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="0479e-135">settingName</span><span class="sxs-lookup"><span data-stu-id="0479e-135">settingName</span></span>|<span data-ttu-id="0479e-136">String</span><span class="sxs-lookup"><span data-stu-id="0479e-136">String</span></span>|<span data-ttu-id="0479e-137">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="0479e-137">Name of the setting.</span></span>|
|<span data-ttu-id="0479e-138">platformType</span><span class="sxs-lookup"><span data-stu-id="0479e-138">platformType</span></span>|[<span data-ttu-id="0479e-139">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="0479e-139">policyPlatformType</span></span>](../resources/intune_deviceconfig_policyplatformtype.md)|<span data-ttu-id="0479e-140">Платформа настройки.</span><span class="sxs-lookup"><span data-stu-id="0479e-140">Setting platform.</span></span> <span data-ttu-id="0479e-141">Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="0479e-141">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="0479e-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0479e-142">unknownDeviceCount</span></span>|<span data-ttu-id="0479e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="0479e-143">Int32</span></span>|<span data-ttu-id="0479e-144">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="0479e-144">Number of unknown devices</span></span>|
|<span data-ttu-id="0479e-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0479e-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="0479e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0479e-146">Int32</span></span>|<span data-ttu-id="0479e-147">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="0479e-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="0479e-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0479e-148">compliantDeviceCount</span></span>|<span data-ttu-id="0479e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="0479e-149">Int32</span></span>|<span data-ttu-id="0479e-150">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="0479e-150">Number of compliant devices</span></span>|
|<span data-ttu-id="0479e-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0479e-151">remediatedDeviceCount</span></span>|<span data-ttu-id="0479e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0479e-152">Int32</span></span>|<span data-ttu-id="0479e-153">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="0479e-153">Number of remediated devices</span></span>|
|<span data-ttu-id="0479e-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0479e-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="0479e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="0479e-155">Int32</span></span>|<span data-ttu-id="0479e-156">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="0479e-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="0479e-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0479e-157">errorDeviceCount</span></span>|<span data-ttu-id="0479e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0479e-158">Int32</span></span>|<span data-ttu-id="0479e-159">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="0479e-159">Number of error devices</span></span>|
|<span data-ttu-id="0479e-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0479e-160">conflictDeviceCount</span></span>|<span data-ttu-id="0479e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="0479e-161">Int32</span></span>|<span data-ttu-id="0479e-162">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="0479e-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="0479e-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="0479e-163">Response</span></span>
<span data-ttu-id="0479e-164">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0479e-164">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0479e-165">Пример</span><span class="sxs-lookup"><span data-stu-id="0479e-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="0479e-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="0479e-166">Request</span></span>
<span data-ttu-id="0479e-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0479e-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0479e-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="0479e-168">Response</span></span>
<span data-ttu-id="0479e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0479e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
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








