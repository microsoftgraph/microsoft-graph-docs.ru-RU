---
title: Список объектов enrollmentTroubleshootingEvent
description: Список свойств и связей объектов enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2d98aa5e411fba91ec2fd9d4112a23483758f42
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882644"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="670a5-103">Список объектов enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="670a5-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="670a5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="670a5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="670a5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="670a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="670a5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="670a5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="670a5-107">Список свойств и связей объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="670a5-107">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="670a5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="670a5-108">Prerequisites</span></span>
<span data-ttu-id="670a5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="670a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="670a5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="670a5-111">Permission type</span></span>|<span data-ttu-id="670a5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="670a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="670a5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="670a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="670a5-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="670a5-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="670a5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="670a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="670a5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="670a5-116">Not supported.</span></span>|
|<span data-ttu-id="670a5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="670a5-117">Application</span></span>|<span data-ttu-id="670a5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="670a5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="670a5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="670a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="670a5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="670a5-120">Request headers</span></span>
|<span data-ttu-id="670a5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="670a5-121">Header</span></span>|<span data-ttu-id="670a5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="670a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="670a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="670a5-123">Authorization</span></span>|<span data-ttu-id="670a5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="670a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="670a5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="670a5-125">Accept</span></span>|<span data-ttu-id="670a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="670a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="670a5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="670a5-127">Request body</span></span>
<span data-ttu-id="670a5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="670a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="670a5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="670a5-129">Response</span></span>
<span data-ttu-id="670a5-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="670a5-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="670a5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="670a5-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="670a5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="670a5-132">Request</span></span>
<span data-ttu-id="670a5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="670a5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="670a5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="670a5-134">Response</span></span>
<span data-ttu-id="670a5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="670a5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





