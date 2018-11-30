---
title: Список объектов enrollmentTroubleshootingEvent
description: Список свойств и связей объектов enrollmentTroubleshootingEvent.
ms.openlocfilehash: 63ba4591e2eb77d85143462bc84f532f25f8b0b3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027444"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="661f5-103">Список объектов enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="661f5-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="661f5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="661f5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="661f5-105">Список свойств и связей объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="661f5-105">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="661f5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="661f5-106">Prerequisites</span></span>
<span data-ttu-id="661f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="661f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="661f5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="661f5-109">Permission type</span></span>|<span data-ttu-id="661f5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="661f5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="661f5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="661f5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="661f5-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="661f5-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="661f5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="661f5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="661f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="661f5-114">Not supported.</span></span>|
|<span data-ttu-id="661f5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="661f5-115">Application</span></span>|<span data-ttu-id="661f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="661f5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="661f5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="661f5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="661f5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="661f5-118">Request headers</span></span>
|<span data-ttu-id="661f5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="661f5-119">Header</span></span>|<span data-ttu-id="661f5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="661f5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="661f5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="661f5-121">Authorization</span></span>|<span data-ttu-id="661f5-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="661f5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="661f5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="661f5-123">Accept</span></span>|<span data-ttu-id="661f5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="661f5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="661f5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="661f5-125">Request body</span></span>
<span data-ttu-id="661f5-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="661f5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="661f5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="661f5-127">Response</span></span>
<span data-ttu-id="661f5-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="661f5-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="661f5-129">Пример</span><span class="sxs-lookup"><span data-stu-id="661f5-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="661f5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="661f5-130">Request</span></span>
<span data-ttu-id="661f5-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="661f5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="661f5-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="661f5-132">Response</span></span>
<span data-ttu-id="661f5-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="661f5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
      "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value",
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



