---
title: Получение windowsAppX
description: Чтение свойства и связи объекта windowsAppX.
ms.openlocfilehash: 53f42d37d45c42f6b4f65637a7da9b9f5a885826
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081847"
---
# <a name="get-windowsappx"></a><span data-ttu-id="0d170-103">Получение windowsAppX</span><span class="sxs-lookup"><span data-stu-id="0d170-103">Get windowsAppX</span></span>

> <span data-ttu-id="0d170-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0d170-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d170-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d170-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d170-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0d170-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d170-107">Чтение свойства и связи объекта [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="0d170-107">Read properties and relationships of the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d170-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0d170-108">Prerequisites</span></span>
<span data-ttu-id="0d170-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d170-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d170-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d170-111">Permission type</span></span>|<span data-ttu-id="0d170-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d170-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d170-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d170-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d170-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d170-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0d170-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d170-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d170-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d170-116">Not supported.</span></span>|
|<span data-ttu-id="0d170-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d170-117">Application</span></span>|<span data-ttu-id="0d170-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d170-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d170-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d170-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d170-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0d170-120">Optional query parameters</span></span>
<span data-ttu-id="0d170-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0d170-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0d170-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d170-122">Request headers</span></span>
|<span data-ttu-id="0d170-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d170-123">Header</span></span>|<span data-ttu-id="0d170-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0d170-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d170-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d170-125">Authorization</span></span>|<span data-ttu-id="0d170-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0d170-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d170-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0d170-127">Accept</span></span>|<span data-ttu-id="0d170-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0d170-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d170-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d170-129">Request body</span></span>
<span data-ttu-id="0d170-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d170-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d170-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d170-131">Response</span></span>
<span data-ttu-id="0d170-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsAppX](../resources/intune-apps-windowsappx.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0d170-132">If successful, this method returns a `200 OK` response code and [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d170-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0d170-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d170-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d170-134">Request</span></span>
<span data-ttu-id="0d170-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d170-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="0d170-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d170-136">Response</span></span>
<span data-ttu-id="0d170-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0d170-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1524

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAppX",
    "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
    "applicableArchitectures": "x86",
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
    "isBundle": true,
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true,
      "v10_1607": true,
      "v10_1703": true,
      "v10_1709": true,
      "v10_1803": true
    },
    "identityVersion": "Identity Version value"
  }
}
```





