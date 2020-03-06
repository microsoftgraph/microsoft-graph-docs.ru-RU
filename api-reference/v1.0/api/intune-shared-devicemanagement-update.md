---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c9529e9c6edcee009106544244c91a9b54ac889
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512064"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="c77fd-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c77fd-103">Update deviceManagement</span></span>

<span data-ttu-id="c77fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c77fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c77fd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c77fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c77fd-106">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c77fd-106">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c77fd-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c77fd-107">Prerequisites</span></span>
<span data-ttu-id="c77fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c77fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c77fd-110">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="c77fd-110">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="c77fd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c77fd-111">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="c77fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c77fd-112">Delegated (work or school account)</span></span> |
| <span data-ttu-id="c77fd-113">&nbsp;&nbsp; Аудит</span><span class="sxs-lookup"><span data-stu-id="c77fd-113">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="c77fd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-115">&nbsp;&nbsp; Условия компании</span><span class="sxs-lookup"><span data-stu-id="c77fd-115">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="c77fd-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-117">&nbsp;&nbsp; Корпоративная регистрация</span><span class="sxs-lookup"><span data-stu-id="c77fd-117">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="c77fd-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c77fd-119">&nbsp;&nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="c77fd-119">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="c77fd-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-121">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="c77fd-121">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="c77fd-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-123">&nbsp;&nbsp; Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="c77fd-123">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="c77fd-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-125">&nbsp;&nbsp; Уведомление</span><span class="sxs-lookup"><span data-stu-id="c77fd-125">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="c77fd-126">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-126">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-127">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="c77fd-127">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="c77fd-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-129">&nbsp;&nbsp; Управление доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="c77fd-129">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="c77fd-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-130">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-131">&nbsp;&nbsp; Удаленная помощь</span><span class="sxs-lookup"><span data-stu-id="c77fd-131">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="c77fd-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-133">&nbsp;&nbsp; Управление расходами по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="c77fd-133">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="c77fd-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-135">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="c77fd-135">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="c77fd-136">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-136">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-137">&nbsp;&nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="c77fd-137">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="c77fd-138">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77fd-138">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c77fd-139">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c77fd-139">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c77fd-140">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c77fd-140">Not supported.</span></span>|
| <span data-ttu-id="c77fd-141">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c77fd-141">Application</span></span> | <span data-ttu-id="c77fd-142">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c77fd-142">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c77fd-143">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c77fd-143">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="c77fd-144">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c77fd-144">Request headers</span></span>
|<span data-ttu-id="c77fd-145">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c77fd-145">Header</span></span>|<span data-ttu-id="c77fd-146">Значение</span><span class="sxs-lookup"><span data-stu-id="c77fd-146">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c77fd-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="c77fd-147">Authorization</span></span>|<span data-ttu-id="c77fd-148">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c77fd-148">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c77fd-149">Accept</span><span class="sxs-lookup"><span data-stu-id="c77fd-149">Accept</span></span>|<span data-ttu-id="c77fd-150">application/json</span><span class="sxs-lookup"><span data-stu-id="c77fd-150">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c77fd-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c77fd-151">Request body</span></span>
<span data-ttu-id="c77fd-152">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c77fd-152">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="c77fd-153">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c77fd-153">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="c77fd-154">Свойство</span><span class="sxs-lookup"><span data-stu-id="c77fd-154">Property</span></span>|<span data-ttu-id="c77fd-155">Тип</span><span class="sxs-lookup"><span data-stu-id="c77fd-155">Type</span></span>|<span data-ttu-id="c77fd-156">Описание</span><span class="sxs-lookup"><span data-stu-id="c77fd-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c77fd-157">id</span><span class="sxs-lookup"><span data-stu-id="c77fd-157">id</span></span>|<span data-ttu-id="c77fd-158">Строка</span><span class="sxs-lookup"><span data-stu-id="c77fd-158">String</span></span>|<span data-ttu-id="c77fd-159">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="c77fd-159">Unique Identifier for the device</span></span>|
|<span data-ttu-id="c77fd-160">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="c77fd-160">**Device configuration**</span></span>|
|<span data-ttu-id="c77fd-161">settings</span><span class="sxs-lookup"><span data-stu-id="c77fd-161">settings</span></span>|[<span data-ttu-id="c77fd-162">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="c77fd-162">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="c77fd-163">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="c77fd-163">Account level settings.</span></span>|
|<span data-ttu-id="c77fd-164">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c77fd-164">**Device management**</span></span>|
|<span data-ttu-id="c77fd-165">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="c77fd-165">subscriptionState</span></span>|[<span data-ttu-id="c77fd-166">девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="c77fd-166">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="c77fd-167">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="c77fd-167">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="c77fd-168">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="c77fd-168">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="c77fd-169">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c77fd-169">**Onboarding**</span></span>|
|<span data-ttu-id="c77fd-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="c77fd-170">intuneBrand</span></span>|[<span data-ttu-id="c77fd-171">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="c77fd-171">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="c77fd-172">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="c77fd-172">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="c77fd-173">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="c77fd-173">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="c77fd-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="c77fd-174">Response</span></span>
<span data-ttu-id="c77fd-175">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c77fd-175">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c77fd-176">Пример</span><span class="sxs-lookup"><span data-stu-id="c77fd-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="c77fd-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="c77fd-177">Request</span></span>
<span data-ttu-id="c77fd-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c77fd-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c77fd-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="c77fd-179">Response</span></span>

<span data-ttu-id="c77fd-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c77fd-180">Here is an example of the response.</span></span> <span data-ttu-id="c77fd-181">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c77fd-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c77fd-182">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="c77fd-182">Returned properties vary according to workflow and context.</span></span>

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




