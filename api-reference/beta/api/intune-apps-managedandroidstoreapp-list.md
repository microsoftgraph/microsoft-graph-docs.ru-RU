---
title: Перечисление объектов managedAndroidStoreApp
description: Список свойств и связей объектов managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42ee8d04b8b25bd5cf14ed82733ef149dc8f4a60
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143719"
---
# <a name="list-managedandroidstoreapps"></a><span data-ttu-id="06108-103">Перечисление объектов managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="06108-103">List managedAndroidStoreApps</span></span>

<span data-ttu-id="06108-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06108-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06108-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06108-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06108-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06108-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06108-107">Список свойств и связей объектов [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="06108-107">List properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06108-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="06108-108">Prerequisites</span></span>
<span data-ttu-id="06108-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06108-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06108-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06108-111">Permission type</span></span>|<span data-ttu-id="06108-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06108-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06108-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06108-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06108-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06108-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06108-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06108-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06108-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06108-116">Not supported.</span></span>|
|<span data-ttu-id="06108-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="06108-117">Application</span></span>|<span data-ttu-id="06108-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06108-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06108-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06108-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="06108-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="06108-120">Request headers</span></span>
|<span data-ttu-id="06108-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06108-121">Header</span></span>|<span data-ttu-id="06108-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06108-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06108-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06108-123">Authorization</span></span>|<span data-ttu-id="06108-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06108-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06108-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06108-125">Accept</span></span>|<span data-ttu-id="06108-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06108-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06108-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06108-127">Request body</span></span>
<span data-ttu-id="06108-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06108-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06108-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="06108-129">Response</span></span>
<span data-ttu-id="06108-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06108-130">If successful, this method returns a `200 OK` response code and a collection of [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06108-131">Пример</span><span class="sxs-lookup"><span data-stu-id="06108-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="06108-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="06108-132">Request</span></span>
<span data-ttu-id="06108-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06108-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="06108-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="06108-134">Response</span></span>
<span data-ttu-id="06108-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06108-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1766

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
      "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
        "v6_0": true,
        "v7_0": true,
        "v7_1": true,
        "v8_0": true,
        "v8_1": true,
        "v9_0": true,
        "v10_0": true,
        "v11_0": true
      }
    }
  ]
}
```




