---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 57fddece1d8059e46121f23596180636c5765913
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463823"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="6abc7-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6abc7-103">Update deviceManagement</span></span>

<span data-ttu-id="6abc7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6abc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6abc7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6abc7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6abc7-106">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="6abc7-106">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6abc7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6abc7-107">Prerequisites</span></span>
<span data-ttu-id="6abc7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6abc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6abc7-110">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="6abc7-110">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="6abc7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6abc7-111">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="6abc7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6abc7-112">Delegated (work or school account)</span></span> |
| <span data-ttu-id="6abc7-113">&nbsp;&nbsp; Аудит</span><span class="sxs-lookup"><span data-stu-id="6abc7-113">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="6abc7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-115">&nbsp;&nbsp; Условия компании</span><span class="sxs-lookup"><span data-stu-id="6abc7-115">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="6abc7-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-117">&nbsp;&nbsp; Корпоративная регистрация</span><span class="sxs-lookup"><span data-stu-id="6abc7-117">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="6abc7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="6abc7-119">&nbsp;&nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="6abc7-119">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="6abc7-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-121">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="6abc7-121">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="6abc7-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-123">&nbsp;&nbsp; Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="6abc7-123">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="6abc7-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-125">&nbsp;&nbsp; Уведомление</span><span class="sxs-lookup"><span data-stu-id="6abc7-125">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="6abc7-126">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-126">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-127">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="6abc7-127">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="6abc7-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-129">&nbsp;&nbsp; Управление доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="6abc7-129">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="6abc7-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-130">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-131">&nbsp;&nbsp; Удаленная помощь</span><span class="sxs-lookup"><span data-stu-id="6abc7-131">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="6abc7-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-133">&nbsp;&nbsp; Управление расходами по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="6abc7-133">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="6abc7-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-135">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="6abc7-135">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="6abc7-136">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-136">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-137">&nbsp;&nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="6abc7-137">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="6abc7-138">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abc7-138">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="6abc7-139">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6abc7-139">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6abc7-140">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6abc7-140">Not supported.</span></span>|
| <span data-ttu-id="6abc7-141">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6abc7-141">Application</span></span> | <span data-ttu-id="6abc7-142">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6abc7-142">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6abc7-143">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6abc7-143">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="6abc7-144">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6abc7-144">Request headers</span></span>
|<span data-ttu-id="6abc7-145">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6abc7-145">Header</span></span>|<span data-ttu-id="6abc7-146">Значение</span><span class="sxs-lookup"><span data-stu-id="6abc7-146">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6abc7-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="6abc7-147">Authorization</span></span>|<span data-ttu-id="6abc7-148">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6abc7-148">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6abc7-149">Accept</span><span class="sxs-lookup"><span data-stu-id="6abc7-149">Accept</span></span>|<span data-ttu-id="6abc7-150">application/json</span><span class="sxs-lookup"><span data-stu-id="6abc7-150">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6abc7-151">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6abc7-151">Request body</span></span>
<span data-ttu-id="6abc7-152">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6abc7-152">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="6abc7-153">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="6abc7-153">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="6abc7-154">Свойство</span><span class="sxs-lookup"><span data-stu-id="6abc7-154">Property</span></span>|<span data-ttu-id="6abc7-155">Тип</span><span class="sxs-lookup"><span data-stu-id="6abc7-155">Type</span></span>|<span data-ttu-id="6abc7-156">Описание</span><span class="sxs-lookup"><span data-stu-id="6abc7-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6abc7-157">id</span><span class="sxs-lookup"><span data-stu-id="6abc7-157">id</span></span>|<span data-ttu-id="6abc7-158">String</span><span class="sxs-lookup"><span data-stu-id="6abc7-158">String</span></span>|<span data-ttu-id="6abc7-159">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="6abc7-159">Unique Identifier for the device</span></span>|
|<span data-ttu-id="6abc7-160">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="6abc7-160">**Device configuration**</span></span>|
|<span data-ttu-id="6abc7-161">settings</span><span class="sxs-lookup"><span data-stu-id="6abc7-161">settings</span></span>|[<span data-ttu-id="6abc7-162">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="6abc7-162">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="6abc7-163">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="6abc7-163">Account level settings.</span></span>|
|<span data-ttu-id="6abc7-164">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="6abc7-164">**Device management**</span></span>|
|<span data-ttu-id="6abc7-165">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="6abc7-165">subscriptionState</span></span>|[<span data-ttu-id="6abc7-166">девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="6abc7-166">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="6abc7-167">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="6abc7-167">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="6abc7-168">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="6abc7-168">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="6abc7-169">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="6abc7-169">**Onboarding**</span></span>|
|<span data-ttu-id="6abc7-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="6abc7-170">intuneBrand</span></span>|[<span data-ttu-id="6abc7-171">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="6abc7-171">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="6abc7-172">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="6abc7-172">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="6abc7-173">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="6abc7-173">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="6abc7-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="6abc7-174">Response</span></span>
<span data-ttu-id="6abc7-175">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6abc7-175">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6abc7-176">Пример</span><span class="sxs-lookup"><span data-stu-id="6abc7-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="6abc7-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="6abc7-177">Request</span></span>
<span data-ttu-id="6abc7-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6abc7-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6abc7-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="6abc7-179">Response</span></span>

<span data-ttu-id="6abc7-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6abc7-180">Here is an example of the response.</span></span> <span data-ttu-id="6abc7-181">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="6abc7-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6abc7-182">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="6abc7-182">Returned properties vary according to workflow and context.</span></span>

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






