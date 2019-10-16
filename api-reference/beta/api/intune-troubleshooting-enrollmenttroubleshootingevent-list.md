---
title: Список объектов enrollmentTroubleshootingEvent
description: Список свойств и связей объектов enrollmentTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ca7bcd80a115d183179b3e2c041469d19b98f14
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537708"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="6247a-103">Список объектов enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="6247a-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="6247a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6247a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6247a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6247a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6247a-106">Список свойств и связей объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="6247a-106">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6247a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6247a-107">Prerequisites</span></span>
<span data-ttu-id="6247a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6247a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6247a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6247a-110">Permission type</span></span>|<span data-ttu-id="6247a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6247a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6247a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6247a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6247a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6247a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6247a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6247a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6247a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6247a-115">Not supported.</span></span>|
|<span data-ttu-id="6247a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6247a-116">Application</span></span>|<span data-ttu-id="6247a-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6247a-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6247a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6247a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="6247a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6247a-119">Request headers</span></span>
|<span data-ttu-id="6247a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6247a-120">Header</span></span>|<span data-ttu-id="6247a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6247a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6247a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6247a-122">Authorization</span></span>|<span data-ttu-id="6247a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6247a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6247a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6247a-124">Accept</span></span>|<span data-ttu-id="6247a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6247a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6247a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6247a-126">Request body</span></span>
<span data-ttu-id="6247a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6247a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6247a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6247a-128">Response</span></span>
<span data-ttu-id="6247a-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6247a-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6247a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6247a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6247a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6247a-131">Request</span></span>
<span data-ttu-id="6247a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6247a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="6247a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6247a-133">Response</span></span>
<span data-ttu-id="6247a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6247a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






