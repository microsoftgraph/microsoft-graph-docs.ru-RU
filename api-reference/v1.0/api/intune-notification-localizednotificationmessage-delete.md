---
title: Удаление localizedNotificationMessage
description: Удаляет объект localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1a7c7e15a08460dc412492fd7f33ee54385d9760
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925198"
---
# <a name="delete-localizednotificationmessage"></a><span data-ttu-id="46ea2-103">Удаление localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="46ea2-103">Delete localizedNotificationMessage</span></span>

> <span data-ttu-id="46ea2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="46ea2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46ea2-105">Удаляет объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="46ea2-105">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46ea2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="46ea2-106">Prerequisites</span></span>
<span data-ttu-id="46ea2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46ea2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46ea2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46ea2-109">Permission type</span></span>|<span data-ttu-id="46ea2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46ea2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46ea2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46ea2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46ea2-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46ea2-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="46ea2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46ea2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46ea2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ea2-114">Not supported.</span></span>|
|<span data-ttu-id="46ea2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46ea2-115">Application</span></span>|<span data-ttu-id="46ea2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ea2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46ea2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46ea2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="46ea2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46ea2-118">Request headers</span></span>
|<span data-ttu-id="46ea2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46ea2-119">Header</span></span>|<span data-ttu-id="46ea2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="46ea2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46ea2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46ea2-121">Authorization</span></span>|<span data-ttu-id="46ea2-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="46ea2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46ea2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="46ea2-123">Accept</span></span>|<span data-ttu-id="46ea2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="46ea2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46ea2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46ea2-125">Request body</span></span>
<span data-ttu-id="46ea2-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46ea2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46ea2-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="46ea2-127">Response</span></span>
<span data-ttu-id="46ea2-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="46ea2-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="46ea2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="46ea2-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="46ea2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="46ea2-130">Request</span></span>
<span data-ttu-id="46ea2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46ea2-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="46ea2-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="46ea2-132">Response</span></span>
<span data-ttu-id="46ea2-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="46ea2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



