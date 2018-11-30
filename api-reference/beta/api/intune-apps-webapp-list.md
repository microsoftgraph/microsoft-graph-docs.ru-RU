---
title: Перечисление объектов webApp
description: Список свойств и связей объектов webApp.
ms.openlocfilehash: 1114b2086ab1a1170eb49b67e8b38366d53db93b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081872"
---
# <a name="list-webapps"></a><span data-ttu-id="8d0de-103">Перечисление объектов webApp</span><span class="sxs-lookup"><span data-stu-id="8d0de-103">List webApps</span></span>

> <span data-ttu-id="8d0de-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8d0de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d0de-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d0de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d0de-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8d0de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d0de-107">Список свойств и связей объектов [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d0de-107">List properties and relationships of the [webApp](../resources/intune-apps-webapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d0de-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8d0de-108">Prerequisites</span></span>
<span data-ttu-id="8d0de-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d0de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d0de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d0de-111">Permission type</span></span>|<span data-ttu-id="8d0de-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d0de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d0de-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d0de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d0de-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d0de-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8d0de-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d0de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d0de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d0de-116">Not supported.</span></span>|
|<span data-ttu-id="8d0de-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d0de-117">Application</span></span>|<span data-ttu-id="8d0de-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d0de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d0de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d0de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8d0de-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d0de-120">Request headers</span></span>
|<span data-ttu-id="8d0de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d0de-121">Header</span></span>|<span data-ttu-id="8d0de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8d0de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d0de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d0de-123">Authorization</span></span>|<span data-ttu-id="8d0de-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8d0de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d0de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d0de-125">Accept</span></span>|<span data-ttu-id="8d0de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d0de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d0de-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d0de-127">Request body</span></span>
<span data-ttu-id="8d0de-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d0de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d0de-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d0de-129">Response</span></span>
<span data-ttu-id="8d0de-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [webApp](../resources/intune-apps-webapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d0de-130">If successful, this method returns a `200 OK` response code and a collection of [webApp](../resources/intune-apps-webapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d0de-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8d0de-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d0de-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d0de-132">Request</span></span>
<span data-ttu-id="8d0de-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d0de-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="8d0de-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d0de-134">Response</span></span>
<span data-ttu-id="8d0de-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8d0de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 960

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.webApp",
      "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "appUrl": "https://example.com/appUrl/",
      "useManagedBrowser": true
    }
  ]
}
```





