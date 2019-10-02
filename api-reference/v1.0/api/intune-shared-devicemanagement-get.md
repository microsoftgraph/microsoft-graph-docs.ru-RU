---
title: Получение deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd689c80863504e5ae3766a11684a83ed89d086b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361471"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="48653-103">Получение deviceManagement</span><span class="sxs-lookup"><span data-stu-id="48653-103">Get deviceManagement</span></span>

> <span data-ttu-id="48653-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48653-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48653-105">Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="48653-105">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48653-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="48653-106">Prerequisites</span></span>
<span data-ttu-id="48653-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48653-109">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="48653-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="48653-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48653-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="48653-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48653-111">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="48653-112">&nbsp;&nbsp; Аудит</span><span class="sxs-lookup"><span data-stu-id="48653-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="48653-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="48653-114">&nbsp;&nbsp; Условия компании</span><span class="sxs-lookup"><span data-stu-id="48653-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="48653-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="48653-116">&nbsp;&nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="48653-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="48653-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="48653-118">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="48653-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="48653-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="48653-120">&nbsp;&nbsp; Регистрация</span><span class="sxs-lookup"><span data-stu-id="48653-120">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="48653-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="48653-122">&nbsp;&nbsp; Уведомление</span><span class="sxs-lookup"><span data-stu-id="48653-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="48653-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="48653-124">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="48653-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="48653-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="48653-126">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="48653-126">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="48653-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="48653-128">&nbsp;&nbsp; Удаленная помощь</span><span class="sxs-lookup"><span data-stu-id="48653-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="48653-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="48653-130">&nbsp;&nbsp; Управление расходами по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="48653-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="48653-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="48653-132">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="48653-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="48653-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="48653-134">&nbsp;&nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="48653-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="48653-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="48653-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="48653-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48653-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48653-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48653-137">Not supported.</span></span>|
| <span data-ttu-id="48653-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48653-138">Application</span></span> | <span data-ttu-id="48653-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48653-139">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="48653-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48653-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48653-141">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48653-141">Optional query parameters</span></span>
<span data-ttu-id="48653-142">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="48653-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="48653-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48653-143">Request headers</span></span>
|<span data-ttu-id="48653-144">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48653-144">Header</span></span>|<span data-ttu-id="48653-145">Значение</span><span class="sxs-lookup"><span data-stu-id="48653-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48653-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48653-146">Authorization</span></span>|<span data-ttu-id="48653-147">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48653-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48653-148">Accept</span><span class="sxs-lookup"><span data-stu-id="48653-148">Accept</span></span>|<span data-ttu-id="48653-149">application/json</span><span class="sxs-lookup"><span data-stu-id="48653-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48653-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48653-150">Request body</span></span>
<span data-ttu-id="48653-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48653-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48653-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="48653-152">Response</span></span>
<span data-ttu-id="48653-153">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="48653-153">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48653-154">Пример</span><span class="sxs-lookup"><span data-stu-id="48653-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="48653-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="48653-155">Request</span></span>
<span data-ttu-id="48653-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48653-156">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="48653-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="48653-157">Response</span></span>
<span data-ttu-id="48653-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48653-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




