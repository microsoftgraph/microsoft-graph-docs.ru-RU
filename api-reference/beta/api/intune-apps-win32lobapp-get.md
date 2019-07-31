---
title: Получение win32LobApp
description: Чтение свойств и связей объекта win32LobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 655059e6b7daac90ea0bf495ff8afbedea0bf08b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960246"
---
# <a name="get-win32lobapp"></a><span data-ttu-id="b0d54-103">Получение win32LobApp</span><span class="sxs-lookup"><span data-stu-id="b0d54-103">Get win32LobApp</span></span>

> <span data-ttu-id="b0d54-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0d54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0d54-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0d54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0d54-106">Чтение свойств и связей объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b0d54-106">Read properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0d54-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b0d54-107">Prerequisites</span></span>
<span data-ttu-id="b0d54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0d54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0d54-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0d54-110">Permission type</span></span>|<span data-ttu-id="b0d54-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0d54-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0d54-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0d54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0d54-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0d54-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b0d54-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0d54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0d54-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0d54-115">Not supported.</span></span>|
|<span data-ttu-id="b0d54-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0d54-116">Application</span></span>|<span data-ttu-id="b0d54-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0d54-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0d54-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0d54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0d54-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0d54-119">Optional query parameters</span></span>
<span data-ttu-id="b0d54-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b0d54-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0d54-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0d54-121">Request headers</span></span>
|<span data-ttu-id="b0d54-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0d54-122">Header</span></span>|<span data-ttu-id="b0d54-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b0d54-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0d54-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0d54-124">Authorization</span></span>|<span data-ttu-id="b0d54-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0d54-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0d54-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b0d54-126">Accept</span></span>|<span data-ttu-id="b0d54-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b0d54-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0d54-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0d54-128">Request body</span></span>
<span data-ttu-id="b0d54-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0d54-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0d54-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0d54-130">Response</span></span>
<span data-ttu-id="b0d54-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0d54-131">If successful, this method returns a `200 OK` response code and [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0d54-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b0d54-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0d54-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0d54-133">Request</span></span>
<span data-ttu-id="b0d54-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0d54-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="b0d54-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0d54-135">Response</span></span>
<span data-ttu-id="b0d54-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0d54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3151

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
      "packageType": "perUser",
      "productName": "Product Name value",
      "publisher": "Publisher value"
    },
    "setupFilePath": "Setup File Path value"
  }
}
```





