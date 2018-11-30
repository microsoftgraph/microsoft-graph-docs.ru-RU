---
title: Перечисление объектов notificationMessageTemplate
description: Список свойств и связей объектов notificationMessageTemplate.
ms.openlocfilehash: 4a1ab9cc331eb08473f61c5ae247e311f3b16afa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025002"
---
# <a name="list-notificationmessagetemplates"></a><span data-ttu-id="761a8-103">Перечисление объектов notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="761a8-103">List notificationMessageTemplates</span></span>

> <span data-ttu-id="761a8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="761a8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="761a8-105">Список свойств и связей объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="761a8-105">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="761a8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="761a8-106">Prerequisites</span></span>
<span data-ttu-id="761a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="761a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="761a8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="761a8-109">Permission type</span></span>|<span data-ttu-id="761a8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="761a8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="761a8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="761a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="761a8-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="761a8-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="761a8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="761a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="761a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="761a8-114">Not supported.</span></span>|
|<span data-ttu-id="761a8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="761a8-115">Application</span></span>|<span data-ttu-id="761a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="761a8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="761a8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="761a8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="761a8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="761a8-118">Request headers</span></span>
|<span data-ttu-id="761a8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="761a8-119">Header</span></span>|<span data-ttu-id="761a8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="761a8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="761a8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="761a8-121">Authorization</span></span>|<span data-ttu-id="761a8-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="761a8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="761a8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="761a8-123">Accept</span></span>|<span data-ttu-id="761a8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="761a8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="761a8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="761a8-125">Request body</span></span>
<span data-ttu-id="761a8-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="761a8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="761a8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="761a8-127">Response</span></span>
<span data-ttu-id="761a8-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="761a8-128">If successful, this method returns a `200 OK` response code and a collection of [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="761a8-129">Пример</span><span class="sxs-lookup"><span data-stu-id="761a8-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="761a8-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="761a8-130">Request</span></span>
<span data-ttu-id="761a8-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="761a8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
```

### <a name="response"></a><span data-ttu-id="761a8-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="761a8-132">Response</span></span>
<span data-ttu-id="761a8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="761a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 367

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.notificationMessageTemplate",
      "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "defaultLocale": "Default Locale value",
      "brandingOptions": "includeCompanyLogo"
    }
  ]
}
```



