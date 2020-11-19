---
title: Перечисление объектов managedIOSLobApp
description: Список свойств и связей объектов managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b882ab0f65602bd34664d7ae5199f84686dcdd4e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49249773"
---
# <a name="list-managedioslobapps"></a><span data-ttu-id="f0f70-103">Перечисление объектов managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="f0f70-103">List managedIOSLobApps</span></span>

<span data-ttu-id="f0f70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0f70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0f70-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0f70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0f70-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0f70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0f70-107">Список свойств и связей объектов [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0f70-107">List properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0f70-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0f70-108">Prerequisites</span></span>
<span data-ttu-id="f0f70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0f70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0f70-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0f70-111">Permission type</span></span>|<span data-ttu-id="f0f70-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0f70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0f70-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0f70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0f70-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0f70-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f0f70-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0f70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0f70-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0f70-116">Not supported.</span></span>|
|<span data-ttu-id="f0f70-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f0f70-117">Application</span></span>|<span data-ttu-id="f0f70-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0f70-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0f70-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0f70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f0f70-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f0f70-120">Request headers</span></span>
|<span data-ttu-id="f0f70-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0f70-121">Header</span></span>|<span data-ttu-id="f0f70-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0f70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0f70-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0f70-123">Authorization</span></span>|<span data-ttu-id="f0f70-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0f70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0f70-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0f70-125">Accept</span></span>|<span data-ttu-id="f0f70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0f70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0f70-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0f70-127">Request body</span></span>
<span data-ttu-id="f0f70-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0f70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0f70-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0f70-129">Response</span></span>
<span data-ttu-id="f0f70-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0f70-130">If successful, this method returns a `200 OK` response code and a collection of [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0f70-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f0f70-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0f70-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0f70-132">Request</span></span>
<span data-ttu-id="f0f70-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0f70-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f0f70-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0f70-134">Response</span></span>
<span data-ttu-id="f0f70-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0f70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1955

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedIOSLobApp",
      "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "bundleId": "Bundle Id value",
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
        "v8_0": true,
        "v9_0": true,
        "v10_0": true,
        "v11_0": true,
        "v12_0": true,
        "v13_0": true
      },
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "versionNumber": "Version Number value",
      "buildNumber": "Build Number value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```




