---
title: Получение mobileAppTroubleshootingEvent
description: Чтение свойства и связи объекта mobileAppTroubleshootingEvent.
ms.openlocfilehash: f70bdfb30317d1fe1033516b64efe8e046212dd7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079076"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="3f769-103">Получение mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3f769-103">Get mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="3f769-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3f769-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f769-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f769-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f769-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3f769-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f769-107">Чтение свойства и связи объекта [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="3f769-107">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3f769-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3f769-108">Prerequisites</span></span>
<span data-ttu-id="3f769-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f769-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f769-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f769-111">Permission type</span></span>|<span data-ttu-id="3f769-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f769-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f769-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f769-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f769-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f769-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3f769-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f769-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f769-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f769-116">Not supported.</span></span>|
|<span data-ttu-id="3f769-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f769-117">Application</span></span>|<span data-ttu-id="3f769-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f769-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f769-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f769-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3f769-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3f769-120">Optional query parameters</span></span>
<span data-ttu-id="3f769-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3f769-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3f769-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f769-122">Request headers</span></span>
|<span data-ttu-id="3f769-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f769-123">Header</span></span>|<span data-ttu-id="3f769-124">Значение</span><span class="sxs-lookup"><span data-stu-id="3f769-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f769-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f769-125">Authorization</span></span>|<span data-ttu-id="3f769-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3f769-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f769-127">Accept</span><span class="sxs-lookup"><span data-stu-id="3f769-127">Accept</span></span>|<span data-ttu-id="3f769-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3f769-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f769-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f769-129">Request body</span></span>
<span data-ttu-id="3f769-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f769-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f769-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f769-131">Response</span></span>
<span data-ttu-id="3f769-132">Успешно завершена, этот метод возвращает `200 OK` объект [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3f769-132">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f769-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3f769-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="3f769-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f769-134">Request</span></span>
<span data-ttu-id="3f769-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f769-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="3f769-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f769-136">Response</span></span>
<span data-ttu-id="3f769-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3f769-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 583

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
    "id": "77943c10-3c10-7794-103c-9477103c9477",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value",
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "userId": "User Id value",
    "applicationId": "Application Id value",
    "history": [
      {
        "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
        "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
      }
    ]
  }
}
```





