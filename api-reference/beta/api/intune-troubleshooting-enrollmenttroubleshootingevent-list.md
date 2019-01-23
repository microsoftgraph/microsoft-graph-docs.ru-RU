---
title: Список объектов enrollmentTroubleshootingEvent
description: Список свойств и связей объектов enrollmentTroubleshootingEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62a2718408ef1c90c92136cbf2faf87ad2eec63e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404325"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="22e99-103">Список объектов enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="22e99-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="22e99-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22e99-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22e99-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22e99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22e99-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22e99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22e99-107">Список свойств и связей объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="22e99-107">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22e99-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="22e99-108">Prerequisites</span></span>
<span data-ttu-id="22e99-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="22e99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="22e99-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22e99-111">Permission type</span></span>|<span data-ttu-id="22e99-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22e99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22e99-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22e99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22e99-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="22e99-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="22e99-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22e99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22e99-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22e99-116">Not supported.</span></span>|
|<span data-ttu-id="22e99-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22e99-117">Application</span></span>|<span data-ttu-id="22e99-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22e99-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22e99-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22e99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="22e99-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22e99-120">Request headers</span></span>
|<span data-ttu-id="22e99-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22e99-121">Header</span></span>|<span data-ttu-id="22e99-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22e99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22e99-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22e99-123">Authorization</span></span>|<span data-ttu-id="22e99-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="22e99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22e99-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22e99-125">Accept</span></span>|<span data-ttu-id="22e99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22e99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22e99-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22e99-127">Request body</span></span>
<span data-ttu-id="22e99-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22e99-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22e99-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="22e99-129">Response</span></span>
<span data-ttu-id="22e99-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="22e99-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22e99-131">Пример</span><span class="sxs-lookup"><span data-stu-id="22e99-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="22e99-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="22e99-132">Request</span></span>
<span data-ttu-id="22e99-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22e99-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="22e99-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="22e99-134">Response</span></span>
<span data-ttu-id="22e99-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="22e99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




