---
title: Получение windowsPhone81AppXBundle
description: Чтение свойства и связи объекта windowsPhone81AppXBundle.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 56afdac0636288b35445341320e90b8ac14b1698
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425437"
---
# <a name="get-windowsphone81appxbundle"></a><span data-ttu-id="506b4-103">Получение windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="506b4-103">Get windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="506b4-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="506b4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="506b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="506b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="506b4-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="506b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="506b4-107">Чтение свойства и связи объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="506b4-107">Read properties and relationships of the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="506b4-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="506b4-108">Prerequisites</span></span>
<span data-ttu-id="506b4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="506b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="506b4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="506b4-111">Permission type</span></span>|<span data-ttu-id="506b4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="506b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="506b4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="506b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="506b4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="506b4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="506b4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="506b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="506b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="506b4-116">Not supported.</span></span>|
|<span data-ttu-id="506b4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="506b4-117">Application</span></span>|<span data-ttu-id="506b4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="506b4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="506b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="506b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="506b4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="506b4-120">Optional query parameters</span></span>
<span data-ttu-id="506b4-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="506b4-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="506b4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="506b4-122">Request headers</span></span>
|<span data-ttu-id="506b4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="506b4-123">Header</span></span>|<span data-ttu-id="506b4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="506b4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="506b4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="506b4-125">Authorization</span></span>|<span data-ttu-id="506b4-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="506b4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="506b4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="506b4-127">Accept</span></span>|<span data-ttu-id="506b4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="506b4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="506b4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="506b4-129">Request body</span></span>
<span data-ttu-id="506b4-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="506b4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="506b4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="506b4-131">Response</span></span>
<span data-ttu-id="506b4-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="506b4-132">If successful, this method returns a `200 OK` response code and [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="506b4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="506b4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="506b4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="506b4-134">Request</span></span>
<span data-ttu-id="506b4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="506b4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="506b4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="506b4-136">Response</span></span>
<span data-ttu-id="506b4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="506b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2505

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
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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




