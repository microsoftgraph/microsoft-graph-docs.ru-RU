---
title: Перечисление объектов localizedNotificationMessage
description: Список свойств и связей объектов localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ffccd0f496c8096e06371f14cdadf7a1a12e08a5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963684"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="5b5bf-103">Перечисление объектов localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="5b5bf-103">List localizedNotificationMessages</span></span>

> <span data-ttu-id="5b5bf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5b5bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b5bf-105">Список свойств и связей объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="5b5bf-105">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b5bf-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5b5bf-106">Prerequisites</span></span>
<span data-ttu-id="5b5bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b5bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b5bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b5bf-109">Permission type</span></span>|<span data-ttu-id="5b5bf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b5bf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b5bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b5bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b5bf-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b5bf-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5b5bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b5bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b5bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b5bf-114">Not supported.</span></span>|
|<span data-ttu-id="5b5bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b5bf-115">Application</span></span>|<span data-ttu-id="5b5bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b5bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b5bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b5bf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="5b5bf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b5bf-118">Request headers</span></span>
|<span data-ttu-id="5b5bf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b5bf-119">Header</span></span>|<span data-ttu-id="5b5bf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5b5bf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b5bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b5bf-121">Authorization</span></span>|<span data-ttu-id="5b5bf-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5b5bf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b5bf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5b5bf-123">Accept</span></span>|<span data-ttu-id="5b5bf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5b5bf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b5bf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b5bf-125">Request body</span></span>
<span data-ttu-id="5b5bf-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b5bf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b5bf-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b5bf-127">Response</span></span>
<span data-ttu-id="5b5bf-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5b5bf-128">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b5bf-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5b5bf-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b5bf-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b5bf-130">Request</span></span>
<span data-ttu-id="5b5bf-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b5bf-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="5b5bf-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b5bf-132">Response</span></span>
<span data-ttu-id="5b5bf-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5b5bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.localizedNotificationMessage",
      "id": "7a777708-7708-7a77-0877-777a0877777a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "locale": "Locale value",
      "subject": "Subject value",
      "messageTemplate": "Message Template value",
      "isDefault": true
    }
  ]
}
```



