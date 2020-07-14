---
title: Получение win32LobApp
description: Чтение свойств и связей объекта win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5b9141829fa7e321d8447ca8b499511bcf8ae0b5
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123451"
---
# <a name="get-win32lobapp"></a><span data-ttu-id="8fba6-103">Получение win32LobApp</span><span class="sxs-lookup"><span data-stu-id="8fba6-103">Get win32LobApp</span></span>

<span data-ttu-id="8fba6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fba6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fba6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fba6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fba6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8fba6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fba6-107">Чтение свойств и связей объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8fba6-107">Read properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fba6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8fba6-108">Prerequisites</span></span>
<span data-ttu-id="8fba6-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8fba6-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8fba6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fba6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fba6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fba6-111">Permission type</span></span>|<span data-ttu-id="8fba6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fba6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fba6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fba6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fba6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fba6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8fba6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fba6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fba6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fba6-116">Not supported.</span></span>|
|<span data-ttu-id="8fba6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fba6-117">Application</span></span>|<span data-ttu-id="8fba6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fba6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fba6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fba6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8fba6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8fba6-120">Optional query parameters</span></span>
<span data-ttu-id="8fba6-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8fba6-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8fba6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fba6-122">Request headers</span></span>
|<span data-ttu-id="8fba6-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8fba6-123">Header</span></span>|<span data-ttu-id="8fba6-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8fba6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fba6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8fba6-125">Authorization</span></span>|<span data-ttu-id="8fba6-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fba6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fba6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8fba6-127">Accept</span></span>|<span data-ttu-id="8fba6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8fba6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fba6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fba6-129">Request body</span></span>
<span data-ttu-id="8fba6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8fba6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fba6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fba6-131">Response</span></span>
<span data-ttu-id="8fba6-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8fba6-132">If successful, this method returns a `200 OK` response code and [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fba6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8fba6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fba6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fba6-134">Request</span></span>
<span data-ttu-id="8fba6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fba6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="8fba6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fba6-136">Response</span></span>
<span data-ttu-id="8fba6-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="8fba6-137">Here is an example of the response.</span></span> <span data-ttu-id="8fba6-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="8fba6-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8fba6-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="8fba6-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3707

{
  "value": {
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
      "v10_1903": true
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
    "installLanguage": "Install Language value",
    "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
  }
}
```



