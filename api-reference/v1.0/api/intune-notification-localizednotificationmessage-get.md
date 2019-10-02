---
title: Получение объекта localizedNotificationMessage
description: Чтение свойств и связей объекта localizedNotificationMessage.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd48964616ee9353dd87f34af93f97ebd411e84b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362886"
---
# <a name="get-localizednotificationmessage"></a><span data-ttu-id="0abe2-103">Получение объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="0abe2-103">Get localizedNotificationMessage</span></span>

> <span data-ttu-id="0abe2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0abe2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0abe2-105">Чтение свойств и связей объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="0abe2-105">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0abe2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0abe2-106">Prerequisites</span></span>
<span data-ttu-id="0abe2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0abe2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0abe2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0abe2-109">Permission type</span></span>|<span data-ttu-id="0abe2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0abe2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0abe2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0abe2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0abe2-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0abe2-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0abe2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0abe2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0abe2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0abe2-114">Not supported.</span></span>|
|<span data-ttu-id="0abe2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0abe2-115">Application</span></span>|<span data-ttu-id="0abe2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0abe2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0abe2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0abe2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0abe2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0abe2-118">Optional query parameters</span></span>
<span data-ttu-id="0abe2-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0abe2-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0abe2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0abe2-120">Request headers</span></span>
|<span data-ttu-id="0abe2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0abe2-121">Header</span></span>|<span data-ttu-id="0abe2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0abe2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0abe2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0abe2-123">Authorization</span></span>|<span data-ttu-id="0abe2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0abe2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0abe2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0abe2-125">Accept</span></span>|<span data-ttu-id="0abe2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0abe2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0abe2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0abe2-127">Request body</span></span>
<span data-ttu-id="0abe2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0abe2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0abe2-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0abe2-129">Response</span></span>
<span data-ttu-id="0abe2-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0abe2-130">If successful, this method returns a `200 OK` response code and [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0abe2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0abe2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0abe2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0abe2-132">Request</span></span>
<span data-ttu-id="0abe2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0abe2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="0abe2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0abe2-134">Response</span></span>
<span data-ttu-id="0abe2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0abe2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




