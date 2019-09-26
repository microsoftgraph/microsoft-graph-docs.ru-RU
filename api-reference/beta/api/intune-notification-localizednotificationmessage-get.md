---
title: Получение объекта localizedNotificationMessage
description: Чтение свойств и связей объекта localizedNotificationMessage.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91bb7b4d6c93b8a35f5cd38f2a4a263f3a9990f2
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191171"
---
# <a name="get-localizednotificationmessage"></a><span data-ttu-id="0b6ad-103">Получение объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="0b6ad-103">Get localizedNotificationMessage</span></span>

> <span data-ttu-id="0b6ad-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b6ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b6ad-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b6ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b6ad-106">Чтение свойств и связей объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="0b6ad-106">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b6ad-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0b6ad-107">Prerequisites</span></span>
<span data-ttu-id="0b6ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b6ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b6ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b6ad-110">Permission type</span></span>|<span data-ttu-id="0b6ad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b6ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b6ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b6ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b6ad-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b6ad-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0b6ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b6ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b6ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b6ad-115">Not supported.</span></span>|
|<span data-ttu-id="0b6ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b6ad-116">Application</span></span>|<span data-ttu-id="0b6ad-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b6ad-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b6ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b6ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b6ad-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b6ad-119">Optional query parameters</span></span>
<span data-ttu-id="0b6ad-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0b6ad-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b6ad-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b6ad-121">Request headers</span></span>
|<span data-ttu-id="0b6ad-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b6ad-122">Header</span></span>|<span data-ttu-id="0b6ad-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0b6ad-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b6ad-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b6ad-124">Authorization</span></span>|<span data-ttu-id="0b6ad-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b6ad-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b6ad-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0b6ad-126">Accept</span></span>|<span data-ttu-id="0b6ad-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0b6ad-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b6ad-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b6ad-128">Request body</span></span>
<span data-ttu-id="0b6ad-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b6ad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b6ad-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b6ad-130">Response</span></span>
<span data-ttu-id="0b6ad-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b6ad-131">If successful, this method returns a `200 OK` response code and [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b6ad-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0b6ad-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b6ad-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b6ad-133">Request</span></span>
<span data-ttu-id="0b6ad-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b6ad-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="0b6ad-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b6ad-135">Response</span></span>
<span data-ttu-id="0b6ad-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b6ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




