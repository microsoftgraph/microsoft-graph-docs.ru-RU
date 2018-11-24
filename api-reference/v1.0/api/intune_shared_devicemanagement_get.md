# <a name="get-devicemanagement"></a><span data-ttu-id="29a17-101">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="29a17-101">Get deviceManagement</span></span>

> <span data-ttu-id="29a17-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="29a17-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29a17-103">Чтение свойств и связей объекта [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="29a17-103">Read properties and relationships of the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29a17-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="29a17-104">Prerequisites</span></span>
<span data-ttu-id="29a17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="29a17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="29a17-107">Разрешение&nbsp;тип&nbsp;(с&nbsp;рабочего процесса)</span><span class="sxs-lookup"><span data-stu-id="29a17-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="29a17-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="29a17-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="29a17-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29a17-109">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="29a17-110">&nbsp;&nbsp; Аудита</span><span class="sxs-lookup"><span data-stu-id="29a17-110">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="29a17-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="29a17-112">&nbsp;&nbsp; Компании термины</span><span class="sxs-lookup"><span data-stu-id="29a17-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="29a17-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="29a17-114">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="29a17-114">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="29a17-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="29a17-116">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="29a17-116">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="29a17-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="29a17-118">&nbsp;&nbsp; Подачи заявок</span><span class="sxs-lookup"><span data-stu-id="29a17-118">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="29a17-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="29a17-120">&nbsp;&nbsp; Уведомлений</span><span class="sxs-lookup"><span data-stu-id="29a17-120">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="29a17-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="29a17-122">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="29a17-122">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="29a17-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="29a17-124">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="29a17-124">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="29a17-125">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-125">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="29a17-126">&nbsp;&nbsp; Удаленный помощник</span><span class="sxs-lookup"><span data-stu-id="29a17-126">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="29a17-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="29a17-128">&nbsp;&nbsp; Управления расходами телекоммуникации</span><span class="sxs-lookup"><span data-stu-id="29a17-128">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="29a17-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="29a17-130">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="29a17-130">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="29a17-131">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-131">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="29a17-132">&nbsp;&nbsp; Защита информации Windows</span><span class="sxs-lookup"><span data-stu-id="29a17-132">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="29a17-133">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a17-133">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="29a17-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29a17-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29a17-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29a17-135">Not supported.</span></span>|
| <span data-ttu-id="29a17-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29a17-136">Application</span></span> | <span data-ttu-id="29a17-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29a17-137">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="29a17-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29a17-138">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29a17-139">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="29a17-139">Optional query parameters</span></span>
<span data-ttu-id="29a17-140">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="29a17-140">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="29a17-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29a17-141">Request headers</span></span>
|<span data-ttu-id="29a17-142">Заголовок</span><span class="sxs-lookup"><span data-stu-id="29a17-142">Header</span></span>|<span data-ttu-id="29a17-143">Значение</span><span class="sxs-lookup"><span data-stu-id="29a17-143">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29a17-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="29a17-144">Authorization</span></span>|<span data-ttu-id="29a17-145">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="29a17-145">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29a17-146">Accept</span><span class="sxs-lookup"><span data-stu-id="29a17-146">Accept</span></span>|<span data-ttu-id="29a17-147">application/json</span><span class="sxs-lookup"><span data-stu-id="29a17-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29a17-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29a17-148">Request body</span></span>
<span data-ttu-id="29a17-149">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29a17-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29a17-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="29a17-150">Response</span></span>
<span data-ttu-id="29a17-151">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune_shared_devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="29a17-151">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29a17-152">Пример</span><span class="sxs-lookup"><span data-stu-id="29a17-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="29a17-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="29a17-153">Request</span></span>
<span data-ttu-id="29a17-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29a17-154">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="29a17-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="29a17-155">Response</span></span>
<span data-ttu-id="29a17-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="29a17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```



