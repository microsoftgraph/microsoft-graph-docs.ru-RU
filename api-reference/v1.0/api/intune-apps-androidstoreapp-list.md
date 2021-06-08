---
title: Перечисление объектов androidStoreApp
description: Список свойств и связей объектов androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db35dbfa796a1dabc68c1f083039dbb2106148b3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757677"
---
# <a name="list-androidstoreapps"></a><span data-ttu-id="a91f6-103">Перечисление объектов androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="a91f6-103">List androidStoreApps</span></span>

<span data-ttu-id="a91f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a91f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a91f6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a91f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a91f6-106">Список свойств и связей объектов [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="a91f6-106">List properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a91f6-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a91f6-107">Prerequisites</span></span>
<span data-ttu-id="a91f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a91f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a91f6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a91f6-110">Permission type</span></span>|<span data-ttu-id="a91f6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a91f6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a91f6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a91f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a91f6-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a91f6-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a91f6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a91f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a91f6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a91f6-115">Not supported.</span></span>|
|<span data-ttu-id="a91f6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a91f6-116">Application</span></span>|<span data-ttu-id="a91f6-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a91f6-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a91f6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a91f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a91f6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a91f6-119">Request headers</span></span>
|<span data-ttu-id="a91f6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a91f6-120">Header</span></span>|<span data-ttu-id="a91f6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a91f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a91f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a91f6-122">Authorization</span></span>|<span data-ttu-id="a91f6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a91f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a91f6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a91f6-124">Accept</span></span>|<span data-ttu-id="a91f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a91f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a91f6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a91f6-126">Request body</span></span>
<span data-ttu-id="a91f6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a91f6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a91f6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a91f6-128">Response</span></span>
<span data-ttu-id="a91f6-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a91f6-129">If successful, this method returns a `200 OK` response code and a collection of [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a91f6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a91f6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a91f6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a91f6-131">Request</span></span>
<span data-ttu-id="a91f6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a91f6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="a91f6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a91f6-133">Response</span></span>
<span data-ttu-id="a91f6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a91f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1319

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidStoreApp",
      "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
      "packageId": "Package Id value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
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
        "v10_0": true,
        "v11_0": true
      }
    }
  ]
}
```




