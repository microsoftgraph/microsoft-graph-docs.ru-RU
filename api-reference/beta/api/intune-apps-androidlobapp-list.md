---
title: Перечисление объектов androidLobApp
description: Список свойств и связей объектов androidLobApp.
author: tfitzmac
ms.openlocfilehash: 11d9640cd2fab3cfb0ccce736c6fa664b698c988
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309130"
---
# <a name="list-androidlobapps"></a><span data-ttu-id="e08a8-103">Перечисление объектов androidLobApp</span><span class="sxs-lookup"><span data-stu-id="e08a8-103">List androidLobApps</span></span>

> <span data-ttu-id="e08a8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e08a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e08a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e08a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e08a8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e08a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e08a8-107">Список свойств и связей объектов [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e08a8-107">List properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e08a8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e08a8-108">Prerequisites</span></span>
<span data-ttu-id="e08a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e08a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e08a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e08a8-111">Permission type</span></span>|<span data-ttu-id="e08a8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e08a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e08a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e08a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e08a8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e08a8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e08a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e08a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e08a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e08a8-116">Not supported.</span></span>|
|<span data-ttu-id="e08a8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e08a8-117">Application</span></span>|<span data-ttu-id="e08a8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e08a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e08a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e08a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e08a8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e08a8-120">Request headers</span></span>
|<span data-ttu-id="e08a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e08a8-121">Header</span></span>|<span data-ttu-id="e08a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e08a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e08a8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e08a8-123">Authorization</span></span>|<span data-ttu-id="e08a8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e08a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e08a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e08a8-125">Accept</span></span>|<span data-ttu-id="e08a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e08a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e08a8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e08a8-127">Request body</span></span>
<span data-ttu-id="e08a8-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e08a8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e08a8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e08a8-129">Response</span></span>
<span data-ttu-id="e08a8-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidLobApp](../resources/intune-apps-androidlobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e08a8-130">If successful, this method returns a `200 OK` response code and a collection of [androidLobApp](../resources/intune-apps-androidlobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e08a8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e08a8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e08a8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e08a8-132">Request</span></span>
<span data-ttu-id="e08a8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e08a8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="e08a8-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e08a8-134">Response</span></span>
<span data-ttu-id="e08a8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e08a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1686

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidLobApp",
      "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
      "size": 4,
      "packageId": "Package Id value",
      "identityName": "Identity Name value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
        "v4_0": true,
        "v4_0_3": true,
        "v4_1": true,
        "v4_2": true,
        "v4_3": true,
        "v4_4": true,
        "v5_0": true,
        "v5_1": true,
        "v6_0": true,
        "v7_0": true,
        "v7_1": true,
        "v8_0": true,
        "v8_1": true,
        "v9_0": true
      },
      "versionName": "Version Name value",
      "versionCode": "Version Code value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```





