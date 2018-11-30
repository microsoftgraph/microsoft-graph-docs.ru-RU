---
title: Список win32LobApps
description: Свойства списка и связей объектов win32LobApp.
ms.openlocfilehash: ffb4e677ab7481e0bdab94f7300c9ba20e04f8fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082666"
---
# <a name="list-win32lobapps"></a><span data-ttu-id="fa62f-103">Список win32LobApps</span><span class="sxs-lookup"><span data-stu-id="fa62f-103">List win32LobApps</span></span>

> <span data-ttu-id="fa62f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa62f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa62f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa62f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa62f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fa62f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa62f-107">Свойства списка и связей объектов [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="fa62f-107">List properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa62f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fa62f-108">Prerequisites</span></span>
<span data-ttu-id="fa62f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa62f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa62f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa62f-111">Permission type</span></span>|<span data-ttu-id="fa62f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa62f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa62f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa62f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa62f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa62f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fa62f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa62f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa62f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa62f-116">Not supported.</span></span>|
|<span data-ttu-id="fa62f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa62f-117">Application</span></span>|<span data-ttu-id="fa62f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa62f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa62f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa62f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fa62f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa62f-120">Request headers</span></span>
|<span data-ttu-id="fa62f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa62f-121">Header</span></span>|<span data-ttu-id="fa62f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fa62f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa62f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa62f-123">Authorization</span></span>|<span data-ttu-id="fa62f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fa62f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa62f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa62f-125">Accept</span></span>|<span data-ttu-id="fa62f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa62f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa62f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa62f-127">Request body</span></span>
<span data-ttu-id="fa62f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa62f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa62f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa62f-129">Response</span></span>
<span data-ttu-id="fa62f-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [win32LobApp](../resources/intune-apps-win32lobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fa62f-130">If successful, this method returns a `200 OK` response code and a collection of [win32LobApp](../resources/intune-apps-win32lobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa62f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fa62f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa62f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa62f-132">Request</span></span>
<span data-ttu-id="fa62f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa62f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="fa62f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa62f-134">Response</span></span>
<span data-ttu-id="fa62f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="fa62f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2689

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.win32LobApp",
      "id": "9607b530-b530-9607-30b5-079630b50796",
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
      "installCommandLine": "Install Command Line value",
      "uninstallCommandLine": "Uninstall Command Line value",
      "applicableArchitectures": "x86",
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
      "minimumFreeDiskSpaceInMB": 8,
      "minimumMemoryInMB": 1,
      "minimumNumberOfProcessors": 9,
      "minimumCpuSpeedInMHz": 4,
      "detectionRules": [
        {
          "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
          "check32BitOn64System": true,
          "keyPath": "Key Path value",
          "valueName": "Value Name value",
          "detectionType": "exists",
          "operator": "equal",
          "detectionValue": "Detection Value value"
        }
      ],
      "installExperience": {
        "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
        "runAsAccount": "user"
      },
      "returnCodes": [
        {
          "@odata.type": "microsoft.graph.win32LobAppReturnCode",
          "returnCode": 10,
          "type": "success"
        }
      ],
      "msiInformation": {
        "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
        "productCode": "Product Code value",
        "productVersion": "Product Version value",
        "upgradeCode": "Upgrade Code value",
        "requiresReboot": true,
        "packageType": "perUser"
      },
      "setupFilePath": "Setup File Path value"
    }
  ]
}
```





