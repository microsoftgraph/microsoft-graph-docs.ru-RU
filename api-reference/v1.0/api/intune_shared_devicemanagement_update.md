# <a name="update-devicemanagement"></a><span data-ttu-id="67296-101">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="67296-101">Update deviceManagement</span></span>

> <span data-ttu-id="67296-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="67296-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67296-103">Обновление свойств объекта [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="67296-103">Update the properties of a [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67296-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="67296-104">Prerequisites</span></span>
<span data-ttu-id="67296-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="67296-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="67296-107">Тип&nbsp; разрешения (по &nbsp;рабочему процессу)&nbsp;</span><span class="sxs-lookup"><span data-stu-id="67296-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="67296-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="67296-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="67296-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67296-109">Delegated (work or school account)</span></span> |
| <span data-ttu-id="67296-110">&nbsp; &nbsp; Аудит</span><span class="sxs-lookup"><span data-stu-id="67296-110">&nbsp; &nbsp;Auditing</span></span> | <span data-ttu-id="67296-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-111">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-112">&nbsp; &nbsp; Условия организации</span><span class="sxs-lookup"><span data-stu-id="67296-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="67296-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-113">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-114">&nbsp; &nbsp; Корпоративная регистрация</span><span class="sxs-lookup"><span data-stu-id="67296-114">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="67296-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="67296-116">&nbsp; &nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="67296-116">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="67296-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-117">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-118">&nbsp; &nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="67296-118">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="67296-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-120">&nbsp; &nbsp; Защита конечной точки</span><span class="sxs-lookup"><span data-stu-id="67296-120">&nbsp; &nbsp;Endpoint Protection</span></span> | <span data-ttu-id="67296-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-122">&nbsp; &nbsp; Регистрация</span><span class="sxs-lookup"><span data-stu-id="67296-122">&nbsp; &nbsp;Enrollment</span></span> | <span data-ttu-id="67296-123">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-123">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-124">&nbsp; &nbsp; Уведомления</span><span class="sxs-lookup"><span data-stu-id="67296-124">&nbsp; &nbsp;Notification</span></span> | <span data-ttu-id="67296-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-126">&nbsp; &nbsp; Адаптация</span><span class="sxs-lookup"><span data-stu-id="67296-126">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="67296-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-128">&nbsp; &nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="67296-128">&nbsp; &nbsp;RBAC</span></span> | <span data-ttu-id="67296-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-130">&nbsp; &nbsp; Удаленная помощь</span><span class="sxs-lookup"><span data-stu-id="67296-130">remote assistance,</span></span> | <span data-ttu-id="67296-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-132">&nbsp; &nbsp; Управление расходами на телекоммуникации</span><span class="sxs-lookup"><span data-stu-id="67296-132">&nbsp; &nbsp;Telecom expense management partner</span></span> | <span data-ttu-id="67296-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-134">&nbsp; &nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="67296-134">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="67296-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-136">&nbsp; &nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="67296-136">Windows information protection</span></span> | <span data-ttu-id="67296-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67296-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="67296-138">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67296-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67296-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67296-139">Not supported.</span></span>|
| <span data-ttu-id="67296-140">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67296-140">Application</span></span> | <span data-ttu-id="67296-141">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67296-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67296-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67296-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="67296-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67296-143">Request headers</span></span>
|<span data-ttu-id="67296-144">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67296-144">Header</span></span>|<span data-ttu-id="67296-145">Значение</span><span class="sxs-lookup"><span data-stu-id="67296-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67296-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67296-146">Authorization</span></span>|<span data-ttu-id="67296-147">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="67296-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67296-148">Accept</span><span class="sxs-lookup"><span data-stu-id="67296-148">Accept</span></span>|<span data-ttu-id="67296-149">application/json</span><span class="sxs-lookup"><span data-stu-id="67296-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67296-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67296-150">Request body</span></span>
<span data-ttu-id="67296-151">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune_shared_devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67296-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>

<span data-ttu-id="67296-152">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="67296-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune_shared_devicemanagement.md).</span></span>

|<span data-ttu-id="67296-153">Свойство</span><span class="sxs-lookup"><span data-stu-id="67296-153">Property</span></span>|<span data-ttu-id="67296-154">Тип</span><span class="sxs-lookup"><span data-stu-id="67296-154">Type</span></span>|<span data-ttu-id="67296-155">Описание</span><span class="sxs-lookup"><span data-stu-id="67296-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67296-156">id</span><span class="sxs-lookup"><span data-stu-id="67296-156">id</span></span>|<span data-ttu-id="67296-157">String</span><span class="sxs-lookup"><span data-stu-id="67296-157">String</span></span>|<span data-ttu-id="67296-158">Уникальный идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="67296-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="67296-159">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="67296-159">**Device Configuration.**</span></span>|
|<span data-ttu-id="67296-160">settings</span><span class="sxs-lookup"><span data-stu-id="67296-160">settings</span></span>|[<span data-ttu-id="67296-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="67296-161">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="67296-162">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="67296-162">Account level settings.</span></span>|
|<span data-ttu-id="67296-163">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="67296-163">**Device management**</span></span>|
|<span data-ttu-id="67296-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="67296-164">subscriptionState</span></span>|[<span data-ttu-id="67296-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="67296-165">deviceManagementSubscriptionState</span></span>](../resources/intune_devices_devicemanagementsubscriptionstate.md)|<span data-ttu-id="67296-166">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="67296-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="67296-167">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="67296-167">The possible values are `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`, , , , , or .</span></span>|
|<span data-ttu-id="67296-168">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="67296-168">**On-boarding**</span></span>|
|<span data-ttu-id="67296-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="67296-169">intuneBrand</span></span>|[<span data-ttu-id="67296-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="67296-170">intuneBrand</span></span>](../resources/intune_onboarding_intunebrand.md)|<span data-ttu-id="67296-171">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="67296-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="67296-172">Поддержка свойств текст запроса изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="67296-172">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="67296-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="67296-173">Response</span></span>
<span data-ttu-id="67296-174">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune_shared_devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="67296-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67296-175">Пример</span><span class="sxs-lookup"><span data-stu-id="67296-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="67296-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="67296-176">Request</span></span>
<span data-ttu-id="67296-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67296-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67296-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="67296-178">Response</span></span>

<span data-ttu-id="67296-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="67296-179">Here is an example of the response.</span></span> <span data-ttu-id="67296-180">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="67296-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="67296-181">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="67296-181">Returned properties vary according to workflow and context.</span></span>

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



