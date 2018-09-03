# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="51a9e-101">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="51a9e-101">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="51a9e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51a9e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51a9e-103">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="51a9e-103">Update the properties of a [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51a9e-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="51a9e-104">Prerequisites</span></span>
<span data-ttu-id="51a9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="51a9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="51a9e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51a9e-107">Permission type</span></span>|<span data-ttu-id="51a9e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51a9e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51a9e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51a9e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="51a9e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51a9e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51a9e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51a9e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51a9e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51a9e-112">Not supported.</span></span>|
|<span data-ttu-id="51a9e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51a9e-113">Application</span></span>|<span data-ttu-id="51a9e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51a9e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51a9e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51a9e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="51a9e-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51a9e-116">Request headers</span></span>
|<span data-ttu-id="51a9e-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51a9e-117">Header</span></span>|<span data-ttu-id="51a9e-118">Значение</span><span class="sxs-lookup"><span data-stu-id="51a9e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51a9e-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51a9e-119">Authorization</span></span>|<span data-ttu-id="51a9e-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="51a9e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51a9e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="51a9e-121">Accept</span></span>|<span data-ttu-id="51a9e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="51a9e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51a9e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51a9e-123">Request body</span></span>
<span data-ttu-id="51a9e-124">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51a9e-124">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="51a9e-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="51a9e-125">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="51a9e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="51a9e-126">Property</span></span>|<span data-ttu-id="51a9e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="51a9e-127">Type</span></span>|<span data-ttu-id="51a9e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="51a9e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51a9e-129">id</span><span class="sxs-lookup"><span data-stu-id="51a9e-129">id</span></span>|<span data-ttu-id="51a9e-130">Строка</span><span class="sxs-lookup"><span data-stu-id="51a9e-130">String</span></span>|<span data-ttu-id="51a9e-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="51a9e-131">Key of the entity.</span></span>|
|<span data-ttu-id="51a9e-132">installStatus</span><span class="sxs-lookup"><span data-stu-id="51a9e-132">installStatus</span></span>|[<span data-ttu-id="51a9e-133">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="51a9e-133">iosUpdatesInstallStatus</span></span>](../resources/intune_deviceconfig_iosupdatesinstallstatus.md)|<span data-ttu-id="51a9e-134">Состояние установки в отчете о политике.</span><span class="sxs-lookup"><span data-stu-id="51a9e-134">The installation status of the policy report.</span></span> <span data-ttu-id="51a9e-135">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="51a9e-135">The possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="51a9e-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="51a9e-136">osVersion</span></span>|<span data-ttu-id="51a9e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="51a9e-137">String</span></span>|<span data-ttu-id="51a9e-138">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="51a9e-138">The device version that is being reported.</span></span>|
|<span data-ttu-id="51a9e-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="51a9e-139">deviceId</span></span>|<span data-ttu-id="51a9e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="51a9e-140">String</span></span>|<span data-ttu-id="51a9e-141">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="51a9e-141">The device id that is being reported.</span></span>|
|<span data-ttu-id="51a9e-142">userId</span><span class="sxs-lookup"><span data-stu-id="51a9e-142">userId</span></span>|<span data-ttu-id="51a9e-143">Строка</span><span class="sxs-lookup"><span data-stu-id="51a9e-143">String</span></span>|<span data-ttu-id="51a9e-144">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="51a9e-144">The User id that is being reported.</span></span>|
|<span data-ttu-id="51a9e-145">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="51a9e-145">deviceDisplayName</span></span>|<span data-ttu-id="51a9e-146">Строка</span><span class="sxs-lookup"><span data-stu-id="51a9e-146">String</span></span>|<span data-ttu-id="51a9e-147">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="51a9e-147">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="51a9e-148">userName</span><span class="sxs-lookup"><span data-stu-id="51a9e-148">userName</span></span>|<span data-ttu-id="51a9e-149">Строка</span><span class="sxs-lookup"><span data-stu-id="51a9e-149">String</span></span>|<span data-ttu-id="51a9e-150">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="51a9e-150">The User Name that is being reported</span></span>|
|<span data-ttu-id="51a9e-151">deviceModel</span><span class="sxs-lookup"><span data-stu-id="51a9e-151">deviceModel</span></span>|<span data-ttu-id="51a9e-152">Строка</span><span class="sxs-lookup"><span data-stu-id="51a9e-152">String</span></span>|<span data-ttu-id="51a9e-153">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="51a9e-153">The device model that is being reported</span></span>|
|<span data-ttu-id="51a9e-154">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="51a9e-154">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="51a9e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51a9e-155">DateTimeOffset</span></span>|<span data-ttu-id="51a9e-156">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="51a9e-156">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="51a9e-157">status</span><span class="sxs-lookup"><span data-stu-id="51a9e-157">status</span></span>|[<span data-ttu-id="51a9e-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="51a9e-158">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="51a9e-159">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="51a9e-159">Compliance status of the policy report.</span></span> <span data-ttu-id="51a9e-160">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="51a9e-160">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="51a9e-161">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="51a9e-161">lastReportedDateTime</span></span>|<span data-ttu-id="51a9e-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51a9e-162">DateTimeOffset</span></span>|<span data-ttu-id="51a9e-163">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="51a9e-163">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="51a9e-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51a9e-164">userPrincipalName</span></span>|<span data-ttu-id="51a9e-165">Строка</span><span class="sxs-lookup"><span data-stu-id="51a9e-165">String</span></span>|<span data-ttu-id="51a9e-166">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="51a9e-166">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="51a9e-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="51a9e-167">Response</span></span>
<span data-ttu-id="51a9e-168">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="51a9e-168">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51a9e-169">Пример</span><span class="sxs-lookup"><span data-stu-id="51a9e-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="51a9e-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="51a9e-170">Request</span></span>
<span data-ttu-id="51a9e-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51a9e-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
Content-type: application/json
Content-length: 492

{
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="51a9e-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="51a9e-172">Response</span></span>
<span data-ttu-id="51a9e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51a9e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "63a79499-9499-63a7-9994-a7639994a763",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



