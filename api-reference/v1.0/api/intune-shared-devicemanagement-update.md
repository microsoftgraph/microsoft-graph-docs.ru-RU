---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c96877d25476ede3cee6ce407c1df84f08448a9a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576946"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="14a47-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="14a47-103">Update deviceManagement</span></span>

> <span data-ttu-id="14a47-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14a47-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14a47-105">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="14a47-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14a47-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="14a47-106">Prerequisites</span></span>
<span data-ttu-id="14a47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14a47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14a47-109">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="14a47-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="14a47-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14a47-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="14a47-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14a47-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="14a47-112">&nbsp;&nbsp; Аудит</span><span class="sxs-lookup"><span data-stu-id="14a47-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="14a47-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-114">&nbsp;&nbsp; Условия компании</span><span class="sxs-lookup"><span data-stu-id="14a47-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="14a47-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-116">&nbsp;&nbsp; Корпоративная регистрация</span><span class="sxs-lookup"><span data-stu-id="14a47-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="14a47-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="14a47-118">&nbsp;&nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="14a47-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="14a47-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-120">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="14a47-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="14a47-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-122">&nbsp;&nbsp; Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="14a47-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="14a47-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-124">&nbsp;&nbsp; Уведомление</span><span class="sxs-lookup"><span data-stu-id="14a47-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="14a47-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-126">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="14a47-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="14a47-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-128">&nbsp;&nbsp; Управление доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="14a47-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="14a47-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-130">&nbsp;&nbsp; Удаленная помощь</span><span class="sxs-lookup"><span data-stu-id="14a47-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="14a47-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-132">&nbsp;&nbsp; Управление расходами по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="14a47-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="14a47-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-134">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="14a47-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="14a47-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-136">&nbsp;&nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="14a47-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="14a47-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a47-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="14a47-138">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14a47-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14a47-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14a47-139">Not supported.</span></span>|
| <span data-ttu-id="14a47-140">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14a47-140">Application</span></span> | <span data-ttu-id="14a47-141">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14a47-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14a47-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14a47-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="14a47-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14a47-143">Request headers</span></span>
|<span data-ttu-id="14a47-144">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14a47-144">Header</span></span>|<span data-ttu-id="14a47-145">Значение</span><span class="sxs-lookup"><span data-stu-id="14a47-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14a47-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14a47-146">Authorization</span></span>|<span data-ttu-id="14a47-147">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14a47-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14a47-148">Accept</span><span class="sxs-lookup"><span data-stu-id="14a47-148">Accept</span></span>|<span data-ttu-id="14a47-149">application/json</span><span class="sxs-lookup"><span data-stu-id="14a47-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14a47-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14a47-150">Request body</span></span>
<span data-ttu-id="14a47-151">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14a47-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="14a47-152">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="14a47-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="14a47-153">Свойство</span><span class="sxs-lookup"><span data-stu-id="14a47-153">Property</span></span>|<span data-ttu-id="14a47-154">Тип</span><span class="sxs-lookup"><span data-stu-id="14a47-154">Type</span></span>|<span data-ttu-id="14a47-155">Описание</span><span class="sxs-lookup"><span data-stu-id="14a47-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14a47-156">id</span><span class="sxs-lookup"><span data-stu-id="14a47-156">id</span></span>|<span data-ttu-id="14a47-157">String</span><span class="sxs-lookup"><span data-stu-id="14a47-157">String</span></span>|<span data-ttu-id="14a47-158">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="14a47-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="14a47-159">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="14a47-159">**Device configuration**</span></span>|
|<span data-ttu-id="14a47-160">settings</span><span class="sxs-lookup"><span data-stu-id="14a47-160">settings</span></span>|[<span data-ttu-id="14a47-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="14a47-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="14a47-162">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="14a47-162">Account level settings.</span></span>|
|<span data-ttu-id="14a47-163">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="14a47-163">**Device management**</span></span>|
|<span data-ttu-id="14a47-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="14a47-164">subscriptionState</span></span>|[<span data-ttu-id="14a47-165">Девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="14a47-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="14a47-166">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="14a47-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="14a47-167">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="14a47-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="14a47-168">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="14a47-168">**Onboarding**</span></span>|
|<span data-ttu-id="14a47-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="14a47-169">intuneBrand</span></span>|[<span data-ttu-id="14a47-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="14a47-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="14a47-171">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="14a47-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="14a47-172">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="14a47-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="14a47-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="14a47-173">Response</span></span>
<span data-ttu-id="14a47-174">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="14a47-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14a47-175">Пример</span><span class="sxs-lookup"><span data-stu-id="14a47-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="14a47-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="14a47-176">Request</span></span>
<span data-ttu-id="14a47-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14a47-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14a47-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="14a47-178">Response</span></span>

<span data-ttu-id="14a47-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14a47-179">Here is an example of the response.</span></span> <span data-ttu-id="14a47-180">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="14a47-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="14a47-181">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="14a47-181">Returned properties vary according to workflow and context.</span></span>

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



