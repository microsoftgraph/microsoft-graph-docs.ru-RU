# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="17c30-101">Обновление объекта deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="17c30-101">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="17c30-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="17c30-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17c30-103">Обновление свойств объекта [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="17c30-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="17c30-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="17c30-104">Prerequisites</span></span>
<span data-ttu-id="17c30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="17c30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="17c30-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17c30-107">Permission type</span></span>|<span data-ttu-id="17c30-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17c30-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17c30-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17c30-109">Delegated (work or school account)</span></span>|<span data-ttu-id="17c30-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17c30-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17c30-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17c30-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17c30-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17c30-112">Not supported.</span></span>|
|<span data-ttu-id="17c30-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17c30-113">Application</span></span>|<span data-ttu-id="17c30-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17c30-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17c30-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17c30-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="17c30-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17c30-116">Request headers</span></span>
|<span data-ttu-id="17c30-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17c30-117">Header</span></span>|<span data-ttu-id="17c30-118">Значение</span><span class="sxs-lookup"><span data-stu-id="17c30-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17c30-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="17c30-119">Authorization</span></span>|<span data-ttu-id="17c30-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17c30-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="17c30-121">Accept</span><span class="sxs-lookup"><span data-stu-id="17c30-121">Accept</span></span>|<span data-ttu-id="17c30-122">application/json</span><span class="sxs-lookup"><span data-stu-id="17c30-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17c30-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17c30-123">Request body</span></span>
<span data-ttu-id="17c30-124">В тексте запроса добавьте представление объекта [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17c30-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="17c30-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="17c30-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="17c30-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="17c30-126">Property</span></span>|<span data-ttu-id="17c30-127">Тип</span><span class="sxs-lookup"><span data-stu-id="17c30-127">Type</span></span>|<span data-ttu-id="17c30-128">Описание</span><span class="sxs-lookup"><span data-stu-id="17c30-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17c30-129">id</span><span class="sxs-lookup"><span data-stu-id="17c30-129">id</span></span>|<span data-ttu-id="17c30-130">String</span><span class="sxs-lookup"><span data-stu-id="17c30-130">String</span></span>|<span data-ttu-id="17c30-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="17c30-131">Key of the setting.</span></span>|
|<span data-ttu-id="17c30-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="17c30-132">userDisplayName</span></span>|<span data-ttu-id="17c30-133">String</span><span class="sxs-lookup"><span data-stu-id="17c30-133">String</span></span>|<span data-ttu-id="17c30-134">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="17c30-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="17c30-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="17c30-135">devicesCount</span></span>|<span data-ttu-id="17c30-136">Int32</span><span class="sxs-lookup"><span data-stu-id="17c30-136">Int32</span></span>|<span data-ttu-id="17c30-137">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="17c30-137">Devices count for that user.</span></span>|
|<span data-ttu-id="17c30-138">status</span><span class="sxs-lookup"><span data-stu-id="17c30-138">status</span></span>|<span data-ttu-id="17c30-139">String</span><span class="sxs-lookup"><span data-stu-id="17c30-139">String</span></span>|<span data-ttu-id="17c30-140">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="17c30-140">Compliance status of the policy report.</span></span> <span data-ttu-id="17c30-141">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="17c30-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="17c30-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="17c30-142">lastReportedDateTime</span></span>|<span data-ttu-id="17c30-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17c30-143">DateTimeOffset</span></span>|<span data-ttu-id="17c30-144">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="17c30-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="17c30-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="17c30-145">userPrincipalName</span></span>|<span data-ttu-id="17c30-146">String</span><span class="sxs-lookup"><span data-stu-id="17c30-146">String</span></span>|<span data-ttu-id="17c30-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="17c30-147">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="17c30-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="17c30-148">Response</span></span>
<span data-ttu-id="17c30-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17c30-149">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17c30-150">Пример</span><span class="sxs-lookup"><span data-stu-id="17c30-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="17c30-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="17c30-151">Request</span></span>
<span data-ttu-id="17c30-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17c30-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
Content-type: application/json
Content-length: 222

{
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="17c30-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="17c30-153">Response</span></span>
<span data-ttu-id="17c30-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="17c30-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



