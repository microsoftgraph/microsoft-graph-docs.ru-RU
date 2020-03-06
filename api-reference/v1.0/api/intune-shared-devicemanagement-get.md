---
title: Получение deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 78b9c2a70a594feb0f1ab0fb8ccbf333a0883056
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512078"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="7f87d-103">Получение deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7f87d-103">Get deviceManagement</span></span>

<span data-ttu-id="7f87d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f87d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f87d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f87d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f87d-106">Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7f87d-106">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f87d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f87d-107">Prerequisites</span></span>
<span data-ttu-id="7f87d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f87d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f87d-110">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="7f87d-110">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="7f87d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f87d-111">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="7f87d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f87d-112">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="7f87d-113">&nbsp;&nbsp; Аудит</span><span class="sxs-lookup"><span data-stu-id="7f87d-113">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="7f87d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="7f87d-115">&nbsp;&nbsp; Условия компании</span><span class="sxs-lookup"><span data-stu-id="7f87d-115">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="7f87d-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7f87d-117">&nbsp;&nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="7f87d-117">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="7f87d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="7f87d-119">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="7f87d-119">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="7f87d-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="7f87d-121">&nbsp;&nbsp; Регистрация</span><span class="sxs-lookup"><span data-stu-id="7f87d-121">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="7f87d-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7f87d-123">&nbsp;&nbsp; Уведомление</span><span class="sxs-lookup"><span data-stu-id="7f87d-123">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="7f87d-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7f87d-125">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="7f87d-125">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="7f87d-126">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-126">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7f87d-127">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="7f87d-127">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="7f87d-128">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-128">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="7f87d-129">&nbsp;&nbsp; Удаленная помощь</span><span class="sxs-lookup"><span data-stu-id="7f87d-129">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="7f87d-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7f87d-131">&nbsp;&nbsp; Управление расходами по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="7f87d-131">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="7f87d-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7f87d-133">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="7f87d-133">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="7f87d-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="7f87d-135">&nbsp;&nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="7f87d-135">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="7f87d-136">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f87d-136">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="7f87d-137">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f87d-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f87d-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f87d-138">Not supported.</span></span>|
| <span data-ttu-id="7f87d-139">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f87d-139">Application</span></span> | <span data-ttu-id="7f87d-140">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f87d-140">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="7f87d-141">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f87d-141">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f87d-142">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f87d-142">Optional query parameters</span></span>
<span data-ttu-id="7f87d-143">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7f87d-143">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7f87d-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f87d-144">Request headers</span></span>
|<span data-ttu-id="7f87d-145">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f87d-145">Header</span></span>|<span data-ttu-id="7f87d-146">Значение</span><span class="sxs-lookup"><span data-stu-id="7f87d-146">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f87d-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f87d-147">Authorization</span></span>|<span data-ttu-id="7f87d-148">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f87d-148">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f87d-149">Accept</span><span class="sxs-lookup"><span data-stu-id="7f87d-149">Accept</span></span>|<span data-ttu-id="7f87d-150">application/json</span><span class="sxs-lookup"><span data-stu-id="7f87d-150">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f87d-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f87d-151">Request body</span></span>
<span data-ttu-id="7f87d-152">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f87d-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f87d-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f87d-153">Response</span></span>
<span data-ttu-id="7f87d-154">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7f87d-154">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f87d-155">Пример</span><span class="sxs-lookup"><span data-stu-id="7f87d-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f87d-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f87d-156">Request</span></span>
<span data-ttu-id="7f87d-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f87d-157">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="7f87d-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f87d-158">Response</span></span>
<span data-ttu-id="7f87d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f87d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




