---
title: Получение deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bbbe6c21d602266be2223fbd72b10ae9f51f7818
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898383"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="5242d-103">Получение deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5242d-103">Get deviceManagement</span></span>

> <span data-ttu-id="5242d-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5242d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5242d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5242d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5242d-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5242d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5242d-107">Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="5242d-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5242d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5242d-108">Prerequisites</span></span>

<span data-ttu-id="5242d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5242d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5242d-111">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="5242d-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="5242d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5242d-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="5242d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5242d-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="5242d-114">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="5242d-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="5242d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="5242d-116">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="5242d-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="5242d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="5242d-118">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="5242d-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="5242d-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5242d-120">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="5242d-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5242d-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="5242d-122">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="5242d-122">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="5242d-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5242d-124">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="5242d-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5242d-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="5242d-126">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="5242d-126">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="5242d-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="5242d-128">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="5242d-128">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="5242d-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5242d-130">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="5242d-130">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="5242d-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="5242d-132">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="5242d-132">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="5242d-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5242d-134">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="5242d-134">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5242d-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5242d-136">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="5242d-136">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="5242d-137">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-137">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="5242d-138">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="5242d-138">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="5242d-139">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-139">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="5242d-140">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="5242d-140">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="5242d-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5242d-142">&nbsp;&nbsp; **Управление расходами** по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="5242d-142">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="5242d-143">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-143">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5242d-144">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="5242d-144">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="5242d-145">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-145">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="5242d-146">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="5242d-146">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="5242d-147">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5242d-147">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="5242d-148">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5242d-148">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5242d-149">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5242d-149">Not supported.</span></span>|
| <span data-ttu-id="5242d-150">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5242d-150">Application</span></span> | <span data-ttu-id="5242d-151">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5242d-151">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="5242d-152">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5242d-152">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5242d-153">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5242d-153">Optional query parameters</span></span>

<span data-ttu-id="5242d-154">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5242d-154">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5242d-155">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5242d-155">Request headers</span></span>
|<span data-ttu-id="5242d-156">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5242d-156">Header</span></span>|<span data-ttu-id="5242d-157">Значение</span><span class="sxs-lookup"><span data-stu-id="5242d-157">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5242d-158">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5242d-158">Authorization</span></span>|<span data-ttu-id="5242d-159">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5242d-159">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5242d-160">Accept</span><span class="sxs-lookup"><span data-stu-id="5242d-160">Accept</span></span>|<span data-ttu-id="5242d-161">application/json</span><span class="sxs-lookup"><span data-stu-id="5242d-161">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5242d-162">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5242d-162">Request body</span></span>

<span data-ttu-id="5242d-163">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5242d-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5242d-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="5242d-164">Response</span></span>

<span data-ttu-id="5242d-165">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5242d-165">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5242d-166">Пример</span><span class="sxs-lookup"><span data-stu-id="5242d-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="5242d-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="5242d-167">Request</span></span>

<span data-ttu-id="5242d-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5242d-168">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="5242d-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="5242d-169">Response</span></span>

<span data-ttu-id="5242d-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5242d-170">Here are example of the response.</span></span> 

<span data-ttu-id="5242d-171">Note: объекты ответа, показанные здесь, могут быть усечены для краткости.</span><span class="sxs-lookup"><span data-stu-id="5242d-171">Note: The response objects shown here may be truncated for brevity.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

<span data-ttu-id="5242d-172">Возвращаются свойства, подходящие для рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="5242d-172">Properties appropriate for the workflow are returned.</span></span>

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



