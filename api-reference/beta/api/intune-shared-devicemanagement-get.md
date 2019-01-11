---
title: Получение объекта deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c00b60793209904ce184de25f12f1f4ad14fad1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862638"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="b6167-103">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="b6167-103">Get deviceManagement</span></span>

> <span data-ttu-id="b6167-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6167-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6167-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6167-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6167-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6167-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6167-107">Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="b6167-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6167-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b6167-108">Prerequisites</span></span>

<span data-ttu-id="b6167-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6167-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6167-111">Разрешение&nbsp;тип&nbsp;(с&nbsp;рабочего процесса)</span><span class="sxs-lookup"><span data-stu-id="b6167-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="b6167-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6167-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="b6167-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6167-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="b6167-114">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="b6167-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="b6167-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b6167-116">&nbsp; &nbsp; **аудита;**</span><span class="sxs-lookup"><span data-stu-id="b6167-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="b6167-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b6167-118">&nbsp;&nbsp; **Компании термины**</span><span class="sxs-lookup"><span data-stu-id="b6167-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="b6167-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b6167-120">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="b6167-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b6167-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b6167-122">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="b6167-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b6167-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b6167-124">&nbsp;&nbsp; **Электронных диспетчера установки**</span><span class="sxs-lookup"><span data-stu-id="b6167-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="b6167-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b6167-126">&nbsp; &nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="b6167-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="b6167-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b6167-128">&nbsp;&nbsp; **Разграничения**</span><span class="sxs-lookup"><span data-stu-id="b6167-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="b6167-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b6167-130">&nbsp;&nbsp; **Уведомлений**</span><span class="sxs-lookup"><span data-stu-id="b6167-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="b6167-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b6167-132">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="b6167-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b6167-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b6167-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="b6167-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="b6167-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="b6167-136">&nbsp;&nbsp; **Удаленного доступа**</span><span class="sxs-lookup"><span data-stu-id="b6167-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="b6167-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b6167-138">&nbsp;&nbsp; **Удаленный помощник**</span><span class="sxs-lookup"><span data-stu-id="b6167-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="b6167-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b6167-140">&nbsp;&nbsp; **Управления расходами телекоммуникации**</span><span class="sxs-lookup"><span data-stu-id="b6167-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="b6167-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b6167-142">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="b6167-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b6167-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b6167-144">&nbsp;&nbsp; **Защита информации Windows**</span><span class="sxs-lookup"><span data-stu-id="b6167-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="b6167-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6167-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b6167-146">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6167-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6167-147">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6167-147">Not supported.</span></span>|
| <span data-ttu-id="b6167-148">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6167-148">Application</span></span> | <span data-ttu-id="b6167-149">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6167-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="b6167-150">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6167-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6167-151">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b6167-151">Optional query parameters</span></span>

<span data-ttu-id="b6167-152">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b6167-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6167-153">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6167-153">Request headers</span></span>
|<span data-ttu-id="b6167-154">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6167-154">Header</span></span>|<span data-ttu-id="b6167-155">Значение</span><span class="sxs-lookup"><span data-stu-id="b6167-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6167-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6167-156">Authorization</span></span>|<span data-ttu-id="b6167-157">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b6167-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6167-158">Accept</span><span class="sxs-lookup"><span data-stu-id="b6167-158">Accept</span></span>|<span data-ttu-id="b6167-159">application/json</span><span class="sxs-lookup"><span data-stu-id="b6167-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6167-160">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b6167-160">Request body</span></span>

<span data-ttu-id="b6167-161">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6167-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6167-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6167-162">Response</span></span>

<span data-ttu-id="b6167-163">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b6167-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6167-164">Пример</span><span class="sxs-lookup"><span data-stu-id="b6167-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6167-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6167-165">Request</span></span>

<span data-ttu-id="b6167-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6167-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="b6167-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6167-167">Response</span></span>

<span data-ttu-id="b6167-168">Вот пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b6167-168">Here are example of the response.</span></span> 

<span data-ttu-id="b6167-169">Примечание: Для краткости может усекаться объекты ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="b6167-169">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="b6167-170">Возвращаются свойства, подходящую для рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="b6167-170">Properties appropriate for the workflow are returned.</span></span>

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



