# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="9d988-101">Создание объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="9d988-101">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="9d988-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9d988-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d988-103">Создание объекта [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9d988-103">Create a new [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d988-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9d988-104">Prerequisites</span></span>
<span data-ttu-id="9d988-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d988-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d988-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d988-107">Permission type</span></span>|<span data-ttu-id="9d988-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d988-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d988-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d988-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9d988-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d988-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d988-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d988-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d988-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d988-112">Not supported.</span></span>|
|<span data-ttu-id="9d988-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d988-113">Application</span></span>|<span data-ttu-id="9d988-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d988-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d988-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d988-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9d988-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d988-116">Request headers</span></span>
|<span data-ttu-id="9d988-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d988-117">Header</span></span>|<span data-ttu-id="9d988-118">Значение</span><span class="sxs-lookup"><span data-stu-id="9d988-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d988-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d988-119">Authorization</span></span>|<span data-ttu-id="9d988-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="9d988-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d988-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9d988-121">Accept</span></span>|<span data-ttu-id="9d988-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="9d988-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d988-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d988-123">Request body</span></span>
<span data-ttu-id="9d988-124">В тексте запроса добавьте представление объекта deviceComplianceDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d988-124">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="9d988-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="9d988-125">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="9d988-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d988-126">Property</span></span>|<span data-ttu-id="9d988-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9d988-127">Type</span></span>|<span data-ttu-id="9d988-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9d988-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d988-129">id</span><span class="sxs-lookup"><span data-stu-id="9d988-129">id</span></span>|<span data-ttu-id="9d988-130">Строка</span><span class="sxs-lookup"><span data-stu-id="9d988-130">String</span></span>|<span data-ttu-id="9d988-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9d988-131">Key of the entity.</span></span>|
|<span data-ttu-id="9d988-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9d988-132">deviceDisplayName</span></span>|<span data-ttu-id="9d988-133">String (строка)</span><span class="sxs-lookup"><span data-stu-id="9d988-133">String</span></span>|<span data-ttu-id="9d988-134">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="9d988-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="9d988-135">userName</span><span class="sxs-lookup"><span data-stu-id="9d988-135">userName</span></span>|<span data-ttu-id="9d988-136">String (строка)</span><span class="sxs-lookup"><span data-stu-id="9d988-136">String</span></span>|<span data-ttu-id="9d988-137">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="9d988-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="9d988-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9d988-138">deviceModel</span></span>|<span data-ttu-id="9d988-139">String (строка)</span><span class="sxs-lookup"><span data-stu-id="9d988-139">String</span></span>|<span data-ttu-id="9d988-140">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="9d988-140">The device model that is being reported</span></span>|
|<span data-ttu-id="9d988-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9d988-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9d988-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d988-142">DateTimeOffset</span></span>|<span data-ttu-id="9d988-143">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9d988-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="9d988-144">Состояние</span><span class="sxs-lookup"><span data-stu-id="9d988-144">status</span></span>|[<span data-ttu-id="9d988-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9d988-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="9d988-p102">Состояние соответствия требованиям отчета о политике. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="9d988-p102">Compliance status of the policy report. The possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="9d988-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d988-148">lastReportedDateTime</span></span>|<span data-ttu-id="9d988-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d988-149">DateTimeOffset</span></span>|<span data-ttu-id="9d988-150">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="9d988-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="9d988-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9d988-151">userPrincipalName</span></span>|<span data-ttu-id="9d988-152">String (строка)</span><span class="sxs-lookup"><span data-stu-id="9d988-152">String</span></span>|<span data-ttu-id="9d988-153">Имя пользователя-участника.</span><span class="sxs-lookup"><span data-stu-id="9d988-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="9d988-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d988-154">Response</span></span>
<span data-ttu-id="9d988-155">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d988-155">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d988-156">Пример</span><span class="sxs-lookup"><span data-stu-id="9d988-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d988-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d988-157">Request</span></span>
<span data-ttu-id="9d988-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d988-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="9d988-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d988-159">Response</span></span>
<span data-ttu-id="9d988-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d988-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```








