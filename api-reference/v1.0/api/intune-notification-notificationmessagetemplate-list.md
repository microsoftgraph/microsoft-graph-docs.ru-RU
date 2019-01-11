---
title: Перечисление объектов notificationMessageTemplate
description: Список свойств и связей объектов notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1d47e3d85e0cf50d66b7587601204230074e9675
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805833"
---
# <a name="list-notificationmessagetemplates"></a><span data-ttu-id="2b718-103">Перечисление объектов notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="2b718-103">List notificationMessageTemplates</span></span>

> <span data-ttu-id="2b718-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2b718-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b718-105">Список свойств и связей объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="2b718-105">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b718-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2b718-106">Prerequisites</span></span>
<span data-ttu-id="2b718-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b718-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b718-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b718-109">Permission type</span></span>|<span data-ttu-id="2b718-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b718-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b718-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b718-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b718-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b718-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2b718-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b718-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b718-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b718-114">Not supported.</span></span>|
|<span data-ttu-id="2b718-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b718-115">Application</span></span>|<span data-ttu-id="2b718-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b718-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b718-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b718-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="2b718-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b718-118">Request headers</span></span>
|<span data-ttu-id="2b718-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b718-119">Header</span></span>|<span data-ttu-id="2b718-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2b718-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b718-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b718-121">Authorization</span></span>|<span data-ttu-id="2b718-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2b718-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b718-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2b718-123">Accept</span></span>|<span data-ttu-id="2b718-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2b718-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b718-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b718-125">Request body</span></span>
<span data-ttu-id="2b718-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b718-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b718-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b718-127">Response</span></span>
<span data-ttu-id="2b718-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b718-128">If successful, this method returns a `200 OK` response code and a collection of [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b718-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2b718-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b718-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b718-130">Request</span></span>
<span data-ttu-id="2b718-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b718-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
```

### <a name="response"></a><span data-ttu-id="2b718-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b718-132">Response</span></span>
<span data-ttu-id="2b718-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2b718-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



