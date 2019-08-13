---
title: Get enrollmentTroubleshootingEvent
description: Чтение свойств и связей объекта enrollmentTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a78f0a1e19351e958f020e7160e4445f3e495188
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347327"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="e003e-103">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e003e-103">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="e003e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e003e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e003e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e003e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e003e-106">Чтение свойств и связей объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e003e-106">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e003e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e003e-107">Prerequisites</span></span>
<span data-ttu-id="e003e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e003e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e003e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e003e-110">Permission type</span></span>|<span data-ttu-id="e003e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e003e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e003e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e003e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e003e-113">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="e003e-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="e003e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e003e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e003e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e003e-115">Not supported.</span></span>|
|<span data-ttu-id="e003e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e003e-116">Application</span></span>|<span data-ttu-id="e003e-117">\* \* TODO: определение областей поддержка apponly \* \*</span><span class="sxs-lookup"><span data-stu-id="e003e-117">\*\*TODO: Determine AppOnly scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="e003e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e003e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e003e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e003e-119">Optional query parameters</span></span>
<span data-ttu-id="e003e-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e003e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e003e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e003e-121">Request headers</span></span>
|<span data-ttu-id="e003e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e003e-122">Header</span></span>|<span data-ttu-id="e003e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e003e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e003e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e003e-124">Authorization</span></span>|<span data-ttu-id="e003e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e003e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e003e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e003e-126">Accept</span></span>|<span data-ttu-id="e003e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e003e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e003e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e003e-128">Request body</span></span>
<span data-ttu-id="e003e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e003e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e003e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e003e-130">Response</span></span>
<span data-ttu-id="e003e-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e003e-131">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e003e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e003e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e003e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e003e-133">Request</span></span>
<span data-ttu-id="e003e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e003e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="e003e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e003e-135">Response</span></span>
<span data-ttu-id="e003e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e003e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






