---
title: Перечисление объектов managedAndroidStoreApp
description: Список свойств и связей объектов managedAndroidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d12ed2fc89f26551db445f4a52ec7ad31a7dee08
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451058"
---
# <a name="list-managedandroidstoreapps"></a><span data-ttu-id="aa387-103">Перечисление объектов managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="aa387-103">List managedAndroidStoreApps</span></span>

<span data-ttu-id="aa387-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aa387-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa387-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa387-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa387-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa387-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa387-107">Список свойств и связей объектов [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="aa387-107">List properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa387-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aa387-108">Prerequisites</span></span>
<span data-ttu-id="aa387-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa387-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa387-111">Permission type</span></span>|<span data-ttu-id="aa387-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa387-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa387-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa387-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa387-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa387-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="aa387-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa387-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa387-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa387-116">Not supported.</span></span>|
|<span data-ttu-id="aa387-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa387-117">Application</span></span>|<span data-ttu-id="aa387-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa387-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa387-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa387-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="aa387-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aa387-120">Request headers</span></span>
|<span data-ttu-id="aa387-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa387-121">Header</span></span>|<span data-ttu-id="aa387-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aa387-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa387-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa387-123">Authorization</span></span>|<span data-ttu-id="aa387-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa387-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa387-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa387-125">Accept</span></span>|<span data-ttu-id="aa387-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa387-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa387-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa387-127">Request body</span></span>
<span data-ttu-id="aa387-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa387-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa387-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa387-129">Response</span></span>
<span data-ttu-id="aa387-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa387-130">If successful, this method returns a `200 OK` response code and a collection of [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa387-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aa387-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa387-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa387-132">Request</span></span>
<span data-ttu-id="aa387-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa387-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="aa387-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa387-134">Response</span></span>
<span data-ttu-id="aa387-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa387-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1653

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
        "v9_0": true
      }
    }
  ]
}
```





