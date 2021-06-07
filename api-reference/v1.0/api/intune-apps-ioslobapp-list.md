---
title: Перечисление объектов iosLobApp
description: Список свойств и связей объектов iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ca86a998d031bee92690c40b4b61614eb0faf77
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757404"
---
# <a name="list-ioslobapps"></a><span data-ttu-id="f06f7-103">Перечисление объектов iosLobApp</span><span class="sxs-lookup"><span data-stu-id="f06f7-103">List iosLobApps</span></span>

<span data-ttu-id="f06f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f06f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f06f7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f06f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f06f7-106">Список свойств и связей объектов [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f06f7-106">List properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f06f7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f06f7-107">Prerequisites</span></span>
<span data-ttu-id="f06f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f06f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f06f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f06f7-110">Permission type</span></span>|<span data-ttu-id="f06f7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f06f7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f06f7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f06f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f06f7-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f06f7-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f06f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f06f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f06f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f06f7-115">Not supported.</span></span>|
|<span data-ttu-id="f06f7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f06f7-116">Application</span></span>|<span data-ttu-id="f06f7-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f06f7-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f06f7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f06f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f06f7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f06f7-119">Request headers</span></span>
|<span data-ttu-id="f06f7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f06f7-120">Header</span></span>|<span data-ttu-id="f06f7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f06f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f06f7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f06f7-122">Authorization</span></span>|<span data-ttu-id="f06f7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f06f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f06f7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f06f7-124">Accept</span></span>|<span data-ttu-id="f06f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f06f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f06f7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f06f7-126">Request body</span></span>
<span data-ttu-id="f06f7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f06f7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f06f7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f06f7-128">Response</span></span>
<span data-ttu-id="f06f7-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosLobApp](../resources/intune-apps-ioslobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f06f7-129">If successful, this method returns a `200 OK` response code and a collection of [iosLobApp](../resources/intune-apps-ioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f06f7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f06f7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f06f7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f06f7-131">Request</span></span>
<span data-ttu-id="f06f7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f06f7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f06f7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f06f7-133">Response</span></span>
<span data-ttu-id="f06f7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f06f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1618

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
      "publishingState": "processing",
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
      "buildNumber": "Build Number value"
    }
  ]
}
```




