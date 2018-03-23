# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="7acc2-101">Обновление объекта deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="7acc2-101">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="7acc2-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7acc2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7acc2-103">Обновление свойств объекта [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7acc2-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7acc2-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7acc2-104">Prerequisites</span></span>
<span data-ttu-id="7acc2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7acc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7acc2-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7acc2-107">Permission type</span></span>|<span data-ttu-id="7acc2-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7acc2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7acc2-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7acc2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7acc2-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7acc2-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7acc2-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7acc2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7acc2-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7acc2-112">Not supported.</span></span>|
|<span data-ttu-id="7acc2-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7acc2-113">Application</span></span>|<span data-ttu-id="7acc2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7acc2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7acc2-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7acc2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="7acc2-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7acc2-116">Request headers</span></span>
|<span data-ttu-id="7acc2-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7acc2-117">Header</span></span>|<span data-ttu-id="7acc2-118">Значение</span><span class="sxs-lookup"><span data-stu-id="7acc2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7acc2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7acc2-119">Authorization</span></span>|<span data-ttu-id="7acc2-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7acc2-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7acc2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7acc2-121">Accept</span></span>|<span data-ttu-id="7acc2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7acc2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7acc2-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7acc2-123">Request body</span></span>
<span data-ttu-id="7acc2-124">В теле запроса добавьте представление объекта [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7acc2-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="7acc2-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7acc2-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="7acc2-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="7acc2-126">Property</span></span>|<span data-ttu-id="7acc2-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7acc2-127">Type</span></span>|<span data-ttu-id="7acc2-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7acc2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7acc2-129">setting</span><span class="sxs-lookup"><span data-stu-id="7acc2-129">setting</span></span>|<span data-ttu-id="7acc2-130">String</span><span class="sxs-lookup"><span data-stu-id="7acc2-130">String</span></span>|<span data-ttu-id="7acc2-131">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="7acc2-131">The setting class name and property name.</span></span>|
|<span data-ttu-id="7acc2-132">settingName</span><span class="sxs-lookup"><span data-stu-id="7acc2-132">settingName</span></span>|<span data-ttu-id="7acc2-133">String</span><span class="sxs-lookup"><span data-stu-id="7acc2-133">String</span></span>|<span data-ttu-id="7acc2-134">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="7acc2-134">Name of the setting.</span></span>|
|<span data-ttu-id="7acc2-135">platformType</span><span class="sxs-lookup"><span data-stu-id="7acc2-135">PlatformType</span></span>|<span data-ttu-id="7acc2-136">String</span><span class="sxs-lookup"><span data-stu-id="7acc2-136">String</span></span>|<span data-ttu-id="7acc2-137">Выбор платформы. Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span><span class="sxs-lookup"><span data-stu-id="7acc2-137">Setting platform Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="7acc2-138">id</span><span class="sxs-lookup"><span data-stu-id="7acc2-138">id</span></span>|<span data-ttu-id="7acc2-139">String</span><span class="sxs-lookup"><span data-stu-id="7acc2-139">String</span></span>|<span data-ttu-id="7acc2-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7acc2-140">Key of the setting.</span></span>|
|<span data-ttu-id="7acc2-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7acc2-141">unknownDeviceCount</span></span>|<span data-ttu-id="7acc2-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc2-142">Int32</span></span>|<span data-ttu-id="7acc2-143">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="7acc2-143">Number of unknown devices</span></span>|
|<span data-ttu-id="7acc2-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7acc2-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="7acc2-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc2-145">Int32</span></span>|<span data-ttu-id="7acc2-146">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="7acc2-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="7acc2-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7acc2-147">compliantDeviceCount</span></span>|<span data-ttu-id="7acc2-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc2-148">Int32</span></span>|<span data-ttu-id="7acc2-149">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="7acc2-149">Number of compliant devices</span></span>|
|<span data-ttu-id="7acc2-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7acc2-150">remediatedDeviceCount</span></span>|<span data-ttu-id="7acc2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc2-151">Int32</span></span>|<span data-ttu-id="7acc2-152">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="7acc2-152">Number of remediated devices</span></span>|
|<span data-ttu-id="7acc2-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7acc2-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7acc2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc2-154">Int32</span></span>|<span data-ttu-id="7acc2-155">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="7acc2-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="7acc2-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7acc2-156">errorDeviceCount</span></span>|<span data-ttu-id="7acc2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc2-157">Int32</span></span>|<span data-ttu-id="7acc2-158">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="7acc2-158">Number of error devices</span></span>|
|<span data-ttu-id="7acc2-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7acc2-159">conflictDeviceCount</span></span>|<span data-ttu-id="7acc2-160">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc2-160">Int32</span></span>|<span data-ttu-id="7acc2-161">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="7acc2-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="7acc2-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="7acc2-162">Response</span></span>
<span data-ttu-id="7acc2-163">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7acc2-163">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7acc2-164">Пример</span><span class="sxs-lookup"><span data-stu-id="7acc2-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="7acc2-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="7acc2-165">Request</span></span>
<span data-ttu-id="7acc2-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7acc2-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7acc2-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="7acc2-167">Response</span></span>
<span data-ttu-id="7acc2-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7acc2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



