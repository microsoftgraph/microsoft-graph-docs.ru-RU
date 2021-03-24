---
title: Get enrollmentTroubleshootingEvent
description: Чтение свойств и связей объекта enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f80bbe052d36ae2803a470b684eda14c0b1db17
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141507"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="e892f-103">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e892f-103">Get enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="e892f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e892f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e892f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e892f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e892f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e892f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e892f-107">Чтение свойств и связей объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e892f-107">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e892f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e892f-108">Prerequisites</span></span>
<span data-ttu-id="e892f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e892f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e892f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e892f-111">Permission type</span></span>|<span data-ttu-id="e892f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e892f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e892f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e892f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e892f-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e892f-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e892f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e892f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e892f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e892f-116">Not supported.</span></span>|
|<span data-ttu-id="e892f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e892f-117">Application</span></span>|<span data-ttu-id="e892f-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e892f-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e892f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e892f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e892f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e892f-120">Optional query parameters</span></span>
<span data-ttu-id="e892f-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e892f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e892f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e892f-122">Request headers</span></span>
|<span data-ttu-id="e892f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e892f-123">Header</span></span>|<span data-ttu-id="e892f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e892f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e892f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e892f-125">Authorization</span></span>|<span data-ttu-id="e892f-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e892f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e892f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e892f-127">Accept</span></span>|<span data-ttu-id="e892f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e892f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e892f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e892f-129">Request body</span></span>
<span data-ttu-id="e892f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e892f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e892f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e892f-131">Response</span></span>
<span data-ttu-id="e892f-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e892f-132">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e892f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e892f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e892f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e892f-134">Request</span></span>
<span data-ttu-id="e892f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e892f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="e892f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e892f-136">Response</span></span>
<span data-ttu-id="e892f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e892f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1318

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
    "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value",
    "troubleshootingErrorDetails": {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
      "context": "Context value",
      "failure": "Failure value",
      "failureDetails": "Failure Details value",
      "remediation": "Remediation value",
      "resources": [
        {
          "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
          "text": "Text value",
          "link": "Link value"
        }
      ]
    },
    "eventName": "Event Name value",
    "additionalInformation": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "operatingSystem": "Operating System value",
    "osVersion": "Os Version value",
    "userId": "User Id value",
    "deviceId": "Device Id value",
    "enrollmentType": "userEnrollment",
    "failureCategory": "authentication",
    "failureReason": "Failure Reason value"
  }
}
```




