---
title: Получение объекта deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 89156113d0b357bc0d7a76cadad8c2ab7e2e4b91
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816270"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="f21a9-103">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f21a9-103">Get deviceManagement</span></span>

> <span data-ttu-id="f21a9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f21a9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f21a9-105">Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="f21a9-105">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f21a9-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f21a9-106">Prerequisites</span></span>
<span data-ttu-id="f21a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f21a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f21a9-109">Разрешение&nbsp;тип&nbsp;(с&nbsp;рабочего процесса)</span><span class="sxs-lookup"><span data-stu-id="f21a9-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="f21a9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f21a9-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="f21a9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f21a9-111">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="f21a9-112">&nbsp;&nbsp; Аудита</span><span class="sxs-lookup"><span data-stu-id="f21a9-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="f21a9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="f21a9-114">&nbsp;&nbsp; Компании термины</span><span class="sxs-lookup"><span data-stu-id="f21a9-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="f21a9-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f21a9-116">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="f21a9-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="f21a9-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="f21a9-118">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="f21a9-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="f21a9-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="f21a9-120">&nbsp;&nbsp; Подачи заявок</span><span class="sxs-lookup"><span data-stu-id="f21a9-120">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="f21a9-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f21a9-122">&nbsp;&nbsp; Уведомлений</span><span class="sxs-lookup"><span data-stu-id="f21a9-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="f21a9-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f21a9-124">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="f21a9-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="f21a9-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f21a9-126">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="f21a9-126">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="f21a9-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="f21a9-128">&nbsp;&nbsp; Удаленный помощник</span><span class="sxs-lookup"><span data-stu-id="f21a9-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="f21a9-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f21a9-130">&nbsp;&nbsp; Управления расходами телекоммуникации</span><span class="sxs-lookup"><span data-stu-id="f21a9-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="f21a9-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f21a9-132">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="f21a9-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="f21a9-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="f21a9-134">&nbsp;&nbsp; Защита информации Windows</span><span class="sxs-lookup"><span data-stu-id="f21a9-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="f21a9-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f21a9-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="f21a9-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f21a9-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f21a9-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f21a9-137">Not supported.</span></span>|
| <span data-ttu-id="f21a9-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f21a9-138">Application</span></span> | <span data-ttu-id="f21a9-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f21a9-139">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="f21a9-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f21a9-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f21a9-141">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f21a9-141">Optional query parameters</span></span>
<span data-ttu-id="f21a9-142">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f21a9-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f21a9-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f21a9-143">Request headers</span></span>
|<span data-ttu-id="f21a9-144">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f21a9-144">Header</span></span>|<span data-ttu-id="f21a9-145">Значение</span><span class="sxs-lookup"><span data-stu-id="f21a9-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f21a9-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="f21a9-146">Authorization</span></span>|<span data-ttu-id="f21a9-147">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f21a9-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f21a9-148">Accept</span><span class="sxs-lookup"><span data-stu-id="f21a9-148">Accept</span></span>|<span data-ttu-id="f21a9-149">application/json</span><span class="sxs-lookup"><span data-stu-id="f21a9-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f21a9-150">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f21a9-150">Request body</span></span>
<span data-ttu-id="f21a9-151">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f21a9-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f21a9-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="f21a9-152">Response</span></span>
<span data-ttu-id="f21a9-153">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f21a9-153">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f21a9-154">Пример</span><span class="sxs-lookup"><span data-stu-id="f21a9-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="f21a9-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="f21a9-155">Request</span></span>
<span data-ttu-id="f21a9-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f21a9-156">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="f21a9-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="f21a9-157">Response</span></span>
<span data-ttu-id="f21a9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f21a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



