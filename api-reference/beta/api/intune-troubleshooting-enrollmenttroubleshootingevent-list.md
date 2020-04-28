---
title: Список объектов enrollmentTroubleshootingEvent
description: Список свойств и связей объектов enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5705fd0e500fda315b69479db2c1d916d002ebc7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473993"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="8a728-103">Список объектов enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8a728-103">List enrollmentTroubleshootingEvents</span></span>

<span data-ttu-id="8a728-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a728-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a728-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a728-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a728-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a728-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a728-107">Список свойств и связей объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8a728-107">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a728-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8a728-108">Prerequisites</span></span>
<span data-ttu-id="8a728-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a728-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a728-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a728-111">Permission type</span></span>|<span data-ttu-id="8a728-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a728-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a728-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a728-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a728-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a728-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8a728-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a728-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a728-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a728-116">Not supported.</span></span>|
|<span data-ttu-id="8a728-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a728-117">Application</span></span>|<span data-ttu-id="8a728-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a728-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a728-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a728-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="8a728-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8a728-120">Request headers</span></span>
|<span data-ttu-id="8a728-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a728-121">Header</span></span>|<span data-ttu-id="8a728-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8a728-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a728-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a728-123">Authorization</span></span>|<span data-ttu-id="8a728-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a728-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a728-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8a728-125">Accept</span></span>|<span data-ttu-id="8a728-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a728-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a728-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a728-127">Request body</span></span>
<span data-ttu-id="8a728-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8a728-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a728-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a728-129">Response</span></span>
<span data-ttu-id="8a728-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8a728-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a728-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8a728-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a728-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a728-132">Request</span></span>
<span data-ttu-id="8a728-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a728-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="8a728-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a728-134">Response</span></span>
<span data-ttu-id="8a728-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a728-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



