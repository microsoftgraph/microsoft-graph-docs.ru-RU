---
title: Список macOSLobApps
description: Список свойств и связей объектов macOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e2aa0f46a67bc2ce212b436efe63e6997940dc0b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140513"
---
# <a name="list-macoslobapps"></a><span data-ttu-id="672d8-103">Список macOSLobApps</span><span class="sxs-lookup"><span data-stu-id="672d8-103">List macOSLobApps</span></span>

<span data-ttu-id="672d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="672d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="672d8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="672d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="672d8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="672d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="672d8-107">Список свойств и связей объектов [macOSLobApp.](../resources/intune-apps-macoslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="672d8-107">List properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="672d8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="672d8-108">Prerequisites</span></span>
<span data-ttu-id="672d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="672d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="672d8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="672d8-111">Permission type</span></span>|<span data-ttu-id="672d8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="672d8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="672d8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="672d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="672d8-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="672d8-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="672d8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="672d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="672d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="672d8-116">Not supported.</span></span>|
|<span data-ttu-id="672d8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="672d8-117">Application</span></span>|<span data-ttu-id="672d8-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="672d8-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="672d8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="672d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="672d8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="672d8-120">Request headers</span></span>
|<span data-ttu-id="672d8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="672d8-121">Header</span></span>|<span data-ttu-id="672d8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="672d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="672d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="672d8-123">Authorization</span></span>|<span data-ttu-id="672d8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="672d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="672d8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="672d8-125">Accept</span></span>|<span data-ttu-id="672d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="672d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="672d8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="672d8-127">Request body</span></span>
<span data-ttu-id="672d8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="672d8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="672d8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="672d8-129">Response</span></span>
<span data-ttu-id="672d8-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [macOSLobApp](../resources/intune-apps-macoslobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="672d8-130">If successful, this method returns a `200 OK` response code and a collection of [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="672d8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="672d8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="672d8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="672d8-132">Request</span></span>
<span data-ttu-id="672d8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="672d8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="672d8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="672d8-134">Response</span></span>
<span data-ttu-id="672d8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="672d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2147

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSLobApp",
      "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
      "dependentAppCount": 1,
      "supersedingAppCount": 3,
      "supersededAppCount": 2,
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "bundleId": "Bundle Id value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
        "v10_7": true,
        "v10_8": true,
        "v10_9": true,
        "v10_10": true,
        "v10_11": true,
        "v10_12": true,
        "v10_13": true,
        "v10_14": true,
        "v10_15": true
      },
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value",
      "childApps": [
        {
          "@odata.type": "microsoft.graph.macOSLobChildApp",
          "bundleId": "Bundle Id value",
          "buildNumber": "Build Number value",
          "versionNumber": "Version Number value"
        }
      ],
      "identityVersion": "Identity Version value",
      "md5HashChunkSize": 0,
      "md5Hash": [
        "Md5Hash value"
      ],
      "ignoreVersionDetection": true,
      "installAsManaged": true
    }
  ]
}
```




