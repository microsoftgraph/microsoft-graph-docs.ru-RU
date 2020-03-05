---
title: Список объектов enrollmentTroubleshootingEvent
description: Список свойств и связей объектов enrollmentTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 82d40704ddbaaef1be7bbe509f4463a971a84f39
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457645"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="34bf0-103">Список объектов enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="34bf0-103">List enrollmentTroubleshootingEvents</span></span>

<span data-ttu-id="34bf0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="34bf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34bf0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34bf0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34bf0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34bf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34bf0-107">Список свойств и связей объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="34bf0-107">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34bf0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="34bf0-108">Prerequisites</span></span>
<span data-ttu-id="34bf0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34bf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34bf0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34bf0-111">Permission type</span></span>|<span data-ttu-id="34bf0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34bf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34bf0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34bf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34bf0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34bf0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="34bf0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34bf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34bf0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34bf0-116">Not supported.</span></span>|
|<span data-ttu-id="34bf0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34bf0-117">Application</span></span>|<span data-ttu-id="34bf0-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34bf0-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34bf0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34bf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="34bf0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="34bf0-120">Request headers</span></span>
|<span data-ttu-id="34bf0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34bf0-121">Header</span></span>|<span data-ttu-id="34bf0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="34bf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34bf0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34bf0-123">Authorization</span></span>|<span data-ttu-id="34bf0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34bf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34bf0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="34bf0-125">Accept</span></span>|<span data-ttu-id="34bf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34bf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34bf0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34bf0-127">Request body</span></span>
<span data-ttu-id="34bf0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34bf0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34bf0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="34bf0-129">Response</span></span>
<span data-ttu-id="34bf0-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="34bf0-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34bf0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="34bf0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="34bf0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="34bf0-132">Request</span></span>
<span data-ttu-id="34bf0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34bf0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="34bf0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="34bf0-134">Response</span></span>
<span data-ttu-id="34bf0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34bf0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1400

{
  "value": [
    {
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
  ]
}
```





