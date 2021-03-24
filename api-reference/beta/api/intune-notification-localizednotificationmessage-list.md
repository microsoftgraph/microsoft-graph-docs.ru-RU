---
title: Перечисление объектов localizedNotificationMessage
description: Список свойств и связей объектов localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f8fa31c7a4b4fc1dbaf18c0b6351b942c709764
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125907"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="77739-103">Перечисление объектов localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="77739-103">List localizedNotificationMessages</span></span>

<span data-ttu-id="77739-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77739-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77739-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77739-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77739-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77739-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77739-107">Список свойств и связей объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="77739-107">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77739-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="77739-108">Prerequisites</span></span>
<span data-ttu-id="77739-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77739-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77739-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77739-111">Permission type</span></span>|<span data-ttu-id="77739-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77739-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77739-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77739-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77739-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77739-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="77739-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77739-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77739-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77739-116">Not supported.</span></span>|
|<span data-ttu-id="77739-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="77739-117">Application</span></span>|<span data-ttu-id="77739-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77739-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77739-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77739-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="77739-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="77739-120">Request headers</span></span>
|<span data-ttu-id="77739-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77739-121">Header</span></span>|<span data-ttu-id="77739-122">Значение</span><span class="sxs-lookup"><span data-stu-id="77739-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77739-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77739-123">Authorization</span></span>|<span data-ttu-id="77739-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77739-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77739-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77739-125">Accept</span></span>|<span data-ttu-id="77739-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77739-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77739-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77739-127">Request body</span></span>
<span data-ttu-id="77739-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77739-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77739-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="77739-129">Response</span></span>
<span data-ttu-id="77739-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="77739-130">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77739-131">Пример</span><span class="sxs-lookup"><span data-stu-id="77739-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="77739-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="77739-132">Request</span></span>
<span data-ttu-id="77739-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77739-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="77739-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="77739-134">Response</span></span>
<span data-ttu-id="77739-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77739-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




