---
title: Список Макослобаппс
description: Список свойств и связей объектов Макослобапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c3cb679b3ec0afc8de9f2b9ae2fa98e77784e84
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140749"
---
# <a name="list-macoslobapps"></a><span data-ttu-id="a02d7-103">Список Макослобаппс</span><span class="sxs-lookup"><span data-stu-id="a02d7-103">List macOSLobApps</span></span>

> <span data-ttu-id="a02d7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a02d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a02d7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a02d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a02d7-106">Список свойств и связей объектов [макослобапп](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a02d7-106">List properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a02d7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a02d7-107">Prerequisites</span></span>
<span data-ttu-id="a02d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a02d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a02d7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a02d7-110">Permission type</span></span>|<span data-ttu-id="a02d7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a02d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a02d7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a02d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a02d7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a02d7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a02d7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a02d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a02d7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a02d7-115">Not supported.</span></span>|
|<span data-ttu-id="a02d7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a02d7-116">Application</span></span>|<span data-ttu-id="a02d7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a02d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a02d7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a02d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a02d7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a02d7-119">Request headers</span></span>
|<span data-ttu-id="a02d7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a02d7-120">Header</span></span>|<span data-ttu-id="a02d7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a02d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a02d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a02d7-122">Authorization</span></span>|<span data-ttu-id="a02d7-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a02d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a02d7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a02d7-124">Accept</span></span>|<span data-ttu-id="a02d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a02d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a02d7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a02d7-126">Request body</span></span>
<span data-ttu-id="a02d7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a02d7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a02d7-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a02d7-128">Response</span></span>
<span data-ttu-id="a02d7-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макослобапп](../resources/intune-apps-macoslobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a02d7-129">If successful, this method returns a `200 OK` response code and a collection of [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a02d7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a02d7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a02d7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a02d7-131">Request</span></span>
<span data-ttu-id="a02d7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a02d7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="a02d7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a02d7-133">Response</span></span>
<span data-ttu-id="a02d7-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a02d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1968

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
        "v10_13": true
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
      "ignoreVersionDetection": true
    }
  ]
}
```




