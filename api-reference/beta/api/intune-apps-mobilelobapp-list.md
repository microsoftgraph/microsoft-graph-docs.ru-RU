---
title: Перечисление объектов mobileLobApp
description: Список свойств и связей объектов mobileLobApp.
ms.openlocfilehash: 2691bd626e57a68774efb0be0434e1223d479588
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081893"
---
# <a name="list-mobilelobapps"></a><span data-ttu-id="bdacf-103">Перечисление объектов mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="bdacf-103">List mobileLobApps</span></span>

> <span data-ttu-id="bdacf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bdacf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdacf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdacf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdacf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bdacf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdacf-107">Список свойств и связей объектов [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bdacf-107">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bdacf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bdacf-108">Prerequisites</span></span>
<span data-ttu-id="bdacf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdacf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdacf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdacf-111">Permission type</span></span>|<span data-ttu-id="bdacf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdacf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdacf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdacf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bdacf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdacf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bdacf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdacf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdacf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdacf-116">Not supported.</span></span>|
|<span data-ttu-id="bdacf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdacf-117">Application</span></span>|<span data-ttu-id="bdacf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdacf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdacf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdacf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bdacf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdacf-120">Request headers</span></span>
|<span data-ttu-id="bdacf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdacf-121">Header</span></span>|<span data-ttu-id="bdacf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bdacf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdacf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdacf-123">Authorization</span></span>|<span data-ttu-id="bdacf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bdacf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdacf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bdacf-125">Accept</span></span>|<span data-ttu-id="bdacf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bdacf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdacf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdacf-127">Request body</span></span>
<span data-ttu-id="bdacf-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bdacf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdacf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdacf-129">Response</span></span>
<span data-ttu-id="bdacf-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileLobApp](../resources/intune-apps-mobilelobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdacf-130">If successful, this method returns a `200 OK` response code and a collection of [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdacf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bdacf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="bdacf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdacf-132">Request</span></span>
<span data-ttu-id="bdacf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdacf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="bdacf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdacf-134">Response</span></span>
<span data-ttu-id="bdacf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="bdacf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1009

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileLobApp",
      "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4
    }
  ]
}
```





