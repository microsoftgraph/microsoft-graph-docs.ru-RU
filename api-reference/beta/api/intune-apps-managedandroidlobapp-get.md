---
title: Get managedAndroidLobApp
description: Чтение свойств и связей объекта managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 332803ab731e436d5c11297c049e6c4d225cf36c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978950"
---
# <a name="get-managedandroidlobapp"></a><span data-ttu-id="cada7-103">Get managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="cada7-103">Get managedAndroidLobApp</span></span>

> <span data-ttu-id="cada7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cada7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cada7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cada7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cada7-106">Чтение свойств и связей объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cada7-106">Read properties and relationships of the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cada7-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cada7-107">Prerequisites</span></span>
<span data-ttu-id="cada7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cada7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cada7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cada7-110">Permission type</span></span>|<span data-ttu-id="cada7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cada7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cada7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cada7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cada7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cada7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cada7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cada7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cada7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cada7-115">Not supported.</span></span>|
|<span data-ttu-id="cada7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cada7-116">Application</span></span>|<span data-ttu-id="cada7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cada7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cada7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cada7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cada7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cada7-119">Optional query parameters</span></span>
<span data-ttu-id="cada7-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cada7-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cada7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cada7-121">Request headers</span></span>
|<span data-ttu-id="cada7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cada7-122">Header</span></span>|<span data-ttu-id="cada7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cada7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cada7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cada7-124">Authorization</span></span>|<span data-ttu-id="cada7-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cada7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cada7-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cada7-126">Accept</span></span>|<span data-ttu-id="cada7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cada7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cada7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cada7-128">Request body</span></span>
<span data-ttu-id="cada7-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cada7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cada7-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="cada7-130">Response</span></span>
<span data-ttu-id="cada7-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cada7-131">If successful, this method returns a `200 OK` response code and [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cada7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cada7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cada7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cada7-133">Request</span></span>
<span data-ttu-id="cada7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cada7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="cada7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cada7-135">Response</span></span>
<span data-ttu-id="cada7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cada7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1757

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAndroidLobApp",
    "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
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




