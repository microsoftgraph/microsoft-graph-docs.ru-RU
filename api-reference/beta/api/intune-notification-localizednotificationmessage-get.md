---
title: Получение объекта localizedNotificationMessage
description: Чтение свойств и связей объекта localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ef1e5ad26bc8d2541b9506b572747d3e9314904
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980330"
---
# <a name="get-localizednotificationmessage"></a><span data-ttu-id="92a3f-103">Получение объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="92a3f-103">Get localizedNotificationMessage</span></span>

> <span data-ttu-id="92a3f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="92a3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92a3f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92a3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92a3f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="92a3f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92a3f-107">Чтение свойств и связей объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="92a3f-107">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92a3f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="92a3f-108">Prerequisites</span></span>
<span data-ttu-id="92a3f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92a3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92a3f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92a3f-111">Permission type</span></span>|<span data-ttu-id="92a3f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92a3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92a3f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92a3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92a3f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="92a3f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="92a3f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92a3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92a3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92a3f-116">Not supported.</span></span>|
|<span data-ttu-id="92a3f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92a3f-117">Application</span></span>|<span data-ttu-id="92a3f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92a3f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92a3f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92a3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92a3f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92a3f-120">Optional query parameters</span></span>
<span data-ttu-id="92a3f-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="92a3f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="92a3f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92a3f-122">Request headers</span></span>
|<span data-ttu-id="92a3f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92a3f-123">Header</span></span>|<span data-ttu-id="92a3f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="92a3f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92a3f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="92a3f-125">Authorization</span></span>|<span data-ttu-id="92a3f-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="92a3f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92a3f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="92a3f-127">Accept</span></span>|<span data-ttu-id="92a3f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="92a3f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92a3f-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="92a3f-129">Request body</span></span>
<span data-ttu-id="92a3f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92a3f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92a3f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="92a3f-131">Response</span></span>
<span data-ttu-id="92a3f-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="92a3f-132">If successful, this method returns a `200 OK` response code and [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92a3f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="92a3f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="92a3f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="92a3f-134">Request</span></span>
<span data-ttu-id="92a3f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92a3f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="92a3f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="92a3f-136">Response</span></span>
<span data-ttu-id="92a3f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="92a3f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.localizedNotificationMessage",
    "id": "7a777708-7708-7a77-0877-777a0877777a",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "locale": "Locale value",
    "subject": "Subject value",
    "messageTemplate": "Message Template value",
    "isDefault": true
  }
}
```





