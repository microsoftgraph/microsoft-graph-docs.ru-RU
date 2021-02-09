---
title: Перечисление объектов iosLobApp
description: Список свойств и связей объектов iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8a2c48c9af397eea53329e2c4601aa358ec1c1d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156254"
---
# <a name="list-ioslobapps"></a><span data-ttu-id="cdf04-103">Перечисление объектов iosLobApp</span><span class="sxs-lookup"><span data-stu-id="cdf04-103">List iosLobApps</span></span>

<span data-ttu-id="cdf04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdf04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdf04-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdf04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdf04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdf04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdf04-107">Список свойств и связей объектов [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdf04-107">List properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdf04-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cdf04-108">Prerequisites</span></span>
<span data-ttu-id="cdf04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdf04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdf04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdf04-111">Permission type</span></span>|<span data-ttu-id="cdf04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdf04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdf04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdf04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdf04-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdf04-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cdf04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdf04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdf04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdf04-116">Not supported.</span></span>|
|<span data-ttu-id="cdf04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdf04-117">Application</span></span>|<span data-ttu-id="cdf04-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdf04-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdf04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdf04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cdf04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cdf04-120">Request headers</span></span>
|<span data-ttu-id="cdf04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdf04-121">Header</span></span>|<span data-ttu-id="cdf04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cdf04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdf04-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdf04-123">Authorization</span></span>|<span data-ttu-id="cdf04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdf04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdf04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cdf04-125">Accept</span></span>|<span data-ttu-id="cdf04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdf04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdf04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdf04-127">Request body</span></span>
<span data-ttu-id="cdf04-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdf04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdf04-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdf04-129">Response</span></span>
<span data-ttu-id="cdf04-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosLobApp](../resources/intune-apps-ioslobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cdf04-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobApp](../resources/intune-apps-ioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdf04-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cdf04-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdf04-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdf04-132">Request</span></span>
<span data-ttu-id="cdf04-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdf04-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="cdf04-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdf04-134">Response</span></span>
<span data-ttu-id="cdf04-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdf04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1893

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobApp",
      "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
        "v13_0": true,
        "v14_0": true
      },
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "versionNumber": "Version Number value",
      "buildNumber": "Build Number value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```




