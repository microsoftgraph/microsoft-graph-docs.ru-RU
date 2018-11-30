---
title: Get enrollmentTroubleshootingEvent
description: Чтение свойств и связей объекта enrollmentTroubleshootingEvent.
ms.openlocfilehash: a576568142b6365438d19c197b9ca192c52204f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076401"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="751d0-103">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="751d0-103">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="751d0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="751d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="751d0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="751d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="751d0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="751d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="751d0-107">Чтение свойств и связей объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="751d0-107">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="751d0-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="751d0-108">Prerequisites</span></span>
<span data-ttu-id="751d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="751d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="751d0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="751d0-111">Permission type</span></span>|<span data-ttu-id="751d0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="751d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="751d0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="751d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="751d0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="751d0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="751d0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="751d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="751d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="751d0-116">Not supported.</span></span>|
|<span data-ttu-id="751d0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="751d0-117">Application</span></span>|<span data-ttu-id="751d0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="751d0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="751d0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="751d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="751d0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="751d0-120">Optional query parameters</span></span>
<span data-ttu-id="751d0-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="751d0-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="751d0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="751d0-122">Request headers</span></span>
|<span data-ttu-id="751d0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="751d0-123">Header</span></span>|<span data-ttu-id="751d0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="751d0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="751d0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="751d0-125">Authorization</span></span>|<span data-ttu-id="751d0-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="751d0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="751d0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="751d0-127">Accept</span></span>|<span data-ttu-id="751d0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="751d0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="751d0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="751d0-129">Request body</span></span>
<span data-ttu-id="751d0-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="751d0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="751d0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="751d0-131">Response</span></span>
<span data-ttu-id="751d0-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="751d0-132">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="751d0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="751d0-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="751d0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="751d0-134">Request</span></span>
<span data-ttu-id="751d0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="751d0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="751d0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="751d0-136">Response</span></span>
<span data-ttu-id="751d0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="751d0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "value": {
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
}
```





