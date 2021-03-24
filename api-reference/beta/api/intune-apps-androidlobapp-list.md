---
title: Перечисление объектов androidLobApp
description: Список свойств и связей объектов androidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9cb631216656d64d56fa7823bf5f45116b6253f2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144454"
---
# <a name="list-androidlobapps"></a><span data-ttu-id="cb2f1-103">Перечисление объектов androidLobApp</span><span class="sxs-lookup"><span data-stu-id="cb2f1-103">List androidLobApps</span></span>

<span data-ttu-id="cb2f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb2f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb2f1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb2f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb2f1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb2f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb2f1-107">Список свойств и связей объектов [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb2f1-107">List properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb2f1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cb2f1-108">Prerequisites</span></span>
<span data-ttu-id="cb2f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb2f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb2f1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb2f1-111">Permission type</span></span>|<span data-ttu-id="cb2f1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb2f1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb2f1-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb2f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb2f1-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb2f1-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb2f1-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb2f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb2f1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb2f1-116">Not supported.</span></span>|
|<span data-ttu-id="cb2f1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb2f1-117">Application</span></span>|<span data-ttu-id="cb2f1-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb2f1-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb2f1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb2f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cb2f1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cb2f1-120">Request headers</span></span>
|<span data-ttu-id="cb2f1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb2f1-121">Header</span></span>|<span data-ttu-id="cb2f1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb2f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb2f1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb2f1-123">Authorization</span></span>|<span data-ttu-id="cb2f1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb2f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb2f1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb2f1-125">Accept</span></span>|<span data-ttu-id="cb2f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb2f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb2f1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb2f1-127">Request body</span></span>
<span data-ttu-id="cb2f1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb2f1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb2f1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb2f1-129">Response</span></span>
<span data-ttu-id="cb2f1-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidLobApp](../resources/intune-apps-androidlobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb2f1-130">If successful, this method returns a `200 OK` response code and a collection of [androidLobApp](../resources/intune-apps-androidlobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb2f1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cb2f1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb2f1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb2f1-132">Request</span></span>
<span data-ttu-id="cb2f1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb2f1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="cb2f1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb2f1-134">Response</span></span>
<span data-ttu-id="cb2f1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb2f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1931

{
  "value": [
    {
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
      "supersedingAppCount": 3,
      "supersededAppCount": 2,
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
        "v9_0": true,
        "v10_0": true,
        "v11_0": true
      },
      "versionName": "Version Name value",
      "versionCode": "Version Code value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```




