---
title: Получение deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97c35f52182a82c2ddf2447e4d22935d8410826c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350918"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="38c9b-103">Получение deviceManagement</span><span class="sxs-lookup"><span data-stu-id="38c9b-103">Get deviceManagement</span></span>

> <span data-ttu-id="38c9b-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="38c9b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38c9b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38c9b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38c9b-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38c9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38c9b-107">Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="38c9b-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38c9b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="38c9b-108">Prerequisites</span></span>

<span data-ttu-id="38c9b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38c9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38c9b-111">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="38c9b-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="38c9b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38c9b-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="38c9b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38c9b-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="38c9b-114">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="38c9b-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="38c9b-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="38c9b-116">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="38c9b-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="38c9b-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="38c9b-118">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="38c9b-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="38c9b-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="38c9b-120">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="38c9b-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="38c9b-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="38c9b-122">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="38c9b-122">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="38c9b-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="38c9b-124">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="38c9b-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="38c9b-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="38c9b-126">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="38c9b-126">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="38c9b-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="38c9b-128">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="38c9b-128">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="38c9b-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="38c9b-130">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="38c9b-130">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="38c9b-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="38c9b-132">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="38c9b-132">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="38c9b-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="38c9b-134">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="38c9b-134">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="38c9b-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="38c9b-136">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="38c9b-136">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="38c9b-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="38c9b-138">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="38c9b-138">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="38c9b-139">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-139">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="38c9b-140">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="38c9b-140">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="38c9b-141">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-141">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="38c9b-142">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="38c9b-142">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="38c9b-143">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-143">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="38c9b-144">&nbsp;&nbsp; **Управление расходами** по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="38c9b-144">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="38c9b-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="38c9b-146">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="38c9b-146">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="38c9b-147">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-147">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="38c9b-148">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="38c9b-148">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="38c9b-149">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c9b-149">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="38c9b-150">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38c9b-150">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38c9b-151">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38c9b-151">Not supported.</span></span>|
| <span data-ttu-id="38c9b-152">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38c9b-152">Application</span></span> | <span data-ttu-id="38c9b-153">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38c9b-153">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="38c9b-154">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38c9b-154">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38c9b-155">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="38c9b-155">Optional query parameters</span></span>

<span data-ttu-id="38c9b-156">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="38c9b-156">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38c9b-157">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38c9b-157">Request headers</span></span>
|<span data-ttu-id="38c9b-158">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38c9b-158">Header</span></span>|<span data-ttu-id="38c9b-159">Значение</span><span class="sxs-lookup"><span data-stu-id="38c9b-159">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38c9b-160">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38c9b-160">Authorization</span></span>|<span data-ttu-id="38c9b-161">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38c9b-161">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38c9b-162">Accept</span><span class="sxs-lookup"><span data-stu-id="38c9b-162">Accept</span></span>|<span data-ttu-id="38c9b-163">application/json</span><span class="sxs-lookup"><span data-stu-id="38c9b-163">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38c9b-164">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38c9b-164">Request body</span></span>

<span data-ttu-id="38c9b-165">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38c9b-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38c9b-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="38c9b-166">Response</span></span>

<span data-ttu-id="38c9b-167">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="38c9b-167">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38c9b-168">Пример</span><span class="sxs-lookup"><span data-stu-id="38c9b-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="38c9b-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="38c9b-169">Request</span></span>

<span data-ttu-id="38c9b-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38c9b-170">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="38c9b-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="38c9b-171">Response</span></span>

<span data-ttu-id="38c9b-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="38c9b-172">Here are example of the response.</span></span> 

<span data-ttu-id="38c9b-173">Note: объекты ответа, показанные здесь, могут быть усечены для краткости.</span><span class="sxs-lookup"><span data-stu-id="38c9b-173">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="38c9b-174">Возвращаются свойства, подходящие для рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="38c9b-174">Properties appropriate for the workflow are returned.</span></span>

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






