---
title: Список androidManagedStoreApps
description: Список свойств и связей объектов AndroidManagedStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f73d6dce942731a02753a1498d5848860af2515
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140982"
---
# <a name="list-androidmanagedstoreapps"></a><span data-ttu-id="01e51-103">Список androidManagedStoreApps</span><span class="sxs-lookup"><span data-stu-id="01e51-103">List androidManagedStoreApps</span></span>

<span data-ttu-id="01e51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01e51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01e51-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01e51-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01e51-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01e51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01e51-107">Список свойств и связей объектов [AndroidManagedStoreApp.](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="01e51-107">List properties and relationships of the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01e51-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01e51-108">Prerequisites</span></span>
<span data-ttu-id="01e51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01e51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01e51-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01e51-111">Permission type</span></span>|<span data-ttu-id="01e51-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01e51-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01e51-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01e51-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01e51-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01e51-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01e51-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01e51-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01e51-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01e51-116">Not supported.</span></span>|
|<span data-ttu-id="01e51-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="01e51-117">Application</span></span>|<span data-ttu-id="01e51-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01e51-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01e51-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01e51-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="01e51-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="01e51-120">Request headers</span></span>
|<span data-ttu-id="01e51-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01e51-121">Header</span></span>|<span data-ttu-id="01e51-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01e51-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01e51-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01e51-123">Authorization</span></span>|<span data-ttu-id="01e51-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01e51-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01e51-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01e51-125">Accept</span></span>|<span data-ttu-id="01e51-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01e51-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01e51-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01e51-127">Request body</span></span>
<span data-ttu-id="01e51-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01e51-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01e51-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="01e51-129">Response</span></span>
<span data-ttu-id="01e51-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="01e51-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01e51-131">Пример</span><span class="sxs-lookup"><span data-stu-id="01e51-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="01e51-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="01e51-132">Request</span></span>
<span data-ttu-id="01e51-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01e51-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="01e51-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="01e51-134">Response</span></span>
<span data-ttu-id="01e51-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01e51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1598

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreApp",
      "id": "87247525-7525-8724-2575-248725752487",
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
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "isPrivate": true,
      "isSystemApp": true,
      "appTracks": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
          "trackId": "Track Id value",
          "trackAlias": "Track Alias value"
        }
      ],
      "supportsOemConfig": true
    }
  ]
}
```




