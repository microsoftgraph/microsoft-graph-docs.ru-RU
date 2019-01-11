---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e88b6379e340865adeb41bb0430fd8eecc8f0b69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860685"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="69b33-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="69b33-103">Update deviceManagement</span></span>

> <span data-ttu-id="69b33-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="69b33-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69b33-105">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="69b33-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69b33-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="69b33-106">Prerequisites</span></span>
<span data-ttu-id="69b33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69b33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69b33-109">Разрешение&nbsp;тип&nbsp;(с&nbsp;рабочего процесса)</span><span class="sxs-lookup"><span data-stu-id="69b33-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="69b33-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69b33-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="69b33-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69b33-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="69b33-112">&nbsp;&nbsp; Аудита</span><span class="sxs-lookup"><span data-stu-id="69b33-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="69b33-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-114">&nbsp;&nbsp; Компании термины</span><span class="sxs-lookup"><span data-stu-id="69b33-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="69b33-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-116">&nbsp;&nbsp; Корпоративной подачи заявок</span><span class="sxs-lookup"><span data-stu-id="69b33-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="69b33-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="69b33-118">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="69b33-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="69b33-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-120">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="69b33-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="69b33-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-122">&nbsp;&nbsp; Защиты конечной точки</span><span class="sxs-lookup"><span data-stu-id="69b33-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="69b33-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-124">&nbsp;&nbsp; Уведомлений</span><span class="sxs-lookup"><span data-stu-id="69b33-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="69b33-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-126">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="69b33-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="69b33-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-128">&nbsp;&nbsp; Управления доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="69b33-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="69b33-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-130">&nbsp;&nbsp; Удаленный помощник</span><span class="sxs-lookup"><span data-stu-id="69b33-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="69b33-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-132">&nbsp;&nbsp; Управления расходами телекоммуникации</span><span class="sxs-lookup"><span data-stu-id="69b33-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="69b33-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-134">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="69b33-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="69b33-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-136">&nbsp;&nbsp; Защита информации Windows</span><span class="sxs-lookup"><span data-stu-id="69b33-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="69b33-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b33-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="69b33-138">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69b33-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69b33-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69b33-139">Not supported.</span></span>|
| <span data-ttu-id="69b33-140">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69b33-140">Application</span></span> | <span data-ttu-id="69b33-141">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69b33-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69b33-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69b33-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="69b33-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69b33-143">Request headers</span></span>
|<span data-ttu-id="69b33-144">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69b33-144">Header</span></span>|<span data-ttu-id="69b33-145">Значение</span><span class="sxs-lookup"><span data-stu-id="69b33-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69b33-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="69b33-146">Authorization</span></span>|<span data-ttu-id="69b33-147">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="69b33-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69b33-148">Accept</span><span class="sxs-lookup"><span data-stu-id="69b33-148">Accept</span></span>|<span data-ttu-id="69b33-149">application/json</span><span class="sxs-lookup"><span data-stu-id="69b33-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69b33-150">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69b33-150">Request body</span></span>
<span data-ttu-id="69b33-151">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69b33-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="69b33-152">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="69b33-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="69b33-153">Свойство</span><span class="sxs-lookup"><span data-stu-id="69b33-153">Property</span></span>|<span data-ttu-id="69b33-154">Тип</span><span class="sxs-lookup"><span data-stu-id="69b33-154">Type</span></span>|<span data-ttu-id="69b33-155">Описание</span><span class="sxs-lookup"><span data-stu-id="69b33-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69b33-156">id</span><span class="sxs-lookup"><span data-stu-id="69b33-156">id</span></span>|<span data-ttu-id="69b33-157">String</span><span class="sxs-lookup"><span data-stu-id="69b33-157">String</span></span>|<span data-ttu-id="69b33-158">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="69b33-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="69b33-159">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="69b33-159">**Device configuration**</span></span>|
|<span data-ttu-id="69b33-160">settings</span><span class="sxs-lookup"><span data-stu-id="69b33-160">settings</span></span>|[<span data-ttu-id="69b33-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="69b33-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="69b33-162">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="69b33-162">Account level settings.</span></span>|
|<span data-ttu-id="69b33-163">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="69b33-163">**Device management**</span></span>|
|<span data-ttu-id="69b33-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="69b33-164">subscriptionState</span></span>|[<span data-ttu-id="69b33-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="69b33-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="69b33-166">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="69b33-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="69b33-167">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="69b33-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="69b33-168">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="69b33-168">**Onboarding**</span></span>|
|<span data-ttu-id="69b33-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="69b33-169">intuneBrand</span></span>|[<span data-ttu-id="69b33-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="69b33-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="69b33-171">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="69b33-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="69b33-172">Поддержка свойств текст запроса изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="69b33-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="69b33-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="69b33-173">Response</span></span>
<span data-ttu-id="69b33-174">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="69b33-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69b33-175">Пример</span><span class="sxs-lookup"><span data-stu-id="69b33-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="69b33-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="69b33-176">Request</span></span>
<span data-ttu-id="69b33-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69b33-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="69b33-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="69b33-178">Response</span></span>

<span data-ttu-id="69b33-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="69b33-179">Here is an example of the response.</span></span> <span data-ttu-id="69b33-180">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="69b33-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="69b33-181">Возвращаемых свойств различаться в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="69b33-181">Returned properties vary according to workflow and context.</span></span>

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



