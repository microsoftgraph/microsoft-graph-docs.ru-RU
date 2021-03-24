---
title: Список win32LobApps
description: Список свойств и связей объектов win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3813e3a192a76c32ed1335fc9f1cd26618b14d81
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139158"
---
# <a name="list-win32lobapps"></a><span data-ttu-id="030c7-103">Список win32LobApps</span><span class="sxs-lookup"><span data-stu-id="030c7-103">List win32LobApps</span></span>

<span data-ttu-id="030c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="030c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="030c7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="030c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="030c7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="030c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="030c7-107">Список свойств и связей объектов [win32LobApp.](../resources/intune-apps-win32lobapp.md)</span><span class="sxs-lookup"><span data-stu-id="030c7-107">List properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="030c7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="030c7-108">Prerequisites</span></span>
<span data-ttu-id="030c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="030c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="030c7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="030c7-111">Permission type</span></span>|<span data-ttu-id="030c7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="030c7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="030c7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="030c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="030c7-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="030c7-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="030c7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="030c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="030c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="030c7-116">Not supported.</span></span>|
|<span data-ttu-id="030c7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="030c7-117">Application</span></span>|<span data-ttu-id="030c7-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="030c7-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="030c7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="030c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="030c7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="030c7-120">Request headers</span></span>
|<span data-ttu-id="030c7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="030c7-121">Header</span></span>|<span data-ttu-id="030c7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="030c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="030c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="030c7-123">Authorization</span></span>|<span data-ttu-id="030c7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="030c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="030c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="030c7-125">Accept</span></span>|<span data-ttu-id="030c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="030c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="030c7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="030c7-127">Request body</span></span>
<span data-ttu-id="030c7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="030c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="030c7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="030c7-129">Response</span></span>
<span data-ttu-id="030c7-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="030c7-130">If successful, this method returns a `200 OK` response code and a collection of [win32LobApp](../resources/intune-apps-win32lobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="030c7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="030c7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="030c7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="030c7-132">Request</span></span>
<span data-ttu-id="030c7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="030c7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="030c7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="030c7-134">Response</span></span>
<span data-ttu-id="030c7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="030c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4050

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
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true,
        "v10_1909": true,
        "v10_2004": true
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
      "requirementRules": [
        {
          "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
          "operator": "equal",
          "detectionValue": "Detection Value value",
          "check32BitOn64System": true,
          "keyPath": "Key Path value",
          "valueName": "Value Name value",
          "detectionType": "exists"
        }
      ],
      "rules": [
        {
          "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
          "ruleType": "requirement",
          "check32BitOn64System": true,
          "keyPath": "Key Path value",
          "valueName": "Value Name value",
          "operationType": "exists",
          "operator": "equal",
          "comparisonValue": "Comparison Value value"
        }
      ],
      "installExperience": {
        "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
        "runAsAccount": "user",
        "deviceRestartBehavior": "allow"
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
        "packageType": "perUser",
        "productName": "Product Name value",
        "publisher": "Publisher value"
      },
      "setupFilePath": "Setup File Path value",
      "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value",
      "displayVersion": "Display Version value"
    }
  ]
}
```




