# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="5ec2f-101">Обновление объекта deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="5ec2f-101">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="5ec2f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ec2f-103">Обновление свойств объекта [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5ec2f-103">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ec2f-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5ec2f-104">Prerequisites</span></span>
<span data-ttu-id="5ec2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5ec2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ec2f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ec2f-107">Permission type</span></span>|<span data-ttu-id="5ec2f-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ec2f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ec2f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ec2f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5ec2f-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ec2f-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ec2f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ec2f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ec2f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-112">Not supported.</span></span>|
|<span data-ttu-id="5ec2f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ec2f-113">Application</span></span>|<span data-ttu-id="5ec2f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ec2f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ec2f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="5ec2f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ec2f-116">Request headers</span></span>
|<span data-ttu-id="5ec2f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ec2f-117">Header</span></span>|<span data-ttu-id="5ec2f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="5ec2f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ec2f-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ec2f-119">Authorization</span></span>|<span data-ttu-id="5ec2f-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="5ec2f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ec2f-121">Принять</span><span class="sxs-lookup"><span data-stu-id="5ec2f-121">Accept</span></span>|<span data-ttu-id="5ec2f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5ec2f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ec2f-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ec2f-123">Request body</span></span>
<span data-ttu-id="5ec2f-124">В теле запроса добавьте представление объекта [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-124">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="5ec2f-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5ec2f-125">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="5ec2f-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ec2f-126">Property</span></span>|<span data-ttu-id="5ec2f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="5ec2f-127">Type</span></span>|<span data-ttu-id="5ec2f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5ec2f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ec2f-129">id</span><span class="sxs-lookup"><span data-stu-id="5ec2f-129">id</span></span>|<span data-ttu-id="5ec2f-130">Строка</span><span class="sxs-lookup"><span data-stu-id="5ec2f-130">String</span></span>|<span data-ttu-id="5ec2f-131">Ключ сущности.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-131">Key of the entity.</span></span>|
|<span data-ttu-id="5ec2f-132">setting</span><span class="sxs-lookup"><span data-stu-id="5ec2f-132">setting</span></span>|<span data-ttu-id="5ec2f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5ec2f-133">String</span></span>|<span data-ttu-id="5ec2f-134">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="5ec2f-135">settingName</span><span class="sxs-lookup"><span data-stu-id="5ec2f-135">settingName</span></span>|<span data-ttu-id="5ec2f-136">String</span><span class="sxs-lookup"><span data-stu-id="5ec2f-136">String</span></span>|<span data-ttu-id="5ec2f-137">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-137">Name of the setting.</span></span>|
|<span data-ttu-id="5ec2f-138">platformType</span><span class="sxs-lookup"><span data-stu-id="5ec2f-138">platformType</span></span>|[<span data-ttu-id="5ec2f-139">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="5ec2f-139">policyPlatformType</span></span>](../resources/intune_deviceconfig_policyplatformtype.md)|<span data-ttu-id="5ec2f-140">Платформа настройки.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-140">Setting platform.</span></span> <span data-ttu-id="5ec2f-141">Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-141">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="5ec2f-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ec2f-142">unknownDeviceCount</span></span>|<span data-ttu-id="5ec2f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5ec2f-143">Int32</span></span>|<span data-ttu-id="5ec2f-144">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-144">Number of unknown devices</span></span>|
|<span data-ttu-id="5ec2f-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ec2f-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="5ec2f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5ec2f-146">Int32</span></span>|<span data-ttu-id="5ec2f-147">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="5ec2f-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ec2f-148">compliantDeviceCount</span></span>|<span data-ttu-id="5ec2f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5ec2f-149">Int32</span></span>|<span data-ttu-id="5ec2f-150">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-150">Number of compliant devices</span></span>|
|<span data-ttu-id="5ec2f-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ec2f-151">remediatedDeviceCount</span></span>|<span data-ttu-id="5ec2f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5ec2f-152">Int32</span></span>|<span data-ttu-id="5ec2f-153">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-153">Number of remediated devices</span></span>|
|<span data-ttu-id="5ec2f-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ec2f-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="5ec2f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5ec2f-155">Int32</span></span>|<span data-ttu-id="5ec2f-156">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="5ec2f-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ec2f-157">errorDeviceCount</span></span>|<span data-ttu-id="5ec2f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5ec2f-158">Int32</span></span>|<span data-ttu-id="5ec2f-159">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-159">Number of error devices</span></span>|
|<span data-ttu-id="5ec2f-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ec2f-160">conflictDeviceCount</span></span>|<span data-ttu-id="5ec2f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5ec2f-161">Int32</span></span>|<span data-ttu-id="5ec2f-162">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="5ec2f-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ec2f-163">Response</span></span>
<span data-ttu-id="5ec2f-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ec2f-165">Пример</span><span class="sxs-lookup"><span data-stu-id="5ec2f-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ec2f-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ec2f-166">Request</span></span>
<span data-ttu-id="5ec2f-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 311

{
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

### <a name="response"></a><span data-ttu-id="5ec2f-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ec2f-168">Response</span></span>
<span data-ttu-id="5ec2f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ec2f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








