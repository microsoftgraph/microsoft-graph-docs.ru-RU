# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="7cdcc-101">Создание managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="7cdcc-101">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="7cdcc-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cdcc-103">Создание нового объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="7cdcc-103">Create a new [enrollmentConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cdcc-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7cdcc-104">Prerequisites</span></span>
<span data-ttu-id="7cdcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7cdcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7cdcc-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cdcc-107">Permission type</span></span>|<span data-ttu-id="7cdcc-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cdcc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cdcc-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cdcc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7cdcc-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cdcc-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7cdcc-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cdcc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cdcc-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-112">Not supported.</span></span>|
|<span data-ttu-id="7cdcc-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cdcc-113">Application</span></span>|<span data-ttu-id="7cdcc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cdcc-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cdcc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="7cdcc-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cdcc-116">Request headers</span></span>
|<span data-ttu-id="7cdcc-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7cdcc-117">Header</span></span>|<span data-ttu-id="7cdcc-118">Значение</span><span class="sxs-lookup"><span data-stu-id="7cdcc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cdcc-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7cdcc-119">Authorization</span></span>|<span data-ttu-id="7cdcc-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="7cdcc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cdcc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7cdcc-121">Accept</span></span>|<span data-ttu-id="7cdcc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7cdcc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cdcc-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cdcc-123">Request body</span></span>
<span data-ttu-id="7cdcc-124">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-124">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="7cdcc-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-125">The following table shows the properties that are required when you create the deviceAppManagement.</span></span>

|<span data-ttu-id="7cdcc-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cdcc-126">Property</span></span>|<span data-ttu-id="7cdcc-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7cdcc-127">Type</span></span>|<span data-ttu-id="7cdcc-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7cdcc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cdcc-129">id</span><span class="sxs-lookup"><span data-stu-id="7cdcc-129">id</span></span>|<span data-ttu-id="7cdcc-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7cdcc-130">String</span></span>|<span data-ttu-id="7cdcc-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-131">Key of the entity.</span></span>|
|<span data-ttu-id="7cdcc-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7cdcc-132">deviceDisplayName</span></span>|<span data-ttu-id="7cdcc-133">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7cdcc-133">String</span></span>|<span data-ttu-id="7cdcc-134">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="7cdcc-135">userName</span><span class="sxs-lookup"><span data-stu-id="7cdcc-135">userName</span></span>|<span data-ttu-id="7cdcc-136">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7cdcc-136">String</span></span>|<span data-ttu-id="7cdcc-137">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="7cdcc-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="7cdcc-138">deviceModel</span></span>|<span data-ttu-id="7cdcc-139">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7cdcc-139">String</span></span>|<span data-ttu-id="7cdcc-140">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-140">The device model that is being reported</span></span>|
|<span data-ttu-id="7cdcc-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7cdcc-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="7cdcc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cdcc-142">DateTimeOffset</span></span>|<span data-ttu-id="7cdcc-143">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="7cdcc-144">status</span><span class="sxs-lookup"><span data-stu-id="7cdcc-144">status</span></span>|[<span data-ttu-id="7cdcc-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="7cdcc-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="7cdcc-146">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-146">Compliance status of the policy report.</span></span> <span data-ttu-id="7cdcc-147">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-147">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="7cdcc-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="7cdcc-148">lastReportedDateTime</span></span>|<span data-ttu-id="7cdcc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cdcc-149">DateTimeOffset</span></span>|<span data-ttu-id="7cdcc-150">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="7cdcc-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7cdcc-151">userPrincipalName</span></span>|<span data-ttu-id="7cdcc-152">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7cdcc-152">String</span></span>|<span data-ttu-id="7cdcc-153">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="7cdcc-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cdcc-154">Response</span></span>
<span data-ttu-id="7cdcc-155">В случае успеха этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-155">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cdcc-156">Пример</span><span class="sxs-lookup"><span data-stu-id="7cdcc-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cdcc-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cdcc-157">Request</span></span>
<span data-ttu-id="7cdcc-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="7cdcc-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cdcc-159">Response</span></span>
<span data-ttu-id="7cdcc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7cdcc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



