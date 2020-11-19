---
title: Перечисление объектов localizedNotificationMessage
description: Список свойств и связей объектов localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cbe485cfcb1a461243044d225ab7762a83e811f5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49262590"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="903f6-103">Перечисление объектов localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="903f6-103">List localizedNotificationMessages</span></span>

<span data-ttu-id="903f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="903f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="903f6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="903f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="903f6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="903f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="903f6-107">Список свойств и связей объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="903f6-107">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="903f6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="903f6-108">Prerequisites</span></span>
<span data-ttu-id="903f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="903f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="903f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="903f6-111">Permission type</span></span>|<span data-ttu-id="903f6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="903f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="903f6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="903f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="903f6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="903f6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="903f6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="903f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="903f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="903f6-116">Not supported.</span></span>|
|<span data-ttu-id="903f6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="903f6-117">Application</span></span>|<span data-ttu-id="903f6-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="903f6-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="903f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="903f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="903f6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="903f6-120">Request headers</span></span>
|<span data-ttu-id="903f6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="903f6-121">Header</span></span>|<span data-ttu-id="903f6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="903f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="903f6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="903f6-123">Authorization</span></span>|<span data-ttu-id="903f6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="903f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="903f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="903f6-125">Accept</span></span>|<span data-ttu-id="903f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="903f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="903f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="903f6-127">Request body</span></span>
<span data-ttu-id="903f6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="903f6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="903f6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="903f6-129">Response</span></span>
<span data-ttu-id="903f6-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="903f6-130">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="903f6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="903f6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="903f6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="903f6-132">Request</span></span>
<span data-ttu-id="903f6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="903f6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="903f6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="903f6-134">Response</span></span>
<span data-ttu-id="903f6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="903f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




