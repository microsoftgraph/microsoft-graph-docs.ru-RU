---
title: Получение объекта deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: tfitzmac
ms.openlocfilehash: 65b13da27c16d6b4d9976eb2f7d0d326dfd872c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334343"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="486b4-103">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="486b4-103">Get deviceManagement</span></span>

> <span data-ttu-id="486b4-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="486b4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="486b4-105">Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="486b4-105">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="486b4-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="486b4-106">Prerequisites</span></span>
<span data-ttu-id="486b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="486b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="486b4-109">Разрешение&nbsp;тип&nbsp;(с&nbsp;рабочего процесса)</span><span class="sxs-lookup"><span data-stu-id="486b4-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="486b4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="486b4-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="486b4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="486b4-111">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="486b4-112">&nbsp;&nbsp; Аудита</span><span class="sxs-lookup"><span data-stu-id="486b4-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="486b4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="486b4-114">&nbsp;&nbsp; Компании термины</span><span class="sxs-lookup"><span data-stu-id="486b4-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="486b4-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="486b4-116">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="486b4-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="486b4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="486b4-118">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="486b4-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="486b4-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="486b4-120">&nbsp;&nbsp; Подачи заявок</span><span class="sxs-lookup"><span data-stu-id="486b4-120">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="486b4-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="486b4-122">&nbsp;&nbsp; Уведомлений</span><span class="sxs-lookup"><span data-stu-id="486b4-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="486b4-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="486b4-124">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="486b4-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="486b4-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="486b4-126">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="486b4-126">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="486b4-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="486b4-128">&nbsp;&nbsp; Удаленный помощник</span><span class="sxs-lookup"><span data-stu-id="486b4-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="486b4-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="486b4-130">&nbsp;&nbsp; Управления расходами телекоммуникации</span><span class="sxs-lookup"><span data-stu-id="486b4-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="486b4-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="486b4-132">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="486b4-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="486b4-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="486b4-134">&nbsp;&nbsp; Защита информации Windows</span><span class="sxs-lookup"><span data-stu-id="486b4-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="486b4-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="486b4-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="486b4-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="486b4-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="486b4-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="486b4-137">Not supported.</span></span>|
| <span data-ttu-id="486b4-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="486b4-138">Application</span></span> | <span data-ttu-id="486b4-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="486b4-139">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="486b4-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="486b4-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="486b4-141">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="486b4-141">Optional query parameters</span></span>
<span data-ttu-id="486b4-142">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="486b4-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="486b4-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="486b4-143">Request headers</span></span>
|<span data-ttu-id="486b4-144">Заголовок</span><span class="sxs-lookup"><span data-stu-id="486b4-144">Header</span></span>|<span data-ttu-id="486b4-145">Значение</span><span class="sxs-lookup"><span data-stu-id="486b4-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="486b4-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="486b4-146">Authorization</span></span>|<span data-ttu-id="486b4-147">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="486b4-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="486b4-148">Accept</span><span class="sxs-lookup"><span data-stu-id="486b4-148">Accept</span></span>|<span data-ttu-id="486b4-149">application/json</span><span class="sxs-lookup"><span data-stu-id="486b4-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="486b4-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="486b4-150">Request body</span></span>
<span data-ttu-id="486b4-151">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="486b4-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="486b4-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="486b4-152">Response</span></span>
<span data-ttu-id="486b4-153">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="486b4-153">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="486b4-154">Пример</span><span class="sxs-lookup"><span data-stu-id="486b4-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="486b4-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="486b4-155">Request</span></span>
<span data-ttu-id="486b4-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="486b4-156">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="486b4-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="486b4-157">Response</span></span>
<span data-ttu-id="486b4-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="486b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



