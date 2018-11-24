# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="82651-101">Обновление объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="82651-101">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="82651-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="82651-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82651-103">Обновление свойств объекта [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="82651-103">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82651-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="82651-104">Prerequisites</span></span>
<span data-ttu-id="82651-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="82651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="82651-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82651-107">Permission type</span></span>|<span data-ttu-id="82651-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82651-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82651-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82651-109">Delegated (work or school account)</span></span>|<span data-ttu-id="82651-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82651-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82651-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82651-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82651-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82651-112">Not supported.</span></span>|
|<span data-ttu-id="82651-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82651-113">Application</span></span>|<span data-ttu-id="82651-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82651-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82651-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82651-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="82651-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82651-116">Request headers</span></span>
|<span data-ttu-id="82651-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82651-117">Header</span></span>|<span data-ttu-id="82651-118">Значение</span><span class="sxs-lookup"><span data-stu-id="82651-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82651-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="82651-119">Authorization</span></span>|<span data-ttu-id="82651-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82651-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82651-121">Accept</span><span class="sxs-lookup"><span data-stu-id="82651-121">Accept</span></span>|<span data-ttu-id="82651-122">application/json</span><span class="sxs-lookup"><span data-stu-id="82651-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82651-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82651-123">Request body</span></span>
<span data-ttu-id="82651-124">В теле запроса добавьте представление объекта [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82651-124">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="82651-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="82651-125">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="82651-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="82651-126">Property</span></span>|<span data-ttu-id="82651-127">Тип</span><span class="sxs-lookup"><span data-stu-id="82651-127">Type</span></span>|<span data-ttu-id="82651-128">Описание</span><span class="sxs-lookup"><span data-stu-id="82651-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82651-129">id</span><span class="sxs-lookup"><span data-stu-id="82651-129">id</span></span>|<span data-ttu-id="82651-130">String</span><span class="sxs-lookup"><span data-stu-id="82651-130">String</span></span>|<span data-ttu-id="82651-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="82651-131">Key of the entity.</span></span>|
|<span data-ttu-id="82651-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="82651-132">deviceDisplayName</span></span>|<span data-ttu-id="82651-133">String</span><span class="sxs-lookup"><span data-stu-id="82651-133">String</span></span>|<span data-ttu-id="82651-134">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="82651-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="82651-135">userName</span><span class="sxs-lookup"><span data-stu-id="82651-135">userName</span></span>|<span data-ttu-id="82651-136">String</span><span class="sxs-lookup"><span data-stu-id="82651-136">String</span></span>|<span data-ttu-id="82651-137">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="82651-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="82651-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="82651-138">deviceModel</span></span>|<span data-ttu-id="82651-139">String</span><span class="sxs-lookup"><span data-stu-id="82651-139">String</span></span>|<span data-ttu-id="82651-140">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="82651-140">The device model that is being reported</span></span>|
|<span data-ttu-id="82651-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="82651-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="82651-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82651-142">DateTimeOffset</span></span>|<span data-ttu-id="82651-143">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="82651-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="82651-144">status</span><span class="sxs-lookup"><span data-stu-id="82651-144">status</span></span>|[<span data-ttu-id="82651-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="82651-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="82651-146">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="82651-146">Compliance status of the policy report.</span></span> <span data-ttu-id="82651-147">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="82651-147">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="82651-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="82651-148">lastReportedDateTime</span></span>|<span data-ttu-id="82651-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82651-149">DateTimeOffset</span></span>|<span data-ttu-id="82651-150">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="82651-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="82651-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="82651-151">userPrincipalName</span></span>|<span data-ttu-id="82651-152">String</span><span class="sxs-lookup"><span data-stu-id="82651-152">String</span></span>|<span data-ttu-id="82651-153">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="82651-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="82651-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="82651-154">Response</span></span>
<span data-ttu-id="82651-155">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="82651-155">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82651-156">Пример</span><span class="sxs-lookup"><span data-stu-id="82651-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="82651-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="82651-157">Request</span></span>
<span data-ttu-id="82651-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82651-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 429

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="82651-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="82651-159">Response</span></span>
<span data-ttu-id="82651-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="82651-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



