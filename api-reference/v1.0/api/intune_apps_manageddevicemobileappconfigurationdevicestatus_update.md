# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="a9d7c-101">Обновить managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a9d7c-101">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="a9d7c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9d7c-103">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a9d7c-103">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9d7c-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a9d7c-104">Prerequisites</span></span>
<span data-ttu-id="a9d7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9d7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a9d7c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9d7c-107">Permission type</span></span>|<span data-ttu-id="a9d7c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9d7c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9d7c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9d7c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a9d7c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9d7c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a9d7c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9d7c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9d7c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-112">Not supported.</span></span>|
|<span data-ttu-id="a9d7c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9d7c-113">Application</span></span>|<span data-ttu-id="a9d7c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9d7c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9d7c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="a9d7c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9d7c-116">Request headers</span></span>
|<span data-ttu-id="a9d7c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9d7c-117">Header</span></span>|<span data-ttu-id="a9d7c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a9d7c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9d7c-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9d7c-119">Authorization</span></span>|<span data-ttu-id="a9d7c-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="a9d7c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9d7c-121">Принять</span><span class="sxs-lookup"><span data-stu-id="a9d7c-121">Accept</span></span>|<span data-ttu-id="a9d7c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a9d7c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9d7c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9d7c-123">Request body</span></span>
<span data-ttu-id="a9d7c-124">В теле запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-124">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="a9d7c-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a9d7c-125">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="a9d7c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9d7c-126">Property</span></span>|<span data-ttu-id="a9d7c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a9d7c-127">Type</span></span>|<span data-ttu-id="a9d7c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a9d7c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9d7c-129">ид</span><span class="sxs-lookup"><span data-stu-id="a9d7c-129">id</span></span>|<span data-ttu-id="a9d7c-130">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d7c-130">String</span></span>|<span data-ttu-id="a9d7c-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-131">Key of the entity.</span></span>|
|<span data-ttu-id="a9d7c-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a9d7c-132">deviceDisplayName</span></span>|<span data-ttu-id="a9d7c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d7c-133">String</span></span>|<span data-ttu-id="a9d7c-134">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a9d7c-135">userName</span><span class="sxs-lookup"><span data-stu-id="a9d7c-135">userName</span></span>|<span data-ttu-id="a9d7c-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d7c-136">String</span></span>|<span data-ttu-id="a9d7c-137">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="a9d7c-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a9d7c-138">deviceModel</span></span>|<span data-ttu-id="a9d7c-139">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d7c-139">String</span></span>|<span data-ttu-id="a9d7c-140">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-140">The device model that is being reported</span></span>|
|<span data-ttu-id="a9d7c-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a9d7c-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a9d7c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9d7c-142">DateTimeOffset</span></span>|<span data-ttu-id="a9d7c-143">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a9d7c-144">статус</span><span class="sxs-lookup"><span data-stu-id="a9d7c-144">status</span></span>|[<span data-ttu-id="a9d7c-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a9d7c-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="a9d7c-p102">Состояние соответствия требованиям отчета о политике. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-p102">Compliance status of the policy report. The possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="a9d7c-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9d7c-148">lastReportedDateTime</span></span>|<span data-ttu-id="a9d7c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9d7c-149">DateTimeOffset</span></span>|<span data-ttu-id="a9d7c-150">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a9d7c-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9d7c-151">userPrincipalName</span></span>|<span data-ttu-id="a9d7c-152">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d7c-152">String</span></span>|<span data-ttu-id="a9d7c-153">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="a9d7c-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9d7c-154">Response</span></span>
<span data-ttu-id="a9d7c-155">В случае успеха этот метод возвращает `200 OK` код отклика и обновленный [объект managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-155">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9d7c-156">Пример</span><span class="sxs-lookup"><span data-stu-id="a9d7c-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9d7c-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9d7c-157">Request</span></span>
<span data-ttu-id="a9d7c-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 359

{
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="a9d7c-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9d7c-159">Response</span></span>
<span data-ttu-id="a9d7c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9d7c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








