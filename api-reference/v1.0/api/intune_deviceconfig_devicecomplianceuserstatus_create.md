# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="57fc8-101">Создание объекта deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="57fc8-101">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="57fc8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="57fc8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57fc8-103">Создание объекта [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="57fc8-103">Create a new [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57fc8-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="57fc8-104">Prerequisites</span></span>
<span data-ttu-id="57fc8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="57fc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="57fc8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57fc8-107">Permission type</span></span>|<span data-ttu-id="57fc8-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57fc8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57fc8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57fc8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="57fc8-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57fc8-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57fc8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57fc8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57fc8-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57fc8-112">Not supported.</span></span>|
|<span data-ttu-id="57fc8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57fc8-113">Application</span></span>|<span data-ttu-id="57fc8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57fc8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57fc8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57fc8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="57fc8-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57fc8-116">Request headers</span></span>
|<span data-ttu-id="57fc8-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57fc8-117">Header</span></span>|<span data-ttu-id="57fc8-118">Значение</span><span class="sxs-lookup"><span data-stu-id="57fc8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57fc8-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57fc8-119">Authorization</span></span>|<span data-ttu-id="57fc8-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="57fc8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57fc8-121">Принять</span><span class="sxs-lookup"><span data-stu-id="57fc8-121">Accept</span></span>|<span data-ttu-id="57fc8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="57fc8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57fc8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57fc8-123">Request body</span></span>
<span data-ttu-id="57fc8-124">В тексте запроса добавьте представление объекта deviceComplianceUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57fc8-124">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="57fc8-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="57fc8-125">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="57fc8-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="57fc8-126">Property</span></span>|<span data-ttu-id="57fc8-127">Тип</span><span class="sxs-lookup"><span data-stu-id="57fc8-127">Type</span></span>|<span data-ttu-id="57fc8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="57fc8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57fc8-129">id</span><span class="sxs-lookup"><span data-stu-id="57fc8-129">id</span></span>|<span data-ttu-id="57fc8-130">Строка</span><span class="sxs-lookup"><span data-stu-id="57fc8-130">String</span></span>|<span data-ttu-id="57fc8-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="57fc8-131">Key of the entity.</span></span>|
|<span data-ttu-id="57fc8-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="57fc8-132">userDisplayName</span></span>|<span data-ttu-id="57fc8-133">Строка</span><span class="sxs-lookup"><span data-stu-id="57fc8-133">String</span></span>|<span data-ttu-id="57fc8-134">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="57fc8-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="57fc8-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="57fc8-135">devicesCount</span></span>|<span data-ttu-id="57fc8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="57fc8-136">Int32</span></span>|<span data-ttu-id="57fc8-137">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="57fc8-137">Devices count for that user.</span></span>|
|<span data-ttu-id="57fc8-138">status</span><span class="sxs-lookup"><span data-stu-id="57fc8-138">status</span></span>|[<span data-ttu-id="57fc8-139">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="57fc8-139">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="57fc8-140">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="57fc8-140">Compliance status of the policy report.</span></span> <span data-ttu-id="57fc8-141">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="57fc8-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="57fc8-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="57fc8-142">lastReportedDateTime</span></span>|<span data-ttu-id="57fc8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57fc8-143">DateTimeOffset</span></span>|<span data-ttu-id="57fc8-144">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="57fc8-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="57fc8-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="57fc8-145">userPrincipalName</span></span>|<span data-ttu-id="57fc8-146">Строка</span><span class="sxs-lookup"><span data-stu-id="57fc8-146">String</span></span>|<span data-ttu-id="57fc8-147">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="57fc8-147">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="57fc8-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="57fc8-148">Response</span></span>
<span data-ttu-id="57fc8-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57fc8-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57fc8-150">Пример</span><span class="sxs-lookup"><span data-stu-id="57fc8-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="57fc8-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="57fc8-151">Request</span></span>
<span data-ttu-id="57fc8-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57fc8-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="57fc8-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="57fc8-153">Response</span></span>
<span data-ttu-id="57fc8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57fc8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```








