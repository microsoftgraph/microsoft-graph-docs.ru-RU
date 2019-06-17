---
title: Перечисление объектов localizedNotificationMessage
description: Список свойств и связей объектов localizedNotificationMessage.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1373487b8884c8483073b35f874b70918c4bd97
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34957866"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="8b645-103">Перечисление объектов localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="8b645-103">List localizedNotificationMessages</span></span>

> <span data-ttu-id="8b645-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b645-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b645-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b645-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b645-106">Список свойств и связей объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="8b645-106">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b645-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8b645-107">Prerequisites</span></span>
<span data-ttu-id="8b645-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b645-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b645-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b645-110">Permission type</span></span>|<span data-ttu-id="8b645-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b645-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b645-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b645-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b645-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b645-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8b645-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b645-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b645-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b645-115">Not supported.</span></span>|
|<span data-ttu-id="8b645-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b645-116">Application</span></span>|<span data-ttu-id="8b645-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b645-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b645-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b645-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="8b645-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b645-119">Request headers</span></span>
|<span data-ttu-id="8b645-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b645-120">Header</span></span>|<span data-ttu-id="8b645-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8b645-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b645-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b645-122">Authorization</span></span>|<span data-ttu-id="8b645-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b645-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b645-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8b645-124">Accept</span></span>|<span data-ttu-id="8b645-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b645-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b645-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b645-126">Request body</span></span>
<span data-ttu-id="8b645-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b645-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b645-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b645-128">Response</span></span>
<span data-ttu-id="8b645-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b645-129">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b645-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8b645-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b645-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b645-131">Request</span></span>
<span data-ttu-id="8b645-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b645-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="8b645-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b645-133">Response</span></span>
<span data-ttu-id="8b645-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b645-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





