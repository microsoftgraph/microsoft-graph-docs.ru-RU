# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="061cf-101">Обновление iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="061cf-101">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="061cf-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="061cf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="061cf-103">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="061cf-103">Update the properties of a [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="061cf-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="061cf-104">Prerequisites</span></span>
<span data-ttu-id="061cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="061cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="061cf-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="061cf-107">Permission type</span></span>|<span data-ttu-id="061cf-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="061cf-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="061cf-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="061cf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="061cf-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="061cf-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="061cf-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="061cf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="061cf-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="061cf-112">Not supported.</span></span>|
|<span data-ttu-id="061cf-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="061cf-113">Application</span></span>|<span data-ttu-id="061cf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="061cf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="061cf-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="061cf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="061cf-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="061cf-116">Request headers</span></span>
|<span data-ttu-id="061cf-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="061cf-117">Header</span></span>|<span data-ttu-id="061cf-118">Значение</span><span class="sxs-lookup"><span data-stu-id="061cf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="061cf-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="061cf-119">Authorization</span></span>|<span data-ttu-id="061cf-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="061cf-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="061cf-121">Принять</span><span class="sxs-lookup"><span data-stu-id="061cf-121">Accept</span></span>|<span data-ttu-id="061cf-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="061cf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="061cf-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="061cf-123">Request body</span></span>
<span data-ttu-id="061cf-124">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="061cf-124">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="061cf-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="061cf-125">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="061cf-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="061cf-126">Property</span></span>|<span data-ttu-id="061cf-127">Тип</span><span class="sxs-lookup"><span data-stu-id="061cf-127">Type</span></span>|<span data-ttu-id="061cf-128">Описание</span><span class="sxs-lookup"><span data-stu-id="061cf-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="061cf-129">ИД</span><span class="sxs-lookup"><span data-stu-id="061cf-129">id</span></span>|<span data-ttu-id="061cf-130">Строка</span><span class="sxs-lookup"><span data-stu-id="061cf-130">String</span></span>|<span data-ttu-id="061cf-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="061cf-131">Key of the entity.</span></span>|
|<span data-ttu-id="061cf-132">installStatus</span><span class="sxs-lookup"><span data-stu-id="061cf-132">installStatus</span></span>|[<span data-ttu-id="061cf-133">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="061cf-133">iosUpdatesInstallStatus</span></span>](../resources/intune_deviceconfig_iosupdatesinstallstatus.md)|<span data-ttu-id="061cf-p102">Состояние установки политики отчета. Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="061cf-p102">The installation status of the policy report. The possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="061cf-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="061cf-136">osVersion</span></span>|<span data-ttu-id="061cf-137">Строка</span><span class="sxs-lookup"><span data-stu-id="061cf-137">String</span></span>|<span data-ttu-id="061cf-138">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="061cf-138">The device version that is being reported.</span></span>|
|<span data-ttu-id="061cf-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="061cf-139">deviceId</span></span>|<span data-ttu-id="061cf-140">Строка</span><span class="sxs-lookup"><span data-stu-id="061cf-140">String</span></span>|<span data-ttu-id="061cf-141">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="061cf-141">The device id that is being reported.</span></span>|
|<span data-ttu-id="061cf-142">userId</span><span class="sxs-lookup"><span data-stu-id="061cf-142">userId</span></span>|<span data-ttu-id="061cf-143">Строка</span><span class="sxs-lookup"><span data-stu-id="061cf-143">String</span></span>|<span data-ttu-id="061cf-144">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="061cf-144">The User id that is being reported.</span></span>|
|<span data-ttu-id="061cf-145">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="061cf-145">deviceDisplayName</span></span>|<span data-ttu-id="061cf-146">Строка</span><span class="sxs-lookup"><span data-stu-id="061cf-146">String</span></span>|<span data-ttu-id="061cf-147">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="061cf-147">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="061cf-148">userName</span><span class="sxs-lookup"><span data-stu-id="061cf-148">userName</span></span>|<span data-ttu-id="061cf-149">Строка</span><span class="sxs-lookup"><span data-stu-id="061cf-149">String</span></span>|<span data-ttu-id="061cf-150">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="061cf-150">The User Name that is being reported</span></span>|
|<span data-ttu-id="061cf-151">deviceModel</span><span class="sxs-lookup"><span data-stu-id="061cf-151">deviceModel</span></span>|<span data-ttu-id="061cf-152">Строка</span><span class="sxs-lookup"><span data-stu-id="061cf-152">String</span></span>|<span data-ttu-id="061cf-153">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="061cf-153">The device model that is being reported</span></span>|
|<span data-ttu-id="061cf-154">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="061cf-154">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="061cf-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="061cf-155">DateTimeOffset</span></span>|<span data-ttu-id="061cf-156">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="061cf-156">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="061cf-157">состояние</span><span class="sxs-lookup"><span data-stu-id="061cf-157">status</span></span>|[<span data-ttu-id="061cf-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="061cf-158">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="061cf-p103">Состояние соответствия требованиям отчета о политике. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="061cf-p103">Compliance status of the policy report. The possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="061cf-161">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="061cf-161">lastReportedDateTime</span></span>|<span data-ttu-id="061cf-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="061cf-162">DateTimeOffset</span></span>|<span data-ttu-id="061cf-163">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="061cf-163">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="061cf-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="061cf-164">userPrincipalName</span></span>|<span data-ttu-id="061cf-165">Строка</span><span class="sxs-lookup"><span data-stu-id="061cf-165">String</span></span>|<span data-ttu-id="061cf-166">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="061cf-166">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="061cf-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="061cf-167">Response</span></span>
<span data-ttu-id="061cf-168">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="061cf-168">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="061cf-169">Пример</span><span class="sxs-lookup"><span data-stu-id="061cf-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="061cf-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="061cf-170">Request</span></span>
<span data-ttu-id="061cf-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="061cf-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="061cf-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="061cf-172">Response</span></span>
<span data-ttu-id="061cf-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="061cf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








