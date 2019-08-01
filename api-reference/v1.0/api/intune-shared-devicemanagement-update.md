---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b845a07d8199fcd4a997304f9095d7b364e0988a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023435"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="13c20-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="13c20-103">Update deviceManagement</span></span>

> <span data-ttu-id="13c20-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13c20-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13c20-105">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="13c20-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13c20-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="13c20-106">Prerequisites</span></span>
<span data-ttu-id="13c20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13c20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13c20-109">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="13c20-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="13c20-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13c20-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="13c20-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13c20-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="13c20-112">&nbsp;&nbsp; Аудит</span><span class="sxs-lookup"><span data-stu-id="13c20-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="13c20-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-114">&nbsp;&nbsp; Условия компании</span><span class="sxs-lookup"><span data-stu-id="13c20-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="13c20-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-116">&nbsp;&nbsp; Корпоративная регистрация</span><span class="sxs-lookup"><span data-stu-id="13c20-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="13c20-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="13c20-118">&nbsp;&nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="13c20-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="13c20-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-120">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="13c20-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="13c20-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-122">&nbsp;&nbsp; Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="13c20-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="13c20-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-124">&nbsp;&nbsp; Уведомление</span><span class="sxs-lookup"><span data-stu-id="13c20-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="13c20-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-126">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="13c20-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="13c20-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-128">&nbsp;&nbsp; Управление доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="13c20-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="13c20-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-130">&nbsp;&nbsp; Удаленная помощь</span><span class="sxs-lookup"><span data-stu-id="13c20-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="13c20-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-132">&nbsp;&nbsp; Управление расходами по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="13c20-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="13c20-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-134">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="13c20-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="13c20-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-136">&nbsp;&nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="13c20-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="13c20-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c20-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="13c20-138">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13c20-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13c20-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c20-139">Not supported.</span></span>|
| <span data-ttu-id="13c20-140">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13c20-140">Application</span></span> | <span data-ttu-id="13c20-141">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c20-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13c20-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13c20-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="13c20-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13c20-143">Request headers</span></span>
|<span data-ttu-id="13c20-144">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13c20-144">Header</span></span>|<span data-ttu-id="13c20-145">Значение</span><span class="sxs-lookup"><span data-stu-id="13c20-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13c20-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13c20-146">Authorization</span></span>|<span data-ttu-id="13c20-147">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13c20-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13c20-148">Accept</span><span class="sxs-lookup"><span data-stu-id="13c20-148">Accept</span></span>|<span data-ttu-id="13c20-149">application/json</span><span class="sxs-lookup"><span data-stu-id="13c20-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13c20-150">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="13c20-150">Request body</span></span>
<span data-ttu-id="13c20-151">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13c20-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="13c20-152">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="13c20-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="13c20-153">Свойство</span><span class="sxs-lookup"><span data-stu-id="13c20-153">Property</span></span>|<span data-ttu-id="13c20-154">Тип</span><span class="sxs-lookup"><span data-stu-id="13c20-154">Type</span></span>|<span data-ttu-id="13c20-155">Описание</span><span class="sxs-lookup"><span data-stu-id="13c20-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13c20-156">id</span><span class="sxs-lookup"><span data-stu-id="13c20-156">id</span></span>|<span data-ttu-id="13c20-157">String</span><span class="sxs-lookup"><span data-stu-id="13c20-157">String</span></span>|<span data-ttu-id="13c20-158">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="13c20-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="13c20-159">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="13c20-159">**Device configuration**</span></span>|
|<span data-ttu-id="13c20-160">settings</span><span class="sxs-lookup"><span data-stu-id="13c20-160">settings</span></span>|[<span data-ttu-id="13c20-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="13c20-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="13c20-162">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="13c20-162">Account level settings.</span></span>|
|<span data-ttu-id="13c20-163">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="13c20-163">**Device management**</span></span>|
|<span data-ttu-id="13c20-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="13c20-164">subscriptionState</span></span>|[<span data-ttu-id="13c20-165">Девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="13c20-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="13c20-166">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="13c20-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="13c20-167">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="13c20-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="13c20-168">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="13c20-168">**Onboarding**</span></span>|
|<span data-ttu-id="13c20-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="13c20-169">intuneBrand</span></span>|[<span data-ttu-id="13c20-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="13c20-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="13c20-171">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="13c20-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="13c20-172">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="13c20-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="13c20-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="13c20-173">Response</span></span>
<span data-ttu-id="13c20-174">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="13c20-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13c20-175">Пример</span><span class="sxs-lookup"><span data-stu-id="13c20-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="13c20-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="13c20-176">Request</span></span>
<span data-ttu-id="13c20-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13c20-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="13c20-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="13c20-178">Response</span></span>

<span data-ttu-id="13c20-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13c20-179">Here is an example of the response.</span></span> <span data-ttu-id="13c20-180">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="13c20-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="13c20-181">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="13c20-181">Returned properties vary according to workflow and context.</span></span>

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



