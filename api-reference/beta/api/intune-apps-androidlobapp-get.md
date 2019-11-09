---
title: Get androidLobApp
description: Чтение свойств и связей объекта androidLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5524e240cf3b6e2536e187410edc4512a1047a0
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38081039"
---
# <a name="get-androidlobapp"></a><span data-ttu-id="51870-103">Get androidLobApp</span><span class="sxs-lookup"><span data-stu-id="51870-103">Get androidLobApp</span></span>

> <span data-ttu-id="51870-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51870-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51870-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51870-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51870-106">Чтение свойств и связей объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="51870-106">Read properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51870-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="51870-107">Prerequisites</span></span>
<span data-ttu-id="51870-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51870-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51870-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51870-110">Permission type</span></span>|<span data-ttu-id="51870-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51870-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51870-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51870-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51870-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51870-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="51870-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51870-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51870-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51870-115">Not supported.</span></span>|
|<span data-ttu-id="51870-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51870-116">Application</span></span>|<span data-ttu-id="51870-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51870-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51870-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51870-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51870-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51870-119">Optional query parameters</span></span>
<span data-ttu-id="51870-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51870-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51870-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51870-121">Request headers</span></span>
|<span data-ttu-id="51870-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51870-122">Header</span></span>|<span data-ttu-id="51870-123">Значение</span><span class="sxs-lookup"><span data-stu-id="51870-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51870-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51870-124">Authorization</span></span>|<span data-ttu-id="51870-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51870-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51870-126">Accept</span><span class="sxs-lookup"><span data-stu-id="51870-126">Accept</span></span>|<span data-ttu-id="51870-127">application/json</span><span class="sxs-lookup"><span data-stu-id="51870-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51870-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51870-128">Request body</span></span>
<span data-ttu-id="51870-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51870-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51870-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="51870-130">Response</span></span>
<span data-ttu-id="51870-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="51870-131">If successful, this method returns a `200 OK` response code and [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51870-132">Пример</span><span class="sxs-lookup"><span data-stu-id="51870-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="51870-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="51870-133">Request</span></span>
<span data-ttu-id="51870-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51870-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="51870-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="51870-135">Response</span></span>
<span data-ttu-id="51870-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51870-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1704

{
  "value": {
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
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "dependentAppCount": 1,
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
}
```






