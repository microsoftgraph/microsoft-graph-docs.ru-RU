---
title: Перечисление объектов localizedNotificationMessage
description: Список свойств и связей объектов localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ac56d692f0c9e4cd4e24a8ebb511d5dfba0ed7ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823613"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="387d6-103">Перечисление объектов localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="387d6-103">List localizedNotificationMessages</span></span>

> <span data-ttu-id="387d6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="387d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="387d6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="387d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="387d6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="387d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="387d6-107">Список свойств и связей объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="387d6-107">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="387d6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="387d6-108">Prerequisites</span></span>
<span data-ttu-id="387d6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="387d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="387d6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="387d6-111">Permission type</span></span>|<span data-ttu-id="387d6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="387d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="387d6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="387d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="387d6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="387d6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="387d6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="387d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="387d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="387d6-116">Not supported.</span></span>|
|<span data-ttu-id="387d6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="387d6-117">Application</span></span>|<span data-ttu-id="387d6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="387d6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="387d6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="387d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="387d6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="387d6-120">Request headers</span></span>
|<span data-ttu-id="387d6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="387d6-121">Header</span></span>|<span data-ttu-id="387d6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="387d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="387d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="387d6-123">Authorization</span></span>|<span data-ttu-id="387d6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="387d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="387d6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="387d6-125">Accept</span></span>|<span data-ttu-id="387d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="387d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="387d6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="387d6-127">Request body</span></span>
<span data-ttu-id="387d6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="387d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="387d6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="387d6-129">Response</span></span>
<span data-ttu-id="387d6-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="387d6-130">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="387d6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="387d6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="387d6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="387d6-132">Request</span></span>
<span data-ttu-id="387d6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="387d6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="387d6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="387d6-134">Response</span></span>
<span data-ttu-id="387d6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="387d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





