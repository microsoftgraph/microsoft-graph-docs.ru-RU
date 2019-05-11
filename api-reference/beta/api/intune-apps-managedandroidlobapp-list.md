---
title: Перечисление объектов managedAndroidLobApp
description: Список свойств и связей объектов managedAndroidLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdacd1afc66a6e90aca23e136dbe7e9f6b58060d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935778"
---
# <a name="list-managedandroidlobapps"></a><span data-ttu-id="cf601-103">Перечисление объектов managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="cf601-103">List managedAndroidLobApps</span></span>

> <span data-ttu-id="cf601-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf601-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf601-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf601-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf601-106">Список свойств и связей объектов [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf601-106">List properties and relationships of the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf601-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cf601-107">Prerequisites</span></span>
<span data-ttu-id="cf601-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf601-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf601-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf601-110">Permission type</span></span>|<span data-ttu-id="cf601-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf601-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf601-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf601-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf601-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf601-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cf601-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf601-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf601-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf601-115">Not supported.</span></span>|
|<span data-ttu-id="cf601-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf601-116">Application</span></span>|<span data-ttu-id="cf601-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf601-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf601-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf601-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cf601-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf601-119">Request headers</span></span>
|<span data-ttu-id="cf601-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf601-120">Header</span></span>|<span data-ttu-id="cf601-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cf601-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf601-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf601-122">Authorization</span></span>|<span data-ttu-id="cf601-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf601-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf601-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cf601-124">Accept</span></span>|<span data-ttu-id="cf601-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf601-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf601-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf601-126">Request body</span></span>
<span data-ttu-id="cf601-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf601-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf601-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf601-128">Response</span></span>
<span data-ttu-id="cf601-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf601-129">If successful, this method returns a `200 OK` response code and a collection of [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf601-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cf601-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf601-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf601-131">Request</span></span>
<span data-ttu-id="cf601-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf601-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="cf601-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf601-133">Response</span></span>
<span data-ttu-id="cf601-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf601-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1904

{
  "value": [
    {
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
      "dependentAppCount": 1,
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
  ]
}
```




