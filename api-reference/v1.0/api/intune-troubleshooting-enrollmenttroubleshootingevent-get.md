---
title: Get enrollmentTroubleshootingEvent
description: Чтение свойств и связей объекта enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6686db8c7be23805849542b03ad93392451943d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025668"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="80254-103">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="80254-103">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="80254-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80254-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80254-105">Чтение свойств и связей объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="80254-105">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80254-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="80254-106">Prerequisites</span></span>
<span data-ttu-id="80254-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80254-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80254-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80254-109">Permission type</span></span>|<span data-ttu-id="80254-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="80254-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80254-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80254-111">Delegated (work or school account)</span></span>|<span data-ttu-id="80254-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="80254-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="80254-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80254-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80254-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80254-114">Not supported.</span></span>|
|<span data-ttu-id="80254-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80254-115">Application</span></span>|<span data-ttu-id="80254-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80254-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80254-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80254-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80254-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="80254-118">Optional query parameters</span></span>
<span data-ttu-id="80254-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="80254-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80254-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80254-120">Request headers</span></span>
|<span data-ttu-id="80254-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80254-121">Header</span></span>|<span data-ttu-id="80254-122">Значение</span><span class="sxs-lookup"><span data-stu-id="80254-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80254-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80254-123">Authorization</span></span>|<span data-ttu-id="80254-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80254-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80254-125">Accept</span><span class="sxs-lookup"><span data-stu-id="80254-125">Accept</span></span>|<span data-ttu-id="80254-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80254-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80254-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="80254-127">Request body</span></span>
<span data-ttu-id="80254-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="80254-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80254-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="80254-129">Response</span></span>
<span data-ttu-id="80254-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="80254-130">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80254-131">Пример</span><span class="sxs-lookup"><span data-stu-id="80254-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="80254-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="80254-132">Request</span></span>
<span data-ttu-id="80254-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80254-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="80254-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="80254-134">Response</span></span>
<span data-ttu-id="80254-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80254-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



