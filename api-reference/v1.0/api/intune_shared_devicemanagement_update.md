# <a name="update-devicemanagement"></a><span data-ttu-id="99e54-101">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="99e54-101">Update deviceManagement</span></span>

> <span data-ttu-id="99e54-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="99e54-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99e54-103">Обновление свойств объекта [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="99e54-103">Update the properties of a [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99e54-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="99e54-104">Prerequisites</span></span>
<span data-ttu-id="99e54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="99e54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="99e54-107">Разрешение&nbsp;тип&nbsp;(с&nbsp;рабочего процесса)</span><span class="sxs-lookup"><span data-stu-id="99e54-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="99e54-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99e54-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="99e54-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99e54-109">Delegated (work or school account)</span></span> |
| <span data-ttu-id="99e54-110">&nbsp;&nbsp; Аудита</span><span class="sxs-lookup"><span data-stu-id="99e54-110">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="99e54-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-111">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-112">&nbsp;&nbsp; Компании термины</span><span class="sxs-lookup"><span data-stu-id="99e54-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="99e54-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-113">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-114">&nbsp;&nbsp; Корпоративной подачи заявок</span><span class="sxs-lookup"><span data-stu-id="99e54-114">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="99e54-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="99e54-116">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="99e54-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="99e54-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-117">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-118">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="99e54-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="99e54-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-120">&nbsp;&nbsp; Защиты конечной точки</span><span class="sxs-lookup"><span data-stu-id="99e54-120">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="99e54-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-122">&nbsp;&nbsp; Уведомлений</span><span class="sxs-lookup"><span data-stu-id="99e54-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="99e54-123">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-123">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-124">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="99e54-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="99e54-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-126">&nbsp;&nbsp; Управления доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="99e54-126">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="99e54-127">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-127">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-128">&nbsp;&nbsp; Удаленный помощник</span><span class="sxs-lookup"><span data-stu-id="99e54-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="99e54-129">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-129">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-130">&nbsp;&nbsp; Управления расходами телекоммуникации</span><span class="sxs-lookup"><span data-stu-id="99e54-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="99e54-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-132">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="99e54-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="99e54-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-133">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-134">&nbsp;&nbsp; Защита информации Windows</span><span class="sxs-lookup"><span data-stu-id="99e54-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="99e54-135">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e54-135">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="99e54-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99e54-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99e54-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99e54-137">Not supported.</span></span>|
| <span data-ttu-id="99e54-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99e54-138">Application</span></span> | <span data-ttu-id="99e54-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99e54-139">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99e54-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99e54-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="99e54-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99e54-141">Request headers</span></span>
|<span data-ttu-id="99e54-142">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99e54-142">Header</span></span>|<span data-ttu-id="99e54-143">Значение</span><span class="sxs-lookup"><span data-stu-id="99e54-143">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99e54-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="99e54-144">Authorization</span></span>|<span data-ttu-id="99e54-145">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="99e54-145">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99e54-146">Accept</span><span class="sxs-lookup"><span data-stu-id="99e54-146">Accept</span></span>|<span data-ttu-id="99e54-147">application/json</span><span class="sxs-lookup"><span data-stu-id="99e54-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99e54-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99e54-148">Request body</span></span>
<span data-ttu-id="99e54-149">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune_shared_devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99e54-149">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>

<span data-ttu-id="99e54-150">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="99e54-150">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune_shared_devicemanagement.md).</span></span>

|<span data-ttu-id="99e54-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="99e54-151">Property</span></span>|<span data-ttu-id="99e54-152">Тип</span><span class="sxs-lookup"><span data-stu-id="99e54-152">Type</span></span>|<span data-ttu-id="99e54-153">Описание</span><span class="sxs-lookup"><span data-stu-id="99e54-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99e54-154">id</span><span class="sxs-lookup"><span data-stu-id="99e54-154">id</span></span>|<span data-ttu-id="99e54-155">String</span><span class="sxs-lookup"><span data-stu-id="99e54-155">String</span></span>|<span data-ttu-id="99e54-156">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="99e54-156">Unique Identifier for the device</span></span>|
|<span data-ttu-id="99e54-157">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="99e54-157">**Device configuration**</span></span>|
|<span data-ttu-id="99e54-158">settings</span><span class="sxs-lookup"><span data-stu-id="99e54-158">settings</span></span>|[<span data-ttu-id="99e54-159">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="99e54-159">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="99e54-160">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="99e54-160">Account level settings.</span></span>|
|<span data-ttu-id="99e54-161">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="99e54-161">**Device management**</span></span>|
|<span data-ttu-id="99e54-162">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="99e54-162">subscriptionState</span></span>|[<span data-ttu-id="99e54-163">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="99e54-163">deviceManagementSubscriptionState</span></span>](../resources/intune_devices_devicemanagementsubscriptionstate.md)|<span data-ttu-id="99e54-164">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="99e54-164">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="99e54-165">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="99e54-165">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="99e54-166">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="99e54-166">**Onboarding**</span></span>|
|<span data-ttu-id="99e54-167">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="99e54-167">intuneBrand</span></span>|[<span data-ttu-id="99e54-168">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="99e54-168">intuneBrand</span></span>](../resources/intune_onboarding_intunebrand.md)|<span data-ttu-id="99e54-169">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="99e54-169">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="99e54-170">Поддержка свойств текст запроса изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="99e54-170">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="99e54-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="99e54-171">Response</span></span>
<span data-ttu-id="99e54-172">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune_shared_devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="99e54-172">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99e54-173">Пример</span><span class="sxs-lookup"><span data-stu-id="99e54-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="99e54-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="99e54-174">Request</span></span>
<span data-ttu-id="99e54-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99e54-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
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
```

### <a name="response"></a><span data-ttu-id="99e54-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="99e54-176">Response</span></span>

<span data-ttu-id="99e54-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="99e54-177">Here is an example of the response.</span></span> <span data-ttu-id="99e54-178">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="99e54-178">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="99e54-179">Возвращаемых свойств различаться в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="99e54-179">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
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
```



