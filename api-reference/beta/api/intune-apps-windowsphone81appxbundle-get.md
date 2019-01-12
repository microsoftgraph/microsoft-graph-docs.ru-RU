---
title: Получение windowsPhone81AppXBundle
description: Чтение свойства и связи объекта windowsPhone81AppXBundle.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0dd3d01f5497850d91c396c0836b7ce07eb901f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978916"
---
# <a name="get-windowsphone81appxbundle"></a><span data-ttu-id="23b69-103">Получение windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="23b69-103">Get windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="23b69-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23b69-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23b69-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23b69-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23b69-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="23b69-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23b69-107">Чтение свойства и связи объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="23b69-107">Read properties and relationships of the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23b69-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="23b69-108">Prerequisites</span></span>
<span data-ttu-id="23b69-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23b69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23b69-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23b69-111">Permission type</span></span>|<span data-ttu-id="23b69-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="23b69-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23b69-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23b69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23b69-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="23b69-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="23b69-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23b69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23b69-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23b69-116">Not supported.</span></span>|
|<span data-ttu-id="23b69-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23b69-117">Application</span></span>|<span data-ttu-id="23b69-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23b69-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23b69-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23b69-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23b69-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23b69-120">Optional query parameters</span></span>
<span data-ttu-id="23b69-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="23b69-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="23b69-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23b69-122">Request headers</span></span>
|<span data-ttu-id="23b69-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23b69-123">Header</span></span>|<span data-ttu-id="23b69-124">Значение</span><span class="sxs-lookup"><span data-stu-id="23b69-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23b69-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="23b69-125">Authorization</span></span>|<span data-ttu-id="23b69-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="23b69-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23b69-127">Accept</span><span class="sxs-lookup"><span data-stu-id="23b69-127">Accept</span></span>|<span data-ttu-id="23b69-128">application/json</span><span class="sxs-lookup"><span data-stu-id="23b69-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23b69-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="23b69-129">Request body</span></span>
<span data-ttu-id="23b69-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23b69-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23b69-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="23b69-131">Response</span></span>
<span data-ttu-id="23b69-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="23b69-132">If successful, this method returns a `200 OK` response code and [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23b69-133">Пример</span><span class="sxs-lookup"><span data-stu-id="23b69-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="23b69-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b69-134">Request</span></span>
<span data-ttu-id="23b69-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b69-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="23b69-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="23b69-136">Response</span></span>
<span data-ttu-id="23b69-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="23b69-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2412

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
    "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
    "phoneProductIdentifier": "Phone Product Identifier value",
    "phonePublisherId": "Phone Publisher Id value",
    "identityVersion": "Identity Version value",
    "appXPackageInformationList": [
      {
        "@odata.type": "microsoft.graph.windowsPackageInformation",
        "applicableArchitecture": "x86",
        "displayName": "Display Name value",
        "identityName": "Identity Name value",
        "identityPublisher": "Identity Publisher value",
        "identityResourceIdentifier": "Identity Resource Identifier value",
        "identityVersion": "Identity Version value",
        "minimumSupportedOperatingSystem": {
          "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
          "v8_0": true,
          "v8_1": true,
          "v10_0": true,
          "v10_1607": true,
          "v10_1703": true,
          "v10_1709": true,
          "v10_1803": true
        }
      }
    ]
  }
}
```





