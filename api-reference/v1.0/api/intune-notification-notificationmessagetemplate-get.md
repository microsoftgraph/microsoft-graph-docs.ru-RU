---
title: Get notificationMessageTemplate
description: Чтение свойств и связей объекта notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5b8eaf9b44306c209e688eabb2edc3d8fc39d025
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931400"
---
# <a name="get-notificationmessagetemplate"></a><span data-ttu-id="fd254-103">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="fd254-103">Get notificationMessageTemplate</span></span>

> <span data-ttu-id="fd254-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fd254-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd254-105">Чтение свойств и связей объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="fd254-105">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd254-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fd254-106">Prerequisites</span></span>
<span data-ttu-id="fd254-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd254-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd254-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd254-109">Permission type</span></span>|<span data-ttu-id="fd254-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd254-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd254-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd254-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fd254-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd254-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fd254-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd254-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd254-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd254-114">Not supported.</span></span>|
|<span data-ttu-id="fd254-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd254-115">Application</span></span>|<span data-ttu-id="fd254-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd254-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd254-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd254-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd254-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fd254-118">Optional query parameters</span></span>
<span data-ttu-id="fd254-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fd254-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fd254-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd254-120">Request headers</span></span>
|<span data-ttu-id="fd254-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd254-121">Header</span></span>|<span data-ttu-id="fd254-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fd254-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd254-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd254-123">Authorization</span></span>|<span data-ttu-id="fd254-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fd254-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd254-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fd254-125">Accept</span></span>|<span data-ttu-id="fd254-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd254-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd254-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd254-127">Request body</span></span>
<span data-ttu-id="fd254-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd254-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd254-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd254-129">Response</span></span>
<span data-ttu-id="fd254-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fd254-130">If successful, this method returns a `200 OK` response code and [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd254-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fd254-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd254-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd254-132">Request</span></span>
<span data-ttu-id="fd254-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd254-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

### <a name="response"></a><span data-ttu-id="fd254-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd254-134">Response</span></span>
<span data-ttu-id="fd254-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fd254-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": {
    "@odata.type": "#microsoft.graph.notificationMessageTemplate",
    "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "defaultLocale": "Default Locale value",
    "brandingOptions": "includeCompanyLogo"
  }
}
```



