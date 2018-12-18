---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: tfitzmac
ms.openlocfilehash: d8a84c61751fdbc8267b846a70adb44d2affbfa2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331670"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="77c8b-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="77c8b-103">Update deviceManagement</span></span>

> <span data-ttu-id="77c8b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="77c8b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77c8b-105">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="77c8b-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77c8b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="77c8b-106">Prerequisites</span></span>
<span data-ttu-id="77c8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77c8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77c8b-109">Разрешение&nbsp;тип&nbsp;(с&nbsp;рабочего процесса)</span><span class="sxs-lookup"><span data-stu-id="77c8b-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="77c8b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77c8b-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="77c8b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77c8b-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="77c8b-112">&nbsp;&nbsp; Аудита</span><span class="sxs-lookup"><span data-stu-id="77c8b-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="77c8b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-114">&nbsp;&nbsp; Компании термины</span><span class="sxs-lookup"><span data-stu-id="77c8b-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="77c8b-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-116">&nbsp;&nbsp; Корпоративной подачи заявок</span><span class="sxs-lookup"><span data-stu-id="77c8b-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="77c8b-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="77c8b-118">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="77c8b-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="77c8b-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-120">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="77c8b-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="77c8b-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-122">&nbsp;&nbsp; Защиты конечной точки</span><span class="sxs-lookup"><span data-stu-id="77c8b-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="77c8b-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-124">&nbsp;&nbsp; Уведомлений</span><span class="sxs-lookup"><span data-stu-id="77c8b-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="77c8b-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-126">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="77c8b-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="77c8b-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-128">&nbsp;&nbsp; Управления доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="77c8b-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="77c8b-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-130">&nbsp;&nbsp; Удаленный помощник</span><span class="sxs-lookup"><span data-stu-id="77c8b-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="77c8b-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-132">&nbsp;&nbsp; Управления расходами телекоммуникации</span><span class="sxs-lookup"><span data-stu-id="77c8b-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="77c8b-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-134">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="77c8b-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="77c8b-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-136">&nbsp;&nbsp; Защита информации Windows</span><span class="sxs-lookup"><span data-stu-id="77c8b-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="77c8b-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c8b-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="77c8b-138">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77c8b-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77c8b-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77c8b-139">Not supported.</span></span>|
| <span data-ttu-id="77c8b-140">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77c8b-140">Application</span></span> | <span data-ttu-id="77c8b-141">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77c8b-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77c8b-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77c8b-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="77c8b-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77c8b-143">Request headers</span></span>
|<span data-ttu-id="77c8b-144">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77c8b-144">Header</span></span>|<span data-ttu-id="77c8b-145">Значение</span><span class="sxs-lookup"><span data-stu-id="77c8b-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77c8b-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77c8b-146">Authorization</span></span>|<span data-ttu-id="77c8b-147">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="77c8b-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77c8b-148">Accept</span><span class="sxs-lookup"><span data-stu-id="77c8b-148">Accept</span></span>|<span data-ttu-id="77c8b-149">application/json</span><span class="sxs-lookup"><span data-stu-id="77c8b-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77c8b-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77c8b-150">Request body</span></span>
<span data-ttu-id="77c8b-151">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77c8b-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="77c8b-152">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="77c8b-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="77c8b-153">Свойство</span><span class="sxs-lookup"><span data-stu-id="77c8b-153">Property</span></span>|<span data-ttu-id="77c8b-154">Тип</span><span class="sxs-lookup"><span data-stu-id="77c8b-154">Type</span></span>|<span data-ttu-id="77c8b-155">Описание</span><span class="sxs-lookup"><span data-stu-id="77c8b-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77c8b-156">id</span><span class="sxs-lookup"><span data-stu-id="77c8b-156">id</span></span>|<span data-ttu-id="77c8b-157">String</span><span class="sxs-lookup"><span data-stu-id="77c8b-157">String</span></span>|<span data-ttu-id="77c8b-158">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="77c8b-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="77c8b-159">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="77c8b-159">**Device configuration**</span></span>|
|<span data-ttu-id="77c8b-160">settings</span><span class="sxs-lookup"><span data-stu-id="77c8b-160">settings</span></span>|[<span data-ttu-id="77c8b-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="77c8b-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="77c8b-162">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="77c8b-162">Account level settings.</span></span>|
|<span data-ttu-id="77c8b-163">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="77c8b-163">**Device management**</span></span>|
|<span data-ttu-id="77c8b-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="77c8b-164">subscriptionState</span></span>|[<span data-ttu-id="77c8b-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="77c8b-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="77c8b-166">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="77c8b-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="77c8b-167">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="77c8b-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="77c8b-168">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="77c8b-168">**Onboarding**</span></span>|
|<span data-ttu-id="77c8b-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="77c8b-169">intuneBrand</span></span>|[<span data-ttu-id="77c8b-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="77c8b-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="77c8b-171">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="77c8b-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="77c8b-172">Поддержка свойств текст запроса изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="77c8b-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="77c8b-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="77c8b-173">Response</span></span>
<span data-ttu-id="77c8b-174">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="77c8b-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77c8b-175">Пример</span><span class="sxs-lookup"><span data-stu-id="77c8b-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="77c8b-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="77c8b-176">Request</span></span>
<span data-ttu-id="77c8b-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77c8b-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77c8b-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="77c8b-178">Response</span></span>

<span data-ttu-id="77c8b-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="77c8b-179">Here is an example of the response.</span></span> <span data-ttu-id="77c8b-180">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="77c8b-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="77c8b-181">Возвращаемых свойств различаться в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="77c8b-181">Returned properties vary according to workflow and context.</span></span>

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



